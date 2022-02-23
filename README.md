- Fantasy sports custom scheduler for leagues with two divisions
- Ideal for 10 team or 12 team leagues playing over 14 weeks
- "Offsets" are used to create inter-divisional matchups

10 TEAM Schedule:

- Play each team in your division twice
- Play one team in the other division twice (aka rival)
- Play the other 4 teams in the other division once

Week 1: Inter-division with 1 offset matchup
Weeks 2-6: 4 Intra-division games + 1 inter-division offset matchup (#2)
Weeks 7: Inter-division matchup with 1 offset matchup (#3)
Weeks 8 & 9: Inter-division matchup with 1 offset matchup (#0 aka rivals)
Weeks 10-14: 4 Intra-division games + 1 inter-division offset matchup (#4)
EXAMPLE Code:

Run following command:
$ ./fantasyscheduler.py --div1 a b c d e --div2 m n l o p --inter 1 --intra 2 --inter 3 0 0 -- intra 4 -- distribution

12 TEAM Schedule:

- Play each team in your division twice
- Play one game against teams in the other division

Weeks 1-5: Intra-division games
Weeks 6-11: Inter-division games with offset matchups (0-5)
Weeks 12-16: Intra-division games

Run following command:
$ ./fantasyscheduler.py --div1 a b c d e f --div2 m n l o p q --intra --inter 0 1 2 3 4 5 --intra --distribution

HELP:
Run following command:
$ ./fantasyscheduler.py --help
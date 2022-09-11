# What's The Largest Number In A Video Game Title?
There are a few reasons why game designers include numbers in the titles of their games. Whether it's to point out a prior sequence (Uncharted 2, Borderlands 3), mention a year (FIFA 2022, Cyberpunk 2077) or to describe a quantifiable measurement (Action 52, 10-Pin Bowling), there are many reasons to why a game would have a number in its title.

This raises an interesting question. What is the **largest** number on a video game title?

To answer this, I need a list of video games. Thankfully, there exists [a list](https://archive.ph/PXf1r) of ~40,000 video game titles. However, here's how the first few lines look like...

```
005 (1981, SEGA Enterprises Ltd.) (Arcade)
007: Agent Under Fire (2001, Electronic Arts, Inc., Electronic Arts Ltd.) (GameCube, PlayStation 2, Xbox)
007: Blood Stone (2010, Activision Publishing, Inc., ak tronic Software & Services GmbH) (PlayStation 3, Windows, Xbox 360)
007 Car Chase (1985, Coplin Software) (Commodore 64)
007: Everything or Nothing (2003, Electronic Arts, Inc.) (Game Boy Advance)
```

In other words, every line isn't JUST a video game title. There's also both the video game publisher and the console it was released on. Using some Regex, I can grab the video game titles.

```
005
007: Agent Under Fire
007: Blood Stone
007 Car Chase
007: Everything or Nothing
```

From here, it's a matter of doing the following:
	1) Grabbing every number from every title.
	2) Selecting the highest value.

The following are video games with the largest number in their titles.

| Number | Game Name                                 | Number     |
|:------:|-------------------------------------------|------------|
| 1      | 10000000                                  | 10,000,000 |
| 2      | The $1000000 Pyramid                      | 1,000,000  |
| 3      | 333000 Games                              | 333,000    |
| 4      | The $100000 Pyramid                       | 100,000    |
| 5      | Warhammer 40000: Squad Command            | 40,000     |
| ...    | [...22 other "Warhammer 40000" games...]  | ...        |
| 6      | 38000 Kilo no Koku                        | 38,000     |
| 7      | 25000 Sudoku Puzzles                      | 25,000     |
| 8      | 20000 Leagues Under the Sea: Captain Nemo | 20,000     |
| 9      | 20000 Leagues Under the Sea               | 20,000     |
| 10     | 10000 Games                               | 10,000     |

For context, "10,000,000" is a hybrid puzzle-role-playing game developed by EightyEightGames. The objective of the game is for the player to escape a dungeon that they've been trapped in. In order to escape, the player needs to collect 10,000,000 points through a single run in the dungeon.

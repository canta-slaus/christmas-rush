# WOK Christmas Competition

**It's almost christmas and you forgot to buy presents for your family, so you rush over to Walmart but its... Karen - she is defending Walmart for her family and you MUST get past her or else your whole family will be very upset**

# Goal of the game
Each user starts on one side of the board, either at the very top row or at the very bottom row. The goal is to move to the other side. Means, if you started at the top, you need to move down and vice versa.\
Additionally, in a ranked game, two presents will be randomly placed on the board. Each user has to get one present before they can win by moving to the other side.

# How to play
The game starts with a blank board with randomly placed barriers.\
![Game board](https://imgur.com/oM4XJSJ.png)\
_Whose turn it is will be displayed at the bottom of the image._
In the first turn, both users get to chose which column they would like to start on. To do that, simply reply with the column letter when it's your turn.\
![First turns](https://imgur.com/iJgvaED.png)\
In this example, both users decided to start on `E`/`e`.\
_The Grinch (red) starts at the bottom, while Santa (blue) starts at the top._\
After that, each turn a user can either move or place a wall.

## Moving
`mw` - move up (the directions are the same for both players)\
`ms` - move down\
`md` - move right\
`ma` - move left\
So basically, standard WASD but with an extra `m` at the beginning.\
You, obviously, can not move out of the map or move through walls.\
It is the Grinch's turn and by doing `mw`, he moves up by one.\
![Grinch moves up](https://imgur.com/rUaj8LU.png)\
### Jumping over the opponent
![Jumping](https://imgur.com/ApldtpX.png)\
It is Santa's turn and one addition to moving is: Jumping over the opponent, that is: Santa can't simply do `ms`, as he would then stand on the Grinch.\
However, what Santa can do is: e.g. `mss` to jump over the Grinch and then be at the tile below the Grinch. The rules for moving also apply to jumping, means, Santa can't do `msd` as that would mean that he first moves down and then tries to move through the wall, which doesn't work. Same applies for trying to move outside of the map.\
Santa decided that the best move for him would be to jump over the Grinch and move down: `mss`\
![Santa jumped over the Grinch](https://imgur.com/Vf7lyLL.png)
## Placing walls
You can place either a vertical or a horizontal wall:\
`wh` - horizontal wall\
`wv` - vertical wall\
Further, you need to specify _where_ you would like to place the wall.
For that, look at the columns denoted by letters at the top and the rows denoted by the numbers at the left. E.g. `whc1` will place a barrier horizontally on C1 (`wh1c` also works).\
Now it's Santa's turn - he noticed the Grinch getting closer to his goal but he's having none of that and places a barrier right in front of him.\
![Santa places a wall in front of the Grinch](https://imgur.com/8XiSGsz.png)\
Now, if the Grinch would move to the left two times, Santa will simply place a barrier like `wha7` and the Grinch would have to spend some turns moving around the walls on the right side.\
But be careful, each wall that you place, might cost yourself extra turns later _and trust us, every single turn matters._

# Rules
1. You can not place walls, so that any of the two users doesn't have any paths to their goal.
2. Only in ranked: You can not place walls, so that users who don't have a present, don't have a path to the remaining presents.
3. You can not place walls on top of each other. _(E.g. if you look at the last image, one could not be able to place a wall like `whb7`, but one can place one like `wvc7`)_

# Gamemodes
Currently you can challenge someone with `!!challenge @theirTag#1234`.\
You can also provide options to play with, e.g.:
- `!!challenge @theirTag#1234 ranked` (this will add the presents to the game)
- when `ranked` is enabled, you can add `nodms` so that the game will take part in the current channel and not in DM's.
- `portals`, will add portals to the map that you can use to teleport around. You can't be "inside" of a portal, means, you have to specify where you want to go if you were to move out of the other portal, similar to jumping over a player.
- `hammers`, will give both users one hammer. A hammer can be used to destroy a single 1x1 wall and consume the hammer. The syntax is `hw/ha/hs/hd`: `hw` will remove the wall above you, `ha` will remove the wall to your left, ... You have to stand next to the wall in order to destroy it.
- `candies`, will add 1-3 candy canes randomly to the map. Upon collecting a candy cane, you get another turn. So you could move, to collect the candy cane, and then move again or maybe place a wall.

# Developers
- canta#5556
- jis#2505
- EmanSza#5474

# Additional information
All art (walls, tiles, presents, users, presents and candy canes) have been made by our team.

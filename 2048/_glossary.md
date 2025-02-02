# How to Make 2048: Glossary

## NUMBERS:
```LIST LENGTHS:```
- $TsLen - list length for tile list
- $DsLen - list length for digit list
- Free - list length for list of vacant cells

```VARIABLES:```
- Spacing - the gap between cells
- Speed - tile movement speed + distance needed between a tile's current and goal position before stopping movement

```TILE PROPERTIES:```
- $TileType - type of tile: 0 for 2, 1 for 4, 2 for 8, etc.
- $TileLength - number of digits a tile has
- TileCell - index of cell the tile currently occupies

```DIGIT PROPERTIES:```
- $DigitOrder - order of digit in sublist; right to left
- $DigitTile - index of tile/sublist the digit belongs to

```CELL PROPERTIES:```
- CellValue - value of tile on top of cell

```OTHER:```
- $Tiles - number of tile types
- Check - test cell index used for checking if empty / has tile of same type

## OBJECTS:

```REFERENCES:```
- $Ds - reference digit list
- $Ts - reference tile list
- $Cell - reference cell block
- $Board - board object

```LISTS:```
- $Tile - tile list
- $Digit - digit list 
- Cell - cell list

## VECTORS:

```VARIABLES:```
- $O - origin point
- Board - board position: used for positioning cells and tiles
- Dir - swiped direction

```TILE PROPERTIES:```
- $Tile - tile current position
- $TileGoal - tile goal position

```CELL PROPERTIES:```
- Cell - cell position
- CellTiles - cell's set of tiles: stores IDs of tiles occupying the cell

```OTHER:```
- Free - list of vacant cells
- New - new goal position of a given tile after checking path
- Check - test cell position

## TRUTHS:

```STATES:```
- Spawn - if true, spawns a tile at a random position in the grid
- Check - if true, checks if the game still has any legal moves
- Moving - if true, game moves tiles towards their goal positions
- CanSpawn - tells whether the game should spawn another tile once all tiles have been moved: only becomes true if at least one of the tiles has a new goal position

```TILE PROPERTIES:```
- TileMoving - tells whether the tile is currently moving

```CELL PROPERTIES:```
- CellMerged - tells whether the cell has merged its two tiles yet

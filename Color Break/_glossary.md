# How to Make Color Break: Glossary

## NUMBERS:

```GLOBAL VARIABLES:```
- $BsLen - block list length

- $BlockColor - color of block
  - 0 - red
  - 1 - blue
  - 2 - yellow
  - 3 - green
  - 4 - blue
  - 5 - purple
- $BlockType - type of block
  - 0 - normal block
  - 1 - color changer
  - 2 - pushable block
  - 3 - danger block

```BALL PROPERTIES:```
- BallColor - current ball color
- Speed - movement speed
- Dir - current ball vertical direction
- Side - ball horizontal direction

```LIST LENGTHS:```
- PushLen - pushable block list length
- PsLen - particle list length

```DELAYS:```
- MT - delay before starting game
- WT - delay before game end
- Bump - delay when ball bounces off its side; used to invert ball horizontal direction
- Push - pushable block duration
- PsLT - particle lifetime

```OTHER:```
- PushBlock - index of corresponding block to pushable block
- Goal - number of normal blocks left
- Cam - camera distance

## OBJECTS:

```GLOBAL VARIABLES:```
- $Block - block list
- $Ball - current ball object

```IN MAIN:```
- Ball - reference ball list
- Push - pushable block list
- Ps - particle list

## VECTORS:

```EDGE COORDINATES:```
- $NE - northeast coordinate
- $SW - southwest coordinate

```IN MAIN:```
- $Ball - ball position
- Dir - ball vector direction
- Push - pushable block vector direction
- PsDir - particle vector direction
- Cam - camera position

## TRUTHS:

```IN MAIN:```
- Moving - starts the game if true
- Stop - stops the game if true
- Controls - toggles button controls: (Moving) ∧ ¬(Stop)
- Holding - returns true if player is touching a button: Side ≠ 0
- SameColor - returns true if ball color is equal to matched block's color
- BlockPush - indicates if the box is currently being pushed
- Pushed - becomes true if pushable block's duration reaches 4 frames
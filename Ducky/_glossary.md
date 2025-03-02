# How to Make Ducky: Glossary

## NUMBERS:
```LIST LENGTHS:```
- PsLen - list length of particle list
- $SsLen - list length of spike list
- $EsLen - list length of enemy list
- $KsLen - list length of key list
- $GsLen - list length of gate list

```IN DRAW PARABOLA:```
- PsLen - number of points to draw
- A - acceleration or gravity constant
- VelX - initial velocity X-value
- VelZ - initial velocity Z-value
- T - time parameter

```ENEMY PROPERTIES:```
- $EnemySpd - enemy movement speed
- $EnemyDir - enemy direction

```PARTICLE PROPERTIES:```
- PsT - particle lifetime

```OTHER:```
- Keys - number of keys the player currently has
- $Cam - camera distance

## OBJECTS:
```VARIABLES:```
- $P - player
- $Goal - goal block

```LISTS:```
- Ps - particle list
- $Spike - spike list
- $Enemy - enemy list
- $Key - key list
- $Gate - gate list

```IN DRAW PARABOLA:```
- Ps - particle point list

```ENEMY PROPERTIES:```
- $EnemyEye - enemy movable eye

## VECTORS:
```IN MAIN:```
- Start - start touch position
- Touching - current touch position
- Vel - initial velocity taken from touch positions to apply to player
- Normal - hit direction between collided objects from 2nd to 1st
- $Cam - camera position

```IN DRAW PARABOLA:```
- Start - origin or starting position
- Vel - initial velocity
- Point - particle point position

```PARTICLE PROPERTIES:```
- PsGoal - particle goal position

```KEY PROPERTIES:```
- Key - key base position

## TRUTHS:
```IN MAIN:```
- Moving - returns true if the player is currently moving
- $Stop - stops the game if true
- Controls - toggles touch controls: ¬(Moving ∨ $Stop)
- Drag - returns true if the first touch input executes
- Can - returns true if the distance between the touch positions is greater than 0

```IN DRAW PARABOLA:```
- Vis - returns true if script block is actively executing; sets the visibility of particles

```ENEMY PROPERTIES:```
- $EnemyUp - determines the movement direction of player
  - False - horizontal
  - True - vertical 

```KEY PROPERTIES:```
- KeyHas - checks if the key has been collected

```GATE PROPERTIES:```
- GateHas - checks if the gate has been unlocked
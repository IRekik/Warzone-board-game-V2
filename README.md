# Warzone Board Game

Welcome to Warzone, a strategic board game where players battle for control of territories in the solar system. This readme provides an overview of the game, including its components, rules, and setup.

## Components

### Continents
1. **Mercury:** 6 armies, Yellow color
2. **Venus:** 8 armies, Yellow color
3. **Earth:** 10 armies, Yellow color
4. **Mars:** 10 armies, Yellow color
5. **Comet:** 4 armies, Yellow color
6. **Jupiter:** 12 armies, Yellow color
7. **Saturn:** 8 armies, Yellow color
8. **Uranus:** 6 armies, Yellow color
9. **Neptune:** 6 armies, Yellow color
10. **Pluto:** 2 armies, Yellow color

### Countries
- See the `solar.map` file for the details of each territory, including name, continent, coordinates, and player ownership.

### Borders
- See the `solar.map` file for the borders between territories.

## How to Play

### Commands (from `command.txt`)
1. `loadmap solar.map`: Load the game map.
2. `validatemap`: Validate the loaded map.
3. `addplayer [name]`: Add a player to the game.
4. `gamestart`: Start the game.

### Player Class
- Players are represented by the `Player` class.
- Each player has a name, a set of armies (`reinArmy`), a hand of cards (`playerHand`), a list of orders (`playerOrdersList`), and a list of territories (`playerTerritories`).

## Player Operations

### Reinforcement
- Players receive reinforcements based on their territories.

### Issue Orders
- Players can issue various orders, such as `Deploy`, `Advance`, `Airlift`, `Bomb`, `Blockade`, and `Negotiate`.

### To Defend and To Attack
- Players can compute territories to defend and territories to attack.

## Order Classes

### Deploy
- Tells a certain number of armies to deploy to a target territory.

### Advance
- Tells a certain number of army units to move from a source territory to a target adjacent territory.

### Airlift
- Tells a certain number of armies to be moved from a source territory to a target territory.

### Bomb
- Targets a territory owned by another player, removing half of the armies.

### Blockade
- Targets a territory owned by the player, doubling the number of armies and transferring ownership to the Neutral player.

### Negotiate
- Targets an enemy player, preventing successful attacks for the remainder of the turn.

## Gameplay

- Players take turns issuing orders, reinforcing, and strategizing to conquer territories.
- The game continues until a victory condition is met.

Feel free to refer to the game's source code for detailed implementations and logic.

**Enjoy playing Warzone!**

# Creature Simulator

This is a basic Python creature simulation demonstrating object-oriented programming principles such as classes, inheritance, methods, and interaction between objects. The project includes a base `Creature` class and three specialized creatures: `SwimmingCreature`, `FlyingCreature`, and `FireCreature`, each with their own unique abilities and attack styles.

## File Structure

- `creature_simulation.py`: Defines the `Creature` base class and its subclasses (`SwimmingCreature`, `FlyingCreature`, and `FireCreature`). It also contains test cases for all creature types.

## Creature Class

The `Creature` class is the base class for all creatures. It includes:

### Attributes

- `name` (str): The creature's name.
- `hp` (int): Hit points (health).
- `attack_power` (int): Damage dealt per attack.

### Methods

- `attack(target)`: Attacks another creature and reduces its HP by `attack_power`.
- `is_alive()`: Returns `True` if HP is greater than 0.
- `__str__()`: Returns a string representation of the creature's name and current HP.

## SwimmingCreature Class

Inherits from the `Creature` class and adds underwater abilities.

### Attributes

- `depth` (int): The current underwater depth, starting at 0.

### Methods

- `dive_to(new_depth)`: Changes the creature's underwater depth.
- `attack(target)`: Performs an underwater attack and reduces the target's HP.

## FlyingCreature Class

Inherits from the `Creature` class and adds flying abilities.

### Attributes

- `altitude` (int): The current flying altitude, starting at 0.

### Methods

- `fly_to(new_altitude)`: Changes the creature's flying altitude.
- `attack(target)`: Performs an aerial attack and reduces the target's HP.

## FireCreature Class

Inherits from the `Creature` class and adds fire abilities.

### Attributes

- `fire_level` (int): The current fire level, starting at 0.

### Methods

- `emit_fire(new_fire_level)`: Changes the creature's fire level.
- `attack(target)`: Performs a fire attack and reduces the target's HP.

## How the Simulation Works

The simulation follows these steps:

1. Create different creatures, including a Goblin, Wolf, Sheep, and other test creatures.
2. Test the basic `Creature` class, including initialization, attacks, and health checks.
3. Create a `SwimmingCreature` and test its diving and underwater attack abilities.
4. Create a `FlyingCreature` and test its flying and aerial attack abilities.
5. Create a `FireCreature` and test its fire level and fire attack abilities.
6. Display the results of each test in the terminal.

## Running the Simulation

To run the simulation, execute `creature_simulation.py`:

```bash
python creature_simulation.py
```
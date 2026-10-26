# Python Game Character Stats Tracker

An **Object-Oriented Programming (OOP) workshop project** built as part of the *[freeCodeCamp](https://www.freecodecamp.org/learn/python-v9/lab-game-character-stats/lab-game-character-stats)* Python certification curriculum. This application models a game character's stats system, managing health and mana boundaries, leveling up mechanics, and custom string representation using Python properties and custom setters.

---

## Key Features

- **Object-Oriented Architecture :** Models character attributes and behaviors using standard Python OOP principles and encapsulation.
- **Encapsulation & Property Validation :** Uses `@property` decorators and custom setters to automatically clamp and enforce valid boundaries for health (`0`-`100`) and mana (`0`-`50`).
- **Dynamic Leveling System :** The `level_up()` method increments the character's level while seamlessly restoring health and mana to their maximum default values.
- **Custom String Representation :** Implements the `__str__` magic method to cleanly format and output comprehensive character stats (`Name`, `Level`, `Health`, `Mana`).

---

## Concepts & Technologies Applied

- **Python 3**
- **Object-Oriented Programming (OOP) :** Encapsulation, state management, and instance methods.
- **Decorators :** `@property`, `@<attribute>.setter` for controlled attribute modification.
- **Magic Methods :** `__init__` for initialization and `__str__` for custom object display formatting.

---

## Usage Example

```python
# Create a new character
hero = GameCharacter("Kratos")
print(hero)

# Modify stats (automatically validated and clamped by setters)
hero.health -= 30
hero.mana -= 10
print(hero)

# Level up the character
hero.level_up()
print(hero)

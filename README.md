# Hangman — Software Design Patterns in Java

A terminal Hangman game extended with classic **Gang of Four design patterns**, built as a team project for the Software Design Patterns course (University of Jeddah, 2024). I led a team of 4 and authored 26 of the project's 48 commits.

![Gameplay demo](Final.gif)

## Design patterns applied

| Pattern | Where | What it does |
|---|---|---|
| **Composite** | `Category`, `CompositeCategory`, `AnimalCategory`, `ColorCategory`, `FoodCategory` | Groups word categories so a single category or a mix of categories can be played the same way. |
| **Decorator** | `Hint`, `HintDecorator`, `HintLetter`, `HintDefinitionDecorator`, `HintDecoratorActivate` | Adds hint types (reveal a letter, show a definition) on top of a basic hint without changing it. |
| **Observer** | `GameSubject`, `HangmanObserver`, `RemainPartsObserver` | Notifies the display when the game state changes, such as the remaining body parts. |
| **Factory** | `ParserFactory`, `Parser`, `WordParser` | Creates the right parser for each word source. |

## How to run

```bash
cd hangman
javac *.java
java Hangman
```

## Tech
Java · Object-Oriented Design · Design Patterns

## Team
Jana Malibari (Team Lead) · Bushra Alandijani · Raghad Saleh · Sarah Haddad

## Credits
Built on top of [Hangman](https://github.com/michaelkolesidis/hangman) by Michael Kolesidis (GPL-3.0); the base game's license is kept in `hangman/LICENSE`. Word lists from [dwyl/english-words](https://github.com/dwyl/english-words).

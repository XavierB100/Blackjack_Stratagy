## Technical Architecture Overview

Detailed analysis of the Blackjack Strategy Master site: a simulation combining perfect basic strategy and real-time card counting.

### 🧩 Frontend Technologies

* **HTML5**: Semantic structure with game containers, card displays, and control buttons
* **CSS3**: Modern animations, gradients, responsive elements
* **JavaScript**: Game flow, card logic, strategy engine, counter, and UI updates

### ⚙️ Core Modules

1. **Game State Management**: Handles phases (deal, play, settle)
2. **Deck Simulation**: Multi-deck shoe, automatic reshuffle, standard 52-card logic
3. **Strategy Engine**: Computes correct move for every hand situation
4. **Card Counter**: Hi-Lo based running & true count with deck penetration
5. **UI Engine**: Animations, card visuals, feedback effects
6. **Statistics Tracker**: Wins/losses, pushes, blackjack frequency, win %

### 📊 Deck Management Stats

* Default: 6 decks (312 cards)
* Reshuffle threshold: 20 remaining cards (\~94% penetration)
* Distribution: Full 52-card standard per deck

### 🧮 Card Counting

* System: **Hi-Lo**

  * +1: 2–6
  * 0: 7–9
  * -1: 10–A
* True Count = Running Count / Decks Remaining (to 1 decimal)
* Real-time updates after each card
* Betting advice updates based on true count thresholds

### 📈 Performance Benchmarks

* True count update: <1ms
* Strategy lookup: <1ms
* Hand evaluation: \~0.5ms
* UI refresh: \~5ms per action

---


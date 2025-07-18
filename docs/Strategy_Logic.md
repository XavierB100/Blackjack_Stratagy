# docs/Strategy\_Logic.md

## Strategy Engine Details

Comprehensive decision engine covering all 550+ decision points for basic strategy.

### Hard Hand Logic

```javascript
function getHardHandStrategy(playerValue, dealerUpCard) {
    // Detailed decision tree for hard totals 5–21
}
```

### Soft Hand Logic

```javascript
function getSoftHandStrategy(hand, dealerUpCard) {
    // Strategy for hands with usable Aces (A,2 through A,9)
}
```

### Pair Splitting Logic

```javascript
function getPairStrategy(rank, dealerUpCard) {
    // Rules for splitting each rank, with special handling for Aces/10s
}
```

### Strategy Accuracy

* Covers hard, soft, split hands
* Adjusts for dealer rule set
* Matches published basic strategy charts

---


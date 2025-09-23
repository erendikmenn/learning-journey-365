# Entropy

In the context of data, Entropy is a measure of uncertainty or randomness within a set. It essentially tells us how mixed or impure a dataset is.

The core idea is to quantify how predictable the outcome of a random draw from the dataset would be.

* If a dataset is **pure** (contains only one class, e.g., all blue balls), the uncertainty is very low, and therefore the **Entropy is low** (or zero). We are certain about the outcome.
* If a dataset is **perfectly mixed** (an equal balance of all classes, e.g., half blue balls and half orange balls), the uncertainty is at its maximum, and the **Entropy is high**. The outcome is completely unpredictable.

---

## The Concept of "Surprise"

A helpful way to understand entropy is to think of it as the **average surprise** you would expect from an outcome.

* A **likely outcome** is not surprising, so it has a low surprise value.
* An **unlikely or rare outcome** is very surprising, so it has a high surprise value.

Entropy calculates the weighted average of the surprise for all possible outcomes.

### Practical Example: A Biased Coin

Imagine you have a biased coin that lands on **Heads 90%** of the time and **Tails 10%** of the time.

* **Getting Heads:** This is a very common outcome. It is not surprising at all.
* **Getting Tails:** This is a rare outcome. It is very surprising.

Since we are almost certain the coin will land on Heads, the overall uncertainty is low. Therefore, the average surprise, or **Entropy**, for this biased coin is very low (a value like 0.47). This low number reflects that we are fairly certain about the outcome of a flip.

### Interpreting Entropy Values

Let's look at three different datasets of colored balls to see how entropy values change:

* **Dataset A (6 Orange, 1 Blue):** This set is mostly orange. It is highly predictable that you will draw an orange ball.
    * **Result:** Low uncertainty = **Low Entropy** (e.g., 0.59).

* **Dataset B (1 Orange, 10 Blue):** This set is mostly blue. It is even more predictable than Dataset A.
    * **Result:** Very low uncertainty = **Even Lower Entropy** (e.g., 0.41).

* **Dataset C (3 Orange, 3 Blue):** This set is perfectly balanced. You have a 50/50 chance of drawing either color. It is completely unpredictable.
    * **Result:** Maximum uncertainty = **High Entropy** (e.g., 1.0).
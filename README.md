# Slacking Meow ML

Teaching [Slacking Meow](https://github.com/Bhavana123456/slacking-meow) when **not** to interrupt.

Slacking Meow sends cats when you visit a distracting site during a focus session. But not every YouTube visit is procrastination. Sometimes it's a React tutorial. This project trains a small model from my own "helpful" / "wrong time" feedback and tests whether it interrupts better than fixed site rules.

> Built from scratch as a way to learn machine learning: data, features, classification, evaluation.

## Problem

Site rules are blunt: they treat every visit to a "distracting" site the same way. Every wrong nudge makes me want to switch the tool off.

## Experiment

**Question:** can a model trained on my own corrections cut down unhelpful interruptions compared with my site rules, without missing real slacking?

- **Baseline:** current site rules (block list)
- **Model:** _to be decided as I learn_
- **Measured on:** later sessions the model has never seen

## Key decision

_To be written as the project develops._

## Results

_Coming once there's enough data._

## Limitations

_To be written honestly at the end._

## Structure

```
data/        my feedback logs (not committed)
notebooks/   exploration and experiments
src/         features, training, evaluation
server/      FastAPI service the extension calls
tests/
```

See [LEARNING.md](LEARNING.md) for the roadmap.

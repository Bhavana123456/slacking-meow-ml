# Learning roadmap

Each stage ends with something working. Tick it off before moving on.

## 1. Collect feedback (no ML yet)
- [ ] Add "helpful" / "wrong time" buttons to the cat overlay in the extension
- [ ] Log each nudge: site, page title, time, minutes into session, my label
- [ ] Gather a couple of weeks of real sessions

**Learn:** what a labelled dataset is, and why the way you collect data shapes everything later.

## 2. Explore the data
- [ ] Load it with pandas; count helpful vs. wrong-time nudges
- [ ] Look for patterns by hand: which sites, which times, which titles?

**Learn:** class imbalance, and why you look before you model.

## 3. Features
- [ ] Turn raw logs into numbers: site, hour, session progress, title keywords

**Learn:** feature engineering, and what goes wrong when information from the future leaks into training data.

## 4. Baseline first
- [ ] Score the current site rules on your data

**Learn:** why every model needs a simple baseline to beat.

## 5. First model
- [ ] Logistic regression: first understand the maths, then use scikit-learn
- [ ] Try a small decision tree and compare

**Learn:** training, weights, probabilities, decision thresholds.

## 6. Evaluate honestly
- [ ] Train on earlier sessions, test on later ones (split by time, not at random)
- [ ] Precision, recall, confusion matrix, false positives vs. false negatives

**Learn:** why accuracy alone lies, and which mistakes cost more here.

## 7. Serve it
- [ ] FastAPI endpoint: nudge context in, "interrupt?" out
- [ ] Extension asks the model before sending cats

## 8. Close the loop
- [ ] New feedback keeps flowing in; retrain and compare against the old model
- [ ] Write up Results, Key decision and Limitations in the README

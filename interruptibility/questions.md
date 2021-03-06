- Is the Jensen-Shannon divergence useful in this case? What does it tell me? Is
  it sufficient to show that it goes down drastically? Is measuring it between
  the final histogram and all histograms good? Is it better to measure it
  between adjacent (in time) pairs of histograms?

- Should I use a logarithmic plot for Jensen-Shannon? I'm using it now. Should I
  change back to linear?

- The Kullback-Leibler divergence has a more clear and well-known
  interpretation, but can't be used without modification, because the histograms
  have zeroes. Is there any way to patch over this? Does it retain its
  interpretation after patching?

- Where do those sudden jumps in the histogram development plots come from? Why
  are they not visible in the histogram with 25 bins? They occur in Sarsa(λ),
  but even more astonishingly in Q-learning where one bin on the y-axis is blue
  (red), the next green, and the next blue (red) again. (After changing the
  scale this has changed to a less drastic yellow-green (blue-green) to green
  and back.)

- Why do the histograms take so long to stabilize? Are they stable enough to
  draw valid conclusions?

- Why is the histogram for Q-learning quite stable for six million time steps
  and then starts changing again? This is even more crass when the data from
  time steps after crosses is left in.

- Why is the shape of the histogram for Q-learning more regular? Why is the
  shape of the histogram for Sarsa(λ) not regular? Actually it's quite regular
  except for the bars around and left of zero. Why does the histogram for
  Q-learning stabilize more quickly?

- Are the histograms and mean/std plots sufficient for showing how interruptions
  influence the behaviour of Sarsa(λ) and Q-learning?

- Is throwing out time steps after crosses enough to make the uninterrupted case
  a good baseline?

- How does the way I run the experiments and measure affect the apparence of
  influencedness? In other words, are Sarsa(λ) and Q-learning actually more
  influence-resistent (interruptible) than I make them appear?

- Why do the graphs of the means for Q-learning look so similar? Surely their
  trajectories should be independent.

- Why is the difference between the means (uninterrupted/interrupted) close to
  equal to the difference between standard deviations?

- Why is the variance almost constant over time?

When I ask these questions, I include programming and thinking errors of mine as
potential answers.

# Kalman Filter

Sensor fusion algorithm

In regular kalman filter, only previous state and current state are used. In the other variants like extended, multiple previous states are used

"The objective of the Kalman Filter is to minimize the mean squared error between the actual and estimated data" - MIT

It's a recursive least squares filter

### Statistical Assumptions

sensor noise is independent of x
the state, state noise, and measurement noise make a joint gaussian distribution (ALL VARIABLES ARE GAUSSIAN) and are independent

state noise is independent of the state and the observed output


### State Estimation

- Estimate the current state, based on the current and past observed outputs
- Predict the next state, also based on the current and past observed outputs

There's a standard formula for calculating both and it's simple. The Kalman filter is used to calculate the above recursively

### Markov Process (x)
only the last state is important. x(t-2) doesn't provide any more information than x(t-1).
---

## Resources

https://www.kalmanfilter.net/default.aspx
https://web.stanford.edu/class/ee363/lectures/kf.pdf
https://web.mit.edu/kirtley/kirtley/binlustuff/literature/control/Kalman%20filter.pdf
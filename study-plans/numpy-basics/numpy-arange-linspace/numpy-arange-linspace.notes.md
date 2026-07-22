**Rule of thumb:** use `arange` when you know the step size (e.g. every 0.1), use `linspace` when you know how many points you want (e.g. 100 samples between 0 and 1).

One common gotcha:

python

```python
np.arange(0, 1, 0.1)      # may give 10 or 11 elements depending on float rounding
np.linspace(0, 1, 10)     # always exactly 10 elements, guaranteed
```
# Quantum Gate Circuit Calculator

A SageMath calculator that approximates diagonal single-qubit gates using V-gates. It takes a nonzero complex number $z = a + bi$, normalises it to $\alpha = z/|z|$, and searches for a circuit approximating $\operatorname{diag}(\alpha, \overline{\alpha})$.

## Run the calculator

Open a Jupyter notebook with a **SageMath** kernel in the same directory as [`golden-gate-circuit-calculator.sage`](golden-gate-circuit-calculator.sage), then run:

```python
load("golden-gate-circuit-calculator.sage")
```

Enter the real and imaginary parts `a` and `b`, then set the **Maximum Length** and **Maximum A** sliders. The calculator displays the Diophantine approximation, the V-gate sequence, and the final unitary factor. It also plots the path through the search tree for circuits of length 1 or 2. The search is randomised, so if it finds no solution, try the same inputs again or increase the search limits.

![Example of the golden-gate circuit calculator](https://user-images.githubusercontent.com/68598333/134773818-c2ba9996-d1b9-485d-a5ee-da97dfb3f23e.jpg)

![Second example of the golden-gate circuit calculator](https://user-images.githubusercontent.com/68598333/134773820-9cbc574a-3271-4c5c-9643-1d22fbee99da.jpg)

## Reference

This project builds on Ori Parzanchevski and Peter Sarnak's [*Super-Golden-Gates for PU(2)*](https://doi.org/10.1016/j.aim.2017.06.022), published in *Advances in Mathematics* in 2018.

Released under the [MIT License](LICENSE).

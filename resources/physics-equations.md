---
layout: page
title: "Physics 2130 Equation Sheet"
permalink: /resources/physics-equations/
mathjax: true
---

<!-- MathJax for LaTeX support on this page -->
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async
  src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js">
</script>

Below is a compact equation sheet for Physics 1 students.  
Each equation includes a quick guide to symbols.

---

## Constants

- \(G = 6.67\times 10^{-11}\, \mathrm{N\,m^2/kg^2}\)
- \(M_{\oplus} = 5.97\times 10^{24}\, \mathrm{kg}\)
- \(R_{\oplus} = 6.38\times 10^{6}\, \mathrm{m}\)
- \(g = 9.8\, \mathrm{N/kg} = 9.8\, \mathrm{m/s^2}\)
- \(k_B = 1.38\times 10^{-23}\, \mathrm{J/K}\)
- \(R = 8.31\, \mathrm{J/(mol\,K)}\)
- \(e = 1.602\times 10^{-19}\, \mathrm{C}\)
- \(k_c = 8.99\times 10^{9}\, \mathrm{N\,m^2/C^2}\)

---

## Vector / Trig Summary

Right triangle:
\[
\text{hyp}^2 = \text{opp}^2 + \text{adj}^2
\]

\[
\sin\theta = \frac{\text{opp}}{\text{hyp}},\quad
\cos\theta = \frac{\text{adj}}{\text{hyp}},\quad
\tan\theta = \frac{\text{opp}}{\text{adj}}
\]

**Symbols**
- \(\theta\): angle  
- hyp/opp/adj: hypotenuse / opposite side / adjacent side  

Vector components (2D):
\[
\vec A = A_x \hat{i} + A_y \hat{j},\qquad
A_x = A\cos\theta,\quad A_y = A\sin\theta
\]

**Symbols**
- \(\vec A\): vector  
- \(A\): magnitude  
- \(A_x, A_y\): components  
- \(\hat i,\hat j\): unit vectors  

---

## Unit 2 – Motion (Kinematics)

Position vector:
\[
\vec r = x\,\hat i + y\,\hat j
\]

**Symbols**
- \(\vec r\): position (m)  
- \(x,y\): coordinates (m)

Displacement:
\[
\Delta\vec r = \vec r_f - \vec r_i
\]

**Symbols**
- \(\Delta\vec r\): displacement (m)  
- \(\vec r_i,\vec r_f\): initial/final position  

Average velocity:
\[
\vec v_{\text{avg}} = \frac{\Delta\vec r}{\Delta t}
\]

**Symbols**
- \(\vec v_{\text{avg}}\): average velocity (m/s)  
- \(\Delta t\): time interval (s)

Average acceleration:
\[
\vec a_{\text{avg}} = \frac{\Delta\vec v}{\Delta t}
\]

**Symbols**
- \(\vec a_{\text{avg}}\): average acceleration (m/s\(^2\))

Constant-acceleration relations:
\[
v_f = v_i + a\Delta t
\]
\[
\Delta x = v_i\Delta t + \frac12 a(\Delta t)^2
\]
\[
v_f^2 = v_i^2 + 2a\Delta x
\]

**Symbols**
- \(v_i,v_f\): initial/final velocity (m/s)  
- \(a\): constant acceleration (m/s\(^2\))  
- \(\Delta x\): displacement (m)

---

## Unit 3 – Forces & Newton’s Laws

Net force:
\[
\vec F_{\text{net}}=\sum \vec F
\]

Newton’s 2nd law:
\[
\vec F_{\text{net}} = m\vec a
\]

Weight:
\[
W = mg
\]

Hooke’s law:
\[
F_s = k\Delta x
\]

Friction:
\[
f_s\le \mu_s N,\qquad f_k=\mu_k N
\]

Impulse:
\[
\vec I = \vec F\,\Delta t = m\Delta\vec v
\]

**Symbols**
- \(m\): mass (kg)  
- \(N\): normal force (N)  
- \(k\): spring constant (N/m)  
- \(\mu_s,\mu_k\): friction coefficients  

---

## Unit 4 – Fluids

Density:
\[
\rho = \frac{m}{V}
\]

Pressure:
\[
P = \frac{F}{A}
\]

Hydrostatic pressure:
\[
P = P_0 + \rho g d
\]

Buoyant force:
\[
F_B = \rho_f V_f g
\]

Continuity:
\[
Q = Av = \text{constant}
\]

Poiseuille’s law:
\[
Q = \frac{\pi R^4}{8\mu L}\Delta P
\]

Bernoulli:
\[
P+\frac12\rho v^2+\rho g y = \text{constant}
\]

**Symbols**
- \(\rho\): density (kg/m\(^3\))  
- \(\mu\): viscosity (Pa·s)  
- \(Q\): flow rate (m\(^3\)/s)

---

## Unit 5 – Energy

Work:
\[
W=F_\parallel d
\]

Kinetic energy:
\[
K=\frac12 mv^2
\]

Gravitational potential:
\[
U_g=mgy
\]

Spring potential:
\[
U_s=\frac12 k(\Delta x)^2
\]

Conservation of energy:
\[
E_{\text{tot}} = K + U + E_{\text{th}} + \dots
\]

---

## Unit 6 – Thermodynamics

Temperature:
\[
T(K)=T(^{\circ}C)+273.15
\]

Heat:
\[
Q = mc\Delta T
\]

Ideal gas law:
\[
PV = Nk_BT = nRT
\]

First law:
\[
\Delta U = W + Q
\]

---

## Unit 7 – Electricity & Magnetism

### Coulomb’s law
\[
F_e = k_c\frac{|q_1q_2|}{r^2}
\]

**Symbols**
- \(F_e\): electric force (N)  
- \(k_c\): Coulomb constant  
- \(q_1,q_2\): charges (C)  
- \(r\): separation (m)

### Electric field
\[
E = k_c\frac{|q|}{r^2}
\]
\[
\vec F = q\vec E
\]

**Symbols**
- \(E\): electric field (N/C)  
- \(q\): charge (C)

### Electric potential & energy
\[
V = k_c\frac{q}{r}
\]
\[
U_e = k_c\frac{q_1q_2}{r}
\]
\[
\Delta U = q\Delta V
\]

### Capacitance
\[
C=\frac{Q}{V}
\]
\[
C=\varepsilon_0\frac{A}{d}
\]
\[
U=\frac12 CV^2
\]

### Current & Ohm’s law
\[
I=\frac{\Delta Q}{\Delta t}
\]
\[
V=IR
\]
\[
P=IV=I^2R=\frac{V^2}{R}
\]

Series/parallel:
\[
R_{\text{eq}} = R_1+R_2+\cdots
\]
\[
\frac1{R_{\text{eq}}}=\frac1{R_1}+\frac1{R_2}+\cdots
\]

### Magnetic force
\[
F_B = qvB\sin\theta
\]
\[
F = ILB\sin\theta
\]

### Magnetic field from currents
\[
B=\frac{\mu_0 I}{2\pi r}
\]
\[
B=\mu_0 nI
\]

### Magnetic flux & induction
\[
\Phi_B = BA\cos\theta
\]
\[
\varepsilon = -\frac{d\Phi_B}{dt}
\]

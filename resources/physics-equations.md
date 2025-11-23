---
layout: page
title: false
permalink: /resources/physics-equations/
mathjax: true
---

<!-- MathJax config: allow $...$ inline and $$...$$ display -->
<script>
  window.MathJax = {
    tex: {
      inlineMath: [['$', '$'], ['\\(', '\\)']],
      displayMath: [['$$','$$'], ['\\[','\\]']]
    }
  };
</script>

<!-- MathJax for LaTeX support on this page -->
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async
  src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js">
</script>

<!-- Colors: equations = neon magenta, symbols = green -->
<style>
/* All math glyphs (inline + display) */
mjx-container[jax="CHTML"] mjx-math {
  color: #ff4fd8;  /* neon magenta */
}

/* Symbol labels in the “Symbols” lists */
.sym-green {
  color: #7CFC00;   /* bright green */
  font-weight: 600;
}
</style>

# Physics Equations (PHY 2130 / 2140)

Below is a compact equation sheet for Physics 1 students.  
Each equation includes a quick guide to symbols.

---

## Constants

- $G = 6.67\times 10^{-11}\, \mathrm{N\,m^2/kg^2}$
- $M_{\oplus} = 5.97\times 10^{24}\, \mathrm{kg}$
- $R_{\oplus} = 6.38\times 10^{6}\, \mathrm{m}$
- $g = 9.8\, \mathrm{N/kg} = 9.8\, \mathrm{m/s^2}$
- $k_B = 1.38\times 10^{-23}\, \mathrm{J/K}$
- $R = 8.31\, \mathrm{J/(mol\,K)}$
- $e = 1.602\times 10^{-19}\, \mathrm{C}$
- $k_c = 8.99\times 10^{9}\, \mathrm{N\,m^2/C^2}$
- $\varepsilon_0 = 8.85\times 10^{-12}\, \mathrm{C^2/(N\,m^2)}$
- $\mu_0 = 4\pi\times 10^{-7}\, \mathrm{T\,m/A}$

---

## Vector / Trig Summary

Right triangle:
$$
\text{hyp}^2 = \text{opp}^2 + \text{adj}^2
$$

Trig:
$$
\sin\theta = \frac{\text{opp}}{\text{hyp}},\qquad
\cos\theta = \frac{\text{adj}}{\text{hyp}},\qquad
\tan\theta = \frac{\text{opp}}{\text{adj}}
$$

Vector components:
$$
\vec A = A_x \hat i + A_y \hat j
$$

$$
A_x = A\cos\theta,\qquad A_y = A\sin\theta
$$

**Symbols**

- <span class="sym-green">$\theta$</span>: angle  
- hyp/opp/adj: hypotenuse / opposite / adjacent  
- <span class="sym-green">$A$</span>: magnitude of vector  
- <span class="sym-green">$A_x, A_y$</span>: components  

---

## Unit 2 – Motion (Kinematics)

Position:
$$
\vec r = x\,\hat i + y\,\hat j
$$

Displacement:
$$
\Delta\vec r = \vec r_f - \vec r_i
$$

Average speed:
$$
v_{\text{avg}} = \frac{\text{distance}}{\Delta t}
$$

Average velocity:
$$
\vec v_{\text{avg}} = \frac{\Delta\vec r}{\Delta t}
$$

Average acceleration:
$$
\vec a_{\text{avg}} = \frac{\Delta\vec v}{\Delta t}
$$

Constant-acceleration relations:
$$
v_f = v_i + a t
$$

$$
\Delta x = v_i t + \frac12 a t^2
$$

$$
v_f^2 = v_i^2 + 2a\Delta x
$$

**Symbols**

- <span class="sym-green">$x,y$</span>: position coordinates (m)  
- <span class="sym-green">$v_i, v_f$</span>: initial/final velocity (m/s)  
- <span class="sym-green">$a$</span>: acceleration (m/s$^2$)  
- <span class="sym-green">$t, \Delta t$</span>: time (s)  
- <span class="sym-green">$\Delta x$</span>: displacement (m)  

---

## Unit 3 – Forces & Newton’s Laws

Net force:
$$
\vec F_{\text{net}}=\sum \vec F
$$

Newton’s 2nd law:
$$
\vec F_{\text{net}}=m\vec a
$$

Weight:
$$
W = mg
$$

Hooke’s law:
$$
F_s = k\Delta x
$$

Friction:
$$
f_s \le \mu_s N,\qquad f_k=\mu_k N
$$

Impulse:
$$
\vec I = \vec F\,\Delta t = m\Delta\vec v
$$

Momentum:
$$
\vec p = m\vec v
$$

Conservation:
$$
\vec p_{\text{before}} = \vec p_{\text{after}}
$$

**Symbols**

- <span class="sym-green">$m$</span>: mass (kg)  
- <span class="sym-green">$N$</span>: normal force (N)  
- <span class="sym-green">$k$</span>: spring constant (N/m)  
- <span class="sym-green">$\mu_s,\mu_k$</span>: static/kinetic friction coefficients  
- <span class="sym-green">$\vec I$</span>: impulse (N·s)  
- <span class="sym-green">$\vec p$</span>: momentum (kg·m/s)  

---

## Unit 4 – Solids & Fluids

Density:
$$
\rho = \frac{m}{V}
$$

Pressure:
$$
P = \frac{F}{A}
$$

Hydrostatic pressure:
$$
P = P_0 + \rho g d
$$

Buoyant force:
$$
F_B = \rho_f V_f g
$$

Surface tension pressure:
$$
\Delta P = \frac{2\gamma}{r}
$$

Continuity:
$$
Q = A v = \text{constant}
$$

Poiseuille’s law:
$$
Q = \frac{\pi R^4}{8\mu L}\Delta P
$$

Bernoulli:
$$
P + \frac12\rho v^2 + \rho g y = \text{constant}
$$

**Viscous drag (Stokes)**
$$
F_{\text{viscous}} = 6\pi \mu R v
$$

**Terminal velocity in viscous fluid**
$$
v_t = \frac{2R^2(\rho_s-\rho_f)g}{9\mu}
$$

**Reynolds number**
$$
\mathrm{Re} = \frac{\rho R v}{\mu}
$$

**Symbols**

- <span class="sym-green">$\rho$</span>: density (kg/m$^3$)  
- <span class="sym-green">$P$</span>: pressure (Pa)  
- <span class="sym-green">$P_0$</span>: surface pressure (Pa)  
- <span class="sym-green">$F_B$</span>: buoyant force (N)  
- <span class="sym-green">$Q$</span>: flow rate (m$^3$/s)  
- <span class="sym-green">$R$</span>: sphere / tube radius (m)  
- <span class="sym-green">$L$</span>: tube length (m)  
- <span class="sym-green">$\mu$</span>: viscosity (Pa·s)  
- <span class="sym-green">$v_t$</span>: terminal velocity (m/s)  

---

## Unit 5 – Energy & Work

Work:
$$
W = F_{\parallel} d
$$

Kinetic energy:
$$
K = \frac12 m v^2
$$

Gravitational potential energy:
$$
U_g = m g y
$$

Spring potential energy:
$$
U_s = \frac12 k(\Delta x)^2
$$

Total mechanical energy:
$$
E_{\text{tot}} = K + U + E_{\text{th}} + \dots
$$

Power:
$$
P = \frac{\Delta E}{\Delta t}
$$

**Symbols**

- <span class="sym-green">$W$</span>: work (J)  
- <span class="sym-green">$K$</span>: kinetic energy (J)  
- <span class="sym-green">$U_g, U_s$</span>: potential energies (J)  
- <span class="sym-green">$P$</span>: power (W)  

---

## Unit 6 – Thermodynamics

Temperature conversion:
$$
T(K) = T(^{\circ}C) + 273.15
$$

Heat:
$$
Q = m c \Delta T
$$

Ideal gas law:
$$
P V = N k_B T = n R T
$$

Average kinetic energy (ideal gas):
$$
K_{\text{avg}} = \frac32 k_B T
$$

RMS speed:
$$
v_{\text{rms}} = \sqrt{\frac{3k_B T}{m}}
$$

First law:
$$
\Delta U = W + Q
$$

**Symbols**

- <span class="sym-green">$Q$</span>: heat (J)  
- <span class="sym-green">$c$</span>: specific heat (J/kg·K)  
- <span class="sym-green">$n$</span>: moles  
- <span class="sym-green">$N$</span>: number of molecules  
- <span class="sym-green">$U$</span>: internal energy (J)  

---

# Unit 7 – Electricity & Magnetism

## Coulomb’s Law

$$
F_e = k_c\frac{|q_1 q_2|}{r^2}
$$

**Symbols**

- <span class="sym-green">$F_e$</span>: electric force (N)  
- <span class="sym-green">$k_c$</span>: Coulomb constant  
- <span class="sym-green">$q_1, q_2$</span>: charges (C)  
- <span class="sym-green">$r$</span>: separation (m)  

---

## Electric Field

$$
E = k_c\frac{|q|}{r^2}
$$

$$
\vec F = q \vec E
$$

**Symbols**

- <span class="sym-green">$E$</span>: electric field (N/C or V/m)  
- <span class="sym-green">$q$</span>: charge (C)  
- <span class="sym-green">$\vec F$</span>: force (N)  

---

## Electric Potential & Energy

$$
V = k_c\frac{q}{r}
$$

$$
U_e = k_c\frac{q_1 q_2}{r}
$$

$$
\Delta U = q\,\Delta V
$$

**Symbols**

- <span class="sym-green">$V$</span>: electric potential (V)  
- <span class="sym-green">$U_e$</span>: electric potential energy (J)  
- <span class="sym-green">$\Delta V$</span>: potential difference (V)  

---

## Capacitance

$$
C = \frac{Q}{V}
$$

$$
C = \varepsilon_0\frac{A}{d}
$$

$$
U = \frac12 C V^2 = \frac12 QV = \frac{Q^2}{2C}
$$

**Symbols**

- <span class="sym-green">$C$</span>: capacitance (F)  
- <span class="sym-green">$Q$</span>: charge (C)  
- <span class="sym-green">$V$</span>: voltage (V)  
- <span class="sym-green">$A$</span>: plate area (m$^2$)  
- <span class="sym-green">$d$</span>: separation (m)  

---

## Current & Ohm’s Law

$$
I = \frac{\Delta Q}{\Delta t}
$$

$$
V = IR
$$

Power:
$$
P = IV = I^2 R = \frac{V^2}{R}
$$

Resistors in series:
$$
R_{\text{eq}} = R_1 + R_2 + \cdots
$$

Resistors in parallel:
$$
\frac{1}{R_{\text{eq}}} = \frac{1}{R_1} + \frac{1}{R_2} + \cdots
$$

**Symbols**

- <span class="sym-green">$I$</span>: current (A)  
- <span class="sym-green">$R$</span>: resistance (Ω)  
- <span class="sym-green">$P$</span>: power (W)  

---

## Magnetic Force

Moving charge:
$$
F_B = q v B \sin\theta
$$

Current-carrying wire:
$$
F = I L B \sin\theta
$$

**Symbols**

- <span class="sym-green">$B$</span>: magnetic field (T)  
- <span class="sym-green">$L$</span>: length of wire (m)  
- <span class="sym-green">$\theta$</span>: angle between current/velocity and $B$  

---

## Magnetic Field from Currents

Long straight wire:
$$
B = \frac{\mu_0 I}{2\pi r}
$$

Solenoid:
$$
B = \mu_0 n I
$$

**Symbols**

- <span class="sym-green">$n$</span>: turns per unit length  
- <span class="sym-green">$r$</span>: distance from wire (m)  

---

## Magnetic Flux & Induction

$$
\Phi_B = B A \cos\theta
$$

Faraday’s Law:
$$
\varepsilon = -\frac{d\Phi_B}{dt}
$$

**Symbols**

- <span class="sym-green">$\Phi_B$</span>: magnetic flux (Wb)  
- <span class="sym-green">$\varepsilon$</span>: induced emf (V)  
- <span class="sym-green">$A$</span>: area of loop (m$^2$)  

---

# Diffusion & Brownian Motion

Mean-square displacement:

$$
x_{\text{rms}}^2 = 2Dt \quad (1\text{D})
$$
$$
r_{\text{rms}}^2 = 4Dt \quad (2\text{D})
$$
$$
r_{\text{rms}}^2 = 6Dt \quad (3\text{D})
$$

Gaussian distribution:

$$
P(x,t)=\frac{1}{\sqrt{4\pi Dt}}
\exp\!\left(-\frac{x^2}{4Dt}\right)
$$

Fick’s first law:

$$
J = -D\frac{\Delta n}{\Delta x}
$$

Stokes–Einstein relation:

$$
D = \frac{k_B T}{6\pi \mu r}
$$

**Symbols**

- <span class="sym-green">$D$</span>: diffusion constant (m$^2$/s)  
- <span class="sym-green">$t$</span>: time (s)  
- <span class="sym-green">$r_{\text{rms}}$</span>: rms displacement (m)  
- <span class="sym-green">$J$</span>: diffusion flux  
- <span class="sym-green">$n$</span>: concentration  
- <span class="sym-green">$r$</span>: particle radius (m)  
- <span class="sym-green">$T$</span>: temperature (K)  

---
layout: page
title: false
permalink: /resources/physics-equations/
mathjax: false
---

<!-- MathJax config: allow $...$ inline and $$...$$ display -->
<script>
  window.MathJax = {
    tex: {
      inlineMath: [['$', '$'], ['\\(', '\\)']],
      displayMath: [['$$','$$'], ['\\[','\\]']],
      processEscapes: true
    },
    options: {
      skipHtmlTags: ['script','noscript','style','textarea','pre','code']
    }
  };
</script>

<!-- MathJax v3 (NO async; order matters) -->
<script defer src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>

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

**Symbols**
- $\theta$: angle  
- hyp/opp/adj: hypotenuse / opposite / adjacent  

Vector components:
$$
\vec A = A_x \hat i + A_y \hat j
$$

$$
A_x = A\cos\theta,\qquad A_y = A\sin\theta
$$

**Symbols**
- $\vec A$: vector  
- $A$: magnitude  
- $A_x, A_y$: components  
- $\hat i,\hat j$: unit vectors  

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
- $x,y$: position coordinates (m)  
- $\vec r_i,\vec r_f$: initial/final position  
- $v_i,v_f$: initial/final velocity (m/s)  
- $a$: acceleration (m/s$^2$)  
- $t,\Delta t$: time (s)  
- $\Delta x$: displacement (m)

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

**Symbols**
- $m$: mass (kg)  
- $N$: normal force (N)  
- $k$: spring constant (N/m)  
- $\mu_s,\mu_k$: static/kinetic friction coefficients  
- $\vec I$: impulse (N·s)

---

## Unit 4 – Solids & Fluids

Density:
$$
\rho = \frac{m}{V}
$$

Pressure:
$$
P=\frac{F}{A}
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
Q = Av = \text{constant}
$$

Poiseuille’s law:
$$
Q = \frac{\pi R^4}{8\mu L}\Delta P
$$

Bernoulli:
$$
P+\frac12\rho v^2+\rho g y = \text{constant}
$$

**Symbols**
- $\rho$: density (kg/m$^3$)  
- $P$: pressure (Pa)  
- $P_0$: surface pressure  
- $d$: depth (m)  
- $F_B$: buoyant force (N)  
- $\rho_f$: fluid density  
- $V_f$: displaced volume  
- $\gamma$: surface tension  
- $Q$: flow rate (m$^3$/s)  
- $R$: tube radius, $L$: tube length  
- $\mu$: viscosity  

---

## Unit 5 – Energy & Work

Work:
$$
W = F_{\parallel} d
$$

Kinetic energy:
$$
K = \frac12 mv^2
$$

Gravitational potential energy:
$$
U_g = mgy
$$

Spring potential energy:
$$
U_s=\frac12 k(\Delta x)^2
$$

Total mechanical energy:
$$
E_{\text{tot}} = K + U + E_{\text{th}} + \dots
$$

Power:
$$
P=\frac{\Delta E}{\Delta t}
$$

**Symbols**
- $W$: work (J)  
- $K$: kinetic energy (J)  
- $U_g,U_s$: potential energies (J)  
- $P$: power (W)

---

## Unit 6 – Thermodynamics

Temperature conversion:
$$
T(K)=T(^{\circ}C)+273.15
$$

Heat:
$$
Q=mc\Delta T
$$

Ideal gas law:
$$
PV = Nk_BT = nRT
$$

Average kinetic energy (ideal gas):
$$
K_{\text{avg}}=\frac32 k_B T
$$

RMS speed:
$$
v_{\text{rms}}=\sqrt{\frac{3k_BT}{m}}
$$

First law:
$$
\Delta U = W + Q
$$

**Symbols**
- $Q$: heat (J)  
- $c$: specific heat (J/kg·K)  
- $n$: moles  
- $N$: number of molecules  
- $U$: internal energy (J)

---

# Unit 7 – Electricity & Magnetism

## Coulomb’s Law
$$
F_e = k_c\frac{|q_1 q_2|}{r^2}
$$

**Symbols**
- $F_e$: electric force (N)  
- $k_c$: Coulomb constant  
- $q_1,q_2$: charges (C)  
- $r$: separation (m)

---

## Electric Field
$$
E = k_c\frac{|q|}{r^2}
$$

$$
\vec F = q\vec E
$$

**Symbols**
- $E$: electric field (N/C or V/m)  
- $q$: charge (C)  
- $\vec F$: force on charge (N)

---

## Electric Potential & Energy
$$
V = k_c\frac{q}{r}
$$

$$
U_e = k_c\frac{q_1 q_2}{r}
$$

$$
\Delta U = q\Delta V
$$

**Symbols**
- $V$: electric potential (V)  
- $U_e$: electric potential energy (J)  
- $\Delta V$: potential difference

---

## Capacitance
$$
C=\frac{Q}{V}
$$

$$
C=\varepsilon_0\frac{A}{d}
$$

$$
U=\frac12 CV^2=\frac12 QV=\frac{Q^2}{2C}
$$

**Symbols**
- $C$: capacitance (F)  
- $Q$: charge stored (C)  
- $V$: voltage (V)  
- $\varepsilon_0$: permittivity of free space  
- $A$: plate area (m$^2$)  
- $d$: separation (m)  
- $U$: stored energy (J)

---

## Current & Ohm’s Law
$$
I=\frac{\Delta Q}{\Delta t}
$$

$$
V = IR
$$

Power:
$$
P = IV = I^2R = \frac{V^2}{R}
$$

Resistors in series:
$$
R_{\text{eq}}=R_1+R_2+\cdots
$$

Resistors in parallel:
$$
\frac1{R_{\text{eq}}}=\frac1{R_1}+\frac1{R_2}+\cdots
$$

**Symbols**
- $I$: current (A)  
- $R$: resistance (Ω)  
- $P$: power (W)

---

## Magnetic Force

Moving charge:
$$
F_B=qvB\sin\theta
$$

Current-carrying wire:
$$
F=ILB\sin\theta
$$

**Symbols**
- $B$: magnetic field (T)  
- $\theta$: angle between motion/current and $B$

---

## Magnetic Field from Currents

Long straight wire:
$$
B=\frac{\mu_0 I}{2\pi r}
$$

Solenoid:
$$
B=\mu_0 nI
$$

**Symbols**
- $\mu_0$: permeability of free space  
- $n$: turns per unit length  
- $r$: distance from wire

---

## Magnetic Flux & Induction
$$
\Phi_B = BA\cos\theta
$$

Faraday’s Law:
$$
\varepsilon = -\frac{d\Phi_B}{dt}
$$

**Symbols**
- $\Phi_B$: magnetic flux (Wb)  
- $\varepsilon$: induced emf (V)  
- $A$: area of loop (m$^2$)

---

## (New) Capacitors in Series/Parallel

Series:
$$
\frac{1}{C_{\text{eq}}}=\frac{1}{C_1}+\frac{1}{C_2}+\cdots
$$

Parallel:
$$
C_{\text{eq}}=C_1+C_2+\cdots
$$

**Symbols**
- $C_{\text{eq}}$: equivalent capacitance (F)

---

## (New) Lorentz Force (vector form)

$$
\vec F = q\vec E + q\,\vec v\times \vec B
$$

**Symbols**
- $\vec v$: velocity of charge (m/s)  
- $\times$: cross product  

---

# Unit 8 – Diffusion, Brownian Motion & Terminal Velocity (Labs)

## Brownian Motion / Diffusion

Mean-square displacement:

1D:
$$
x_{\text{rms}}^2 = 2Dt
$$

2D:
$$
r_{\text{rms}}^2 = 4Dt
$$

3D:
$$
r_{\text{rms}}^2 = 6Dt
$$

Diffusion flux (Fick’s law):
$$
J = -D\frac{\Delta n}{\Delta x}
$$

Stokes-Einstein relation:
$$
D = \frac{k_B T}{6\pi\mu r}
$$

**Symbols**
- $D$: diffusion constant (m$^2$/s)  
- $t$: time (s)  
- $J$: diffusion flux  
- $n$: concentration  
- $\mu$: viscosity (Pa·s)  
- $r$: particle radius (m)  
- $T$: temperature (K)

---

## Viscous Drag (Stokes’ Law)

Force on a small sphere moving in a viscous fluid:
$$
F_{\text{viscous}} = 6\pi\mu r v
$$

**Symbols**
- $F_{\text{viscous}}$: drag force (N)  
- $v$: speed (m/s)

---

## Terminal Velocity (falling sphere)

When drag balances effective weight:

$$
v_t = \frac{2r^2(\rho_s-\rho_f)g}{9\mu}
$$

**Symbols**
- $v_t$: terminal velocity (m/s)  
- $\rho_s$: sphere density (kg/m$^3$)  
- $\rho_f$: fluid density (kg/m$^3$)

---

## Vesicle Transport (motor proteins)

Velocity-ATP relation:
$$
v = R\,s
$$

**Symbols**
- $v$: vesicle speed (m/s)  
- $R$: ATP hydrolysis rate (cycles/s)  
- $s$: motor step size (m)  
  - kinesin: $s \approx 8\,\mathrm{nm}$  
  - myosin V: $s \approx 36\,\mathrm{nm}$  

---

## Useful pixel → SI conversions (ImageJ labs)

If your tracking gives values in micrometers:

$$
1\ \mu\text{m} = 10^{-6}\ \text{m}
$$

If tracking gives pixels and your calibration is:

$$
1\ \text{pixel} \approx 0.193\ \mu\text{m}
$$

then

$$
v(\text{m/s}) = v(\text{pixels/s})\times 0.193\times 10^{-6}
$$

and

$$
r(\text{m}) = r(\text{pixels})\times 0.193\times 10^{-6}
$$



<p style="margin-bottom: 1rem;">
  <a href="{{ '/doc/PHY_2131LabNotes.pdf' | relative_url }}" target="_blank">
    Open PDF in new tab
  </a>
</p>

<div style="width: 100%; height: 90vh;">
  <iframe
    src="{{ '/doc/PHY_2131LabNotes.pdf' | relative_url }}"
    width="100%"
    height="100%"
    style="border: 1px solid #ccc; border-radius: 8px;">
  </iframe>
</div>

---
layout: page
title: false
permalink: /resources/physics-equations/
mathjax: true
---

<!-- MathJax config: allow $...$ inline and $$...$$ display
     + color macros for equations and symbols -->
<script>
  window.MathJax = {
    tex: {
      inlineMath: [['$', '$'], ['\\(', '\\)']],
      displayMath: [['$$','$$'], ['\\[','\\]']],
      macros: {
        eq: ["{\\color{#ff4fd8}{#1}}", 1],   // neon magenta
        sym: ["{\\color{#7CFC00}{#1}}", 1]  // neon green
      }
    }
  };
</script>

<!-- MathJax for LaTeX support on this page -->
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async
  src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js">
</script>

# Physics Equations (PHY 2130 / 2140)

Below is a compact equation sheet for Physics 1 students.  
Each equation includes a quick guide to symbols.

---

## Constants

- $\eq{\sym{G} = 6.67\times 10^{-11}\, \mathrm{N\,m^2/kg^2}}$
- $\eq{\sym{M}_{\oplus} = 5.97\times 10^{24}\, \mathrm{kg}}$
- $\eq{\sym{R}_{\oplus} = 6.38\times 10^{6}\, \mathrm{m}}$
- $\eq{\sym{g} = 9.8\, \mathrm{N/kg} = 9.8\, \mathrm{m/s^2}}$
- $\eq{\sym{k}_B = 1.38\times 10^{-23}\, \mathrm{J/K}}$
- $\eq{\sym{R} = 8.31\, \mathrm{J/(mol\,K)}}$
- $\eq{\sym{e} = 1.602\times 10^{-19}\, \mathrm{C}}$
- $\eq{\sym{k}_c = 8.99\times 10^{9}\, \mathrm{N\,m^2/C^2}}$
- $\eq{\sym{\varepsilon}_0 = 8.85\times 10^{-12}\, \mathrm{C^2/(N\,m^2)}}$
- $\eq{\sym{\mu}_0 = 4\pi\times 10^{-7}\, \mathrm{T\,m/A}}$

---

## Vector / Trig Summary

Right triangle:
$$
\eq{\text{hyp}^2 = \text{opp}^2 + \text{adj}^2}
$$

Trig:
$$
\eq{\sin\sym{\theta} = \frac{\text{opp}}{\text{hyp}},\qquad
\cos\sym{\theta} = \frac{\text{adj}}{\text{hyp}},\qquad
\tan\sym{\theta} = \frac{\text{opp}}{\text{adj}}}
$$

**Symbols**
- $\sym{\theta}$: angle  
- hyp/opp/adj: hypotenuse / opposite / adjacent  

Vector components:
$$
\eq{\vec{\sym{A}} = \sym{A}_x \hat i + \sym{A}_y \hat j}
$$

$$
\eq{\sym{A}_x = \sym{A}\cos\sym{\theta},\qquad \sym{A}_y = \sym{A}\sin\sym{\theta}}
$$

**Symbols**
- $\vec{\sym{A}}$: vector  
- $\sym{A}$: magnitude  
- $\sym{A}_x, \sym{A}_y$: components  
- $\hat i,\hat j$: unit vectors  

---

## Unit 2 – Motion (Kinematics)

Position:
$$
\eq{\vec{\sym{r}} = \sym{x}\,\hat i + \sym{y}\,\hat j}
$$

Displacement:
$$
\eq{\Delta\vec{\sym{r}} = \vec{\sym{r}}_f - \vec{\sym{r}}_i}
$$

Average speed:
$$
\eq{\sym{v}_{\text{avg}} = \frac{\text{distance}}{\Delta \sym{t}}}
$$

Average velocity:
$$
\eq{\vec{\sym{v}}_{\text{avg}} = \frac{\Delta\vec{\sym{r}}}{\Delta \sym{t}}}
$$

Average acceleration:
$$
\eq{\vec{\sym{a}}_{\text{avg}} = \frac{\Delta\vec{\sym{v}}}{\Delta \sym{t}}}
$$

Constant-acceleration relations:
$$
\eq{\sym{v}_f = \sym{v}_i + \sym{a}\sym{t}}
$$

$$
\eq{\Delta \sym{x} = \sym{v}_i\sym{t} + \frac12 \sym{a}\sym{t}^2}
$$

$$
\eq{\sym{v}_f^2 = \sym{v}_i^2 + 2\sym{a}\Delta \sym{x}}
$$

**Symbols**
- $\sym{x},\sym{y}$: position coordinates (m)  
- $\vec{\sym{r}}_i,\vec{\sym{r}}_f$: initial/final position  
- $\sym{v}_i,\sym{v}_f$: initial/final velocity (m/s)  
- $\sym{a}$: acceleration (m/s$^2$)  
- $\sym{t},\Delta \sym{t}$: time (s)  
- $\Delta \sym{x}$: displacement (m)

---

## Unit 3 – Forces & Newton’s Laws

Net force:
$$
\eq{\vec{\sym{F}}_{\text{net}}=\sum \vec{\sym{F}}}
$$

Newton’s 2nd law:
$$
\eq{\vec{\sym{F}}_{\text{net}}=\sym{m}\vec{\sym{a}}}
$$

Weight:
$$
\eq{\sym{W} = \sym{m}\sym{g}}
$$

Hooke’s law:
$$
\eq{\sym{F}_s = \sym{k}\Delta \sym{x}}
$$

Friction:
$$
\eq{\sym{f}_s \le \sym{\mu}_s \sym{N},\qquad \sym{f}_k=\sym{\mu}_k \sym{N}}
$$

Impulse:
$$
\eq{\vec{\sym{I}} = \vec{\sym{F}}\,\Delta \sym{t} = \sym{m}\Delta\vec{\sym{v}}}
$$

Momentum (added):
$$
\eq{\vec{\sym{p}} = \sym{m}\vec{\sym{v}}}
$$

Conservation of momentum:
$$
\eq{\vec{\sym{p}}_{\text{before}}=\vec{\sym{p}}_{\text{after}}}
$$

**Symbols**
- $\sym{m}$: mass (kg)  
- $\sym{N}$: normal force (N)  
- $\sym{k}$: spring constant (N/m)  
- $\sym{\mu}_s,\sym{\mu}_k$: static/kinetic friction coefficients  
- $\vec{\sym{I}}$: impulse (N·s)  
- $\vec{\sym{p}}$: momentum (kg·m/s)

---

## Unit 4 – Solids & Fluids

Density:
$$
\eq{\sym{\rho} = \frac{\sym{m}}{\sym{V}}}
$$

Pressure:
$$
\eq{\sym{P}=\frac{\sym{F}}{\sym{A}}}
$$

Hydrostatic pressure:
$$
\eq{\sym{P} = \sym{P}_0 + \sym{\rho}\sym{g}\sym{d}}
$$

Buoyant force:
$$
\eq{\sym{F}_B = \sym{\rho}_f \sym{V}_f \sym{g}}
$$

Surface tension pressure:
$$
\eq{\Delta \sym{P} = \frac{2\sym{\gamma}}{\sym{r}}}
$$

Continuity:
$$
\eq{\sym{Q} = \sym{A}\sym{v} = \text{constant}}
$$

Poiseuille’s law:
$$
\eq{\sym{Q} = \frac{\pi \sym{R}^4}{8\sym{\mu}\sym{L}}\Delta \sym{P}}
$$

Bernoulli:
$$
\eq{\sym{P}+\frac12\sym{\rho}\sym{v}^2+\sym{\rho}\sym{g}\sym{y} = \text{constant}}
$$

**NEW: Viscous drag (Stokes)**
$$
\eq{\sym{F}_{\text{viscous}} = 6\pi \sym{\mu}\sym{R}\sym{v}}
$$

**NEW: Terminal velocity in viscous fluid**
$$
\eq{\sym{v}_t = \frac{2\sym{R}^2(\sym{\rho}_s-\sym{\rho}_f)\sym{g}}{9\sym{\mu}}}
$$

**NEW: Reynolds number**
$$
\eq{\mathrm{Re}=\frac{\sym{\rho}\,\sym{R}\,\sym{v}}{\sym{\mu}}}
$$

**Symbols**
- $\sym{\rho}$: density (kg/m$^3$)  
- $\sym{P}$: pressure (Pa)  
- $\sym{P}_0$: surface pressure  
- $\sym{d}$: depth (m)  
- $\sym{F}_B$: buoyant force (N)  
- $\sym{\rho}_f$: fluid density  
- $\sym{V}_f$: displaced volume  
- $\sym{\gamma}$: surface tension  
- $\sym{Q}$: flow rate (m$^3$/s)  
- $\sym{R}$: sphere/tube radius  
- $\sym{L}$: tube length  
- $\sym{\mu}$: viscosity (Pa·s)  
- $\sym{v}_t$: terminal velocity  
- $\sym{\rho}_s$: sphere density  

---

## Unit 5 – Energy & Work

Work:
$$
\eq{\sym{W} = \sym{F}_{\parallel} \sym{d}}
$$

Kinetic energy:
$$
\eq{\sym{K} = \frac12 \sym{m}\sym{v}^2}
$$

Gravitational potential energy:
$$
\eq{\sym{U}_g = \sym{m}\sym{g}\sym{y}}
$$

Spring potential energy:
$$
\eq{\sym{U}_s=\frac12 \sym{k}(\Delta \sym{x})^2}
$$

Total mechanical energy:
$$
\eq{\sym{E}_{\text{tot}} = \sym{K} + \sym{U} + \sym{E}_{\text{th}} + \dots}
$$

Power:
$$
\eq{\sym{P}=\frac{\Delta \sym{E}}{\Delta \sym{t}}}
$$

**Symbols**
- $\sym{W}$: work (J)  
- $\sym{K}$: kinetic energy (J)  
- $\sym{U}_g,\sym{U}_s$: potential energies (J)  
- $\sym{P}$: power (W)

---

## Unit 6 – Thermodynamics

Temperature conversion:
$$
\eq{\sym{T}(\mathrm{K})=\sym{T}(^{\circ}\mathrm{C})+273.15}
$$

Heat:
$$
\eq{\sym{Q}=\sym{m}\sym{c}\Delta \sym{T}}
$$

Ideal gas law:
$$
\eq{\sym{P}\sym{V} = \sym{N}\sym{k}_B\sym{T} = \sym{n}\sym{R}\sym{T}}
$$

Average kinetic energy (ideal gas):
$$
\eq{\sym{K}_{\text{avg}}=\frac32 \sym{k}_B \sym{T}}
$$

RMS speed:
$$
\eq{\sym{v}_{\text{rms}}=\sqrt{\frac{3\sym{k}_B\sym{T}}{\sym{m}}}}
$$

First law:
$$
\eq{\Delta \sym{U} = \sym{W} + \sym{Q}}
$$

**Symbols**
- $\sym{Q}$: heat (J)  
- $\sym{c}$: specific heat (J/kg·K)  
- $\sym{n}$: moles  
- $\sym{N}$: number of molecules  
- $\sym{U}$: internal energy (J)

---

# Unit 7 – Electricity & Magnetism

## Coulomb’s Law
$$
\eq{\sym{F}_e = \sym{k}_c\frac{|\sym{q}_1 \sym{q}_2|}{\sym{r}^2}}
$$

**Symbols**
- $\sym{F}_e$: electric force (N)  
- $\sym{k}_c$: Coulomb constant  
- $\sym{q}_1,\sym{q}_2$: charges (C)  
- $\sym{r}$: separation (m)

---

## Electric Field
$$
\eq{\sym{E} = \sym{k}_c\frac{|\sym{q}|}{\sym{r}^2}}
$$

$$
\eq{\vec{\sym{F}} = \sym{q}\vec{\sym{E}}}
$$

**Symbols**
- $\sym{E}$: electric field (N/C or V/m)  
- $\sym{q}$: charge (C)  
- $\vec{\sym{F}}$: force on charge (N)

---

## Electric Potential & Energy
$$
\eq{\sym{V} = \sym{k}_c\frac{\sym{q}}{\sym{r}}}
$$

$$
\eq{\sym{U}_e = \sym{k}_c\frac{\sym{q}_1 \sym{q}_2}{\sym{r}}}
$$

$$
\eq{\Delta \sym{U} = \sym{q}\Delta \sym{V}}
$$

**Symbols**
- $\sym{V}$: electric potential (V)  
- $\sym{U}_e$: electric potential energy (J)  
- $\Delta \sym{V}$: potential difference

---

## Capacitance
$$
\eq{\sym{C}=\frac{\sym{Q}}{\sym{V}}}
$$

$$
\eq{\sym{C}=\sym{\varepsilon}_0\frac{\sym{A}}{\sym{d}}}
$$

$$
\eq{\sym{U}=\frac12 \sym{C}\sym{V}^2=\frac12 \sym{Q}\sym{V}=\frac{\sym{Q}^2}{2\sym{C}}}
$$

**Symbols**
- $\sym{C}$: capacitance (F)  
- $\sym{Q}$: charge stored (C)  
- $\sym{V}$: voltage (V)  
- $\sym{\varepsilon}_0$: permittivity of free space  
- $\sym{A}$: plate area (m$^2$)  
- $\sym{d}$: separation (m)  
- $\sym{U}$: stored energy (J)

---

## Current & Ohm’s Law
$$
\eq{\sym{I}=\frac{\Delta \sym{Q}}{\Delta \sym{t}}}
$$

$$
\eq{\sym{V} = \sym{I}\sym{R}}
$$

Power:
$$
\eq{\sym{P} = \sym{I}\sym{V} = \sym{I}^2\sym{R} = \frac{\sym{V}^2}{\sym{R}}}
$$

Resistors in series:
$$
\eq{\sym{R}_{\text{eq}}=\sym{R}_1+\sym{R}_2+\cdots}
$$

Resistors in parallel:
$$
\eq{\frac1{\sym{R}_{\text{eq}}}=\frac1{\sym{R}_1}+\frac1{\sym{R}_2}+\cdots}
$$

**Symbols**
- $\sym{I}$: current (A)  
- $\sym{R}$: resistance (Ω)  
- $\sym{P}$: power (W)

---

## Magnetic Force

Moving charge:
$$
\eq{\sym{F}_B=\sym{q}\sym{v}\sym{B}\sin\sym{\theta}}
$$

Current-carrying wire:
$$
\eq{\sym{F}=\sym{I}\sym{L}\sym{B}\sin\sym{\theta}}
$$

**Symbols**
- $\sym{B}$: magnetic field (T)  
- $\sym{\theta}$: angle between motion/current and $B$

---

## Magnetic Field from Currents

Long straight wire:
$$
\eq{\sym{B}=\frac{\sym{\mu}_0 \sym{I}}{2\pi \sym{r}}}
$$

Solenoid:
$$
\eq{\sym{B}=\sym{\mu}_0 \sym{n}\sym{I}}
$$

**Symbols**
- $\sym{\mu}_0$: permeability of free space  
- $\sym{n}$: turns per unit length  
- $\sym{r}$: distance from wire

---

## Magnetic Flux & Induction
$$
\eq{\sym{\Phi}_B = \sym{B}\sym{A}\cos\sym{\theta}}
$$

Faraday’s Law:
$$
\eq{\sym{\varepsilon} = -\frac{d\sym{\Phi}_B}{d\sym{t}}}
$$

**Symbols**
- $\sym{\Phi}_B$: magnetic flux (Wb)  
- $\sym{\varepsilon}$: induced emf (V)  
- $\sym{A}$: area of loop (m$^2$)

---

# Diffusion & Brownian Motion (NEW)

Mean-square displacement:

$$
\eq{\sym{x}_{\text{rms}}^2 = 2\sym{D}\sym{t}\quad (1\text{D})}
$$

$$
\eq{\sym{r}_{\text{rms}}^2 = 4\sym{D}\sym{t}\quad (2\text{D})}
$$

$$
\eq{\sym{r}_{\text{rms}}^2 = 6\sym{D}\sym{t}\quad (3\text{D})}
$$

Gaussian distribution:

$$
\eq{\sym{P}(\sym{x},\sym{t})=
\frac{1}{\sqrt{4\pi \sym{D}\sym{t}}}
\exp\!\left(-\frac{\sym{x}^2}{4\sym{D}\sym{t}}\right)}
$$

Fick’s first law:

$$
\eq{\sym{J} = -\sym{D}\frac{\Delta \sym{n}}{\Delta \sym{x}}}
$$

Stokes–Einstein relation:

$$
\eq{\sym{D}=\frac{\sym{k}_B\sym{T}}{6\pi \sym{\mu}\sym{r}}}
$$

**Symbols**
- $\sym{D}$: diffusion constant (m$^2$/s)  
- $\sym{t}$: time (s)  
- $\sym{r}_{\text{rms}}$: rms displacement (m)  
- $\sym{P}(x,t)$: probability density  
- $\sym{J}$: diffusion flux  
- $\sym{n}$: concentration  
- $\sym{\mu}$: viscosity  
- $\sym{r}$: particle radius  
- $\sym{T}$: temperature (K)


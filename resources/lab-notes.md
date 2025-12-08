---
layout: page
title: Physics Lab Notes
permalink: /resources/lab-notes/
mathjax: true
---



# Physics Lab Notes

Below are short concept notes connected to Experiments 2–5  
(Directed motion, Random motion, Random + directed motion, and Vesicle transport).

---

## Experiment 2 – Directed motion (Terminal velocity)

In the coming weeks, your main lecture will cover terminal velocity and the role of resistive forces. To help you get a head start, here is a short introduction that outlines the basic concepts and includes a few equations showing how terminal velocity depends on various parameters.

This document is meant to give you a general idea. Your own predictions about parameter dependence may differ, and your experimental results might not match the theory exactly.

### Terminal velocity

When an object falls through a fluid (air, water, glycerin, etc.), several forces are at play. When you release the sphere, it falls toward the ground (toward the center of the Earth, to be more precise). This is due to the force of gravity, i.e., its weight. But since it is moving through a fluid (not a vacuum), it also experiences a resistive force that tries to slow the object down, much like friction.

So we have a downward gravitational force and upward resistive forces on the object. The resistive force depends on the velocity of the object, so it increases as the object accelerates. The downward gravitational force, however, remains the same. At some point, these forces balance out, making the net force zero, i.e., acceleration zero, which means the velocity becomes constant. This constant velocity is called the **terminal velocity**.

<div style="text-align:center; margin: 1.5rem 0;">
  <img src="{{ '/assets/img/labnotes/velocity_vs_time_terminal.png' | relative_url }}"
       alt="Velocity vs time for object reaching terminal velocity"
       style="max-width: 450px; width: 100%; border-radius: 8px;">
</div>

### Forces on a falling sphere

For a sphere of radius $r$, density $\rho_s$, and mass $m$ falling through a fluid of density $\rho_f$ and viscosity $\eta$:

1. **Weight (downward)**  

   $$
   F_g = mg = \rho_s V g
   $$

   where $V = \tfrac{4}{3}\pi r^3$ is the volume of the sphere.

2. **Buoyant force (upward, Archimedes’ principle)**  

   $$
   F_b = \rho_f V g
   $$

3. **Velocity-dependent resistive forces (drag forces, upward)**  

   At low speeds and for small spheres, viscosity dominates and Stokes’ law applies:

   $$
   F_v = 6\pi \eta r v
   $$

   At higher speeds / turbulent flow, drag depends on velocity squared:

   $$
   F_d = \tfrac{1}{2} C_d \rho_f A v^2
   $$

   where $A = \pi r^2$ is the cross-sectional area of the sphere and $C_d$ is the drag coefficient.

For the current experiment, we can neglect the turbulent contribution and only consider the viscous force.

<div style="text-align:center; margin: 1.5rem 0;">
  <img src="{{ '/assets/img/labnotes/graded_cylinder_forces.png' | relative_url }}"
       alt="Forces on a falling sphere in a fluid"
       style="max-width: 350px; width: 100%; border-radius: 8px;">
</div>

### Condition for terminal velocity

At terminal velocity $v_t$, the net force is zero:

$$
\text{Total downward force} = \text{Total upward force}
$$

$$
F_g = F_b + F_v
$$

Substituting:

$$
\rho_s V g = \rho_f V g + 6\pi \eta r v_t
$$

Solving for $v_t$:

$$
v_t = \frac{(\rho_s - \rho_f) V g}{6\pi r \eta}
= \frac{2 r^2 g (\rho_s - \rho_f)}{9 \eta}
$$

> **Terminal velocity**
>
> $$
> v_t = \frac{2 r^2 g (\rho_s - \rho_f)}{9 \eta}
> $$
>
> where  
> $r$ – radius of the sphere  
> $g$ – acceleration due to gravity ($9.8\ \text{m/s}^2$)  
> $\rho_s$ – density of the sphere  
> $\rho_f$ – density of the fluid  
> $\eta$ – coefficient of viscosity

Our experiment investigates the dependence of $v_t$ on

- the size of the sphere, $r$
- the density of the sphere, $\rho_s$
- the viscosity of the fluid, $\eta$

Qualitative predictions:

1. $v_t$ vs radius $r$ – parabolic ($v_t \propto r^2$)  
2. $v_t$ vs density $\rho_s$ – linear ($v_t \propto (\rho_s - \rho_f)$)  
3. $v_t$ vs viscosity $\eta$ – inverse ($v_t \propto 1/\eta$)

<div style="text-align:center; margin: 1.5rem 0 2rem;">
  <img src="{{ '/assets/img/labnotes/vt.jpg' | relative_url }}"
       alt="Example terminal velocity graphs"
       style="max-width: 700px; width: 100%; border-radius: 8px;">
</div>

---

## Experiment 3 – Random motion (Brownian motion & diffusion)

In this experiment, we look at motion on the microscopic scale, known as Brownian motion. This was one of the first clear pieces of evidence for the existence of molecules. Robert Brown noticed that pollen grains under a microscope seemed to “wiggle” around, which is due to water molecules constantly bumping into the pollen, making it move randomly.

In our class, we replicate this idea by observing tiny silica beads suspended in water under a microscope. We then study how the random motion (or diffusion) of these beads depends on two things: the radius of the bead and the viscosity of the liquid they are in.

### Root mean square (RMS) distance

Consider placing a drop of ink gently on the surface of water in a test tube (to minimize convection and other disturbances) and starting your clock. At time zero, the ink particles are all at the starting point. As time passes, they spread out. Eventually (after many hours), the entire column of water changes color, reaching a uniform concentration of ink particles throughout.

<div style="text-align:center; margin: 1.5rem 0;">
  <img src="{{ '/assets/img/labnotes/Diffusion.jpg' | relative_url }}"
       alt="Diffusion of ink in water"
       style="max-width: 700px; width: 100%; border-radius: 8px;">
</div>

This process is called **diffusion**, the transfer of particles from a region of higher concentration to a region of lower concentration. Diffusion occurs due to the underlying random, or Brownian, motion of the particles.

What would be an appropriate way to measure diffusion? We know diffusion depends on time, so we need a measure that captures how far particles spread as time passes.

A naive idea is to take the average displacement of all the particles from the initial point. But since diffusion is a random walk, each particle has an equal chance of moving left or right. When we add up all these displacements, they cancel out, and the average displacement is always close to zero. So the simple arithmetic mean is a poor choice.

Instead, we use the **root mean square (RMS) displacement**, which is a statistical mean:

1. Square each displacement (this removes negative signs so left and right don’t cancel).  
2. Take the average (mean) of these squared displacements.  
3. Take the square root to return to distance units.

> **RMS displacement**
>
> $$
> r_{\text{rms}}(t) =
> \sqrt{\frac{r_1^2(t) + r_2^2(t) + \dots + r_N^2(t)}{N}}
> $$
>
> where  
> $r_i(t)$ – displacement of the $i^{\text{th}}$ particle at time $t$  
> $N$ – total number of particles

This RMS distance gives us a meaningful measure of how far particles typically wander away from their starting point due to random motion.

For diffusive motion in 2D, the RMS distance is related to the diffusion constant by

> **RMS distance in 2D**
>
> $$
> r_{\text{rms}}(t) = \sqrt{4 D t}
> $$
>
> where  
> $D$ – diffusion constant  
> $t$ – time

The reason for the random motion is thermal agitation in the system. Einstein proposed that the diffusion constant depends on the temperature of the system and on a quantity called the **mobility**, defined as

$$
\mu = \frac{v}{F},
$$

which quantifies how easily an object moves under an applied force.

Einstein related diffusion to mobility through

$$
D = \mu k_B T,
$$

where $k_B$ is Boltzmann’s constant and $T$ is the absolute temperature.

During random motion in a liquid, the dominant force experienced by the particle is the viscous drag, given by Stokes’ law:

$$
F_{\text{viscous}} = 6\pi \eta r v,
$$

where $\eta$ is the viscosity of the fluid and $r$ is the radius of the particle. Therefore, the mobility is

$$
\mu = \frac{v}{F_{\text{viscous}}} = \frac{1}{6\pi \eta r}.
$$

Combining the two relations gives the famous **Stokes–Einstein relation**:

> **Diffusion constant $D$**
>
> $$
> D = \frac{k_B T}{6\pi \eta r}
> $$
>
> where  
> $T$ – temperature  
> $\eta$ – coefficient of viscosity  
> $r$ – radius of the spherical particle

<div style="text-align:center; margin: 1.5rem 0;">
  <img src="{{ '/assets/img/labnotes/vis.png' | relative_url }}"
       alt="Viscosity schematic"
       style="max-width: 700px; width: 100%; border-radius: 8px;">
</div>

<div style="text-align:center; margin: 1.5rem 0 2rem;">
  <img src="{{ '/assets/img/labnotes/excelrms.png' | relative_url }}"
       alt="Example RMS calculation in Excel"
       style="max-width: 700px; width: 100%; border-radius: 8px;">
</div>

### Using ImageJ data

The aim of this experiment is to determine how bead radius and fluid viscosity affect the diffusion constant.

Following the lab manual, you will record three videos of beads suspended in liquid and track at least 10 particles. From the ImageJ output, you will obtain the $x$ and $y$ positions of the tracked particles.

- Take the position at the first frame ($t=0$) as the initial position.
- At each later frame, the displacement of a bead is

  $$
  r(t) = \sqrt{(x(t) - x(0))^2 + (y(t) - y(0))^2}.
  $$

Then compute the squared RMS distance for each time frame:

$$
r_{\text{rms}}^2(t) =
\frac{r_1^2(t) + r_2^2(t) + \dots + r_{10}^2(t)}{10}.
$$

Taking the square root gives $r_{\text{rms}}(t)$.

According to the 2D RMS relation,

$$
r_{\text{rms}}^2 = 4 D t.
$$

So if we plot $r_{\text{rms}}^2$ (on the y-axis) versus time $t$ (on the x-axis), we should obtain a straight line of the form $y = mx$. The slope of this line is $4D$.

Therefore, the diffusion constant is

$$
D = \frac{\text{slope}}{4}.
$$

<div style="text-align:center; margin: 1.5rem 0 2rem;">
  <img src="{{ '/assets/img/labnotes/graph.png' | relative_url }}"
       alt="Example r_rms^2 vs t graph"
       style="max-width: 450px; width: 100%; border-radius: 8px;">
</div>

---

## Experiment 4 – Random + directed motion

In the previous experiment, we studied Brownian motion—the random motion of microscopic beads suspended in water—and observed how the radius of the bead and the viscosity of the fluid influence the diffusion constant. In that case, the motion was driven entirely by thermal agitation, so the particles had no preferred direction of movement.

In this week’s experiment, we perform a similar observation, but we now tilt the microscope stage, introducing a gravitational force component. This adds a directed force that tends to pull the beads in one direction.

- Random motion (Brownian motion) causes particles to spread out in all directions.  
- Directed motion (due to gravity) causes particles to drift preferentially in one direction.

The motion we observe will be a combination of these two effects. The key objective is to determine which type of motion dominates under different conditions, especially how this depends on bead size.

- Smaller beads are strongly influenced by random motion.  
- Larger beads are more affected by gravity.

To distinguish between these behaviors quantitatively, we will analyze bead trajectories using **log–log plots** of mean-squared displacement versus time, which allows us to identify whether the motion is primarily diffusive, primarily directed, or a mixture of both.

### Purely random (diffusive) motion

For Brownian motion in two dimensions, Einstein showed:

$$
R_{\text{rms}}^2 = \langle r^2(t) \rangle = 4Dt,
$$

a linear function of time.

Taking the logarithm of both sides:

$$
\log(R_{\text{rms}}^2) = \log(4D) + \log(t).
$$

So a plot of $\log(R_{\text{rms}}^2)$ vs $\log(t)$ has the form $y = mx + b$ with slope

$$
m = 1.
$$

> **Diffusion-dominated motion**: slope $\approx 1$ on a log–log plot.

<div style="text-align:center; margin: 1.5rem 0;">
  <img src="{{ '/assets/img/labnotes/only diffusion.jpg' | relative_url }}"
       alt="Diffusion-only graphs"
       style="max-width: 700px; width: 100%; border-radius: 8px;">
</div>

### Purely directed motion

If a constant force acts on the particle, it moves with a constant velocity $v$. For microscopic particles in water, viscous drag is so strong that they reach terminal velocity almost instantly, so displacement grows *linearly* in time:

$$
r(t) = vt \quad \Rightarrow \quad R_{\text{rms}}^2 = v^2 t^2.
$$

Taking the logarithm:

$$
\log(R_{\text{rms}}^2) = \log(v^2) + 2\log(t).
$$

So the slope on a log–log plot is

$$
m = 2.
$$

> **Directed motion**: slope $\approx 2$ on a log–log plot.

<div style="text-align:center; margin: 1.5rem 0;">
  <img src="{{ '/assets/img/labnotes/only directed .jpg' | relative_url }}"
       alt="Directed-only graphs"
       style="max-width: 700px; width: 100%; border-radius: 8px;">
</div>

### Mixed motion

In many biological and experimental systems, both random and directed motion occur. In these cases:

$$
\langle r^2(t) \rangle \propto t^\alpha,
$$

with $1 < \alpha < 2$. The exponent $\alpha$ tells you the balance between Brownian motion and directed drift.

<div style="text-align:center; margin: 1.5rem 0;">
  <img src="{{ '/assets/img/labnotes/both equal.jpg' | relative_url }}"
       alt="Mixed motion graphs"
       style="max-width: 700px; width: 100%; border-radius: 8px;">
</div>

If both effects are about equal, the slope will be around $1.5$.

In this experiment:

- $2\,\mu\text{m}$ beads are more affected by Brownian motion, so we expect slopes closer to 1 (about 1–1.5).  
- $5\,\mu\text{m}$ beads feel the directed motion more, so their slopes should be closer to 2 (about 1.5–2).

The exact value depends on how much the microscope is tilted and how well the tracking is done.

### Example data sheet and graphs

<div style="text-align:center; margin: 1.5rem 0;">
  <img src="{{ '/assets/img/labnotes/exp4excel.jpg' | relative_url }}"
       alt="Example Excel data for Experiment 4"
       style="max-width: 700px; width: 100%; border-radius: 8px;">
</div>

<div style="text-align:center; margin: 1.5rem 0 2rem;">
  <img src="{{ '/assets/img/labnotes/exp4Graphs.png' | relative_url }}"
       alt="Example graphs for Experiment 4"
       style="max-width: 700px; width: 100%; border-radius: 8px;">
</div>

---

## Experiment 5 – Vesicle motion, ATP hydrolysis & viscosity

To calculate the **rate of ATP hydrolysis** $R$ and the **coefficient of viscosity** $\mu$, you will use the average radius $r$ and average speed $v$ obtained from ImageJ. With these values, you can proceed as follows.

<div style="text-align:center; margin: 1.5rem 0;">
  <img src="{{ '/assets/img/labnotes/viscous.png' | relative_url }}"
       alt="Vesicle moving through viscous medium"
       style="max-width: 450px; width: 100%; border-radius: 8px;">
</div>

### Work and power

Work done on an object by a force $\mathbf{F}$ causing a displacement $\mathbf{d}$ is

$$
W = \mathbf{F} \cdot \mathbf{d} = |\mathbf{F}|\,|\mathbf{d}| \cos\theta,
$$

where $\theta$ is the angle between the force and displacement. In our case, the viscous drag force is opposite to the direction of motion ($\theta = 180^\circ$), so the work done by the viscous force is negative. In terms of magnitudes we will use

$$
|W| = |\mathbf{F}|\,|\mathbf{d}|.
$$

Power is defined as the rate of doing work:

$$
P = \frac{W}{t}.
$$

Useful biological numbers:

- Average kinesin step size: $s_{\text{kin}} \approx 8\,\text{nm}$  
- Average myosin step size: $s_{\text{myo}} \approx 10\,\text{nm}$  
- One “step” $\approx$ one ATP hydrolysis cycle  
- Energy released per mole of ATP: $E_{\text{mol}} \approx 23\ \text{kJ/mol}$  
- To get the energy per ATP molecule:

  $$
  E = \frac{E_{\text{mol}}}{N_A},
  $$

  where $N_A$ is Avogadro’s number.  

- Motor efficiency: $e \approx 60\% = 0.6$

The efficiency is

$$
e = \frac{W_{\text{produced}}}{E_{\text{consumed}}}
  = \frac{P_{\text{produced}}}{P_{\text{consumed}}}.
$$

The total work **consumed** comes from ATP hydrolysis. If $N$ is the number of ATP cycles in a time $t$ and $E$ is the energy per ATP, then

$$
P_{\text{consumed}} = \frac{W_{\text{consumed}}}{t}
= \frac{N E}{t} = R E,
$$

where

$$
R = \frac{N}{t}
$$

is the **rate of ATP hydrolysis** (ATP molecules per second).

Since the vesicle moves with approximately constant velocity, the net force is zero: the forward motor force equals the viscous drag. The mechanical power **produced** by the vesicle is

$$
P_{\text{produced}} = \frac{W_{\text{produced}}}{t}
= \frac{F d}{t} = F v,
$$

where $F$ is the magnitude of the force exerted by the motor and $v$ is the speed.

### Rate of ATP hydrolysis $R$ from average velocity $v$

The average velocity is

$$
v = \frac{d}{t}.
$$

If $N$ is the number of ATP cycles and $s$ is the step size of the motor, then $d = N s$ and

$$
v = \frac{N s}{t} = R s.
$$

Thus,

$$
R = \frac{v}{s}.
$$

**Important:** use SI units.

- Step size in meters ($1\ \text{nm} = 10^{-9}\ \text{m}$)  
- $v$ in m/s (convert from $\mu\text{m/s}$, etc.)

### Coefficient of viscosity $\mu$ from average radius $r$

The viscous drag force on a slowly moving spherical particle is given by Stokes’ law:

$$
F_{\text{viscous}} = 6 \pi \mu r v,
$$

where

- $r$ – average radius of the vesicle  
- $v$ – terminal (steady) velocity  
- $\mu$ – dynamic viscosity of the cytosol

From the efficiency relation,

$$
e \, P_{\text{consumed}} = P_{\text{produced}},
$$

so

$$
e \, R E = F v.
$$

Hence

$$
F = \frac{e R E}{v}.
$$

Using Stokes’ law:

$$
\mu = \frac{F}{6\pi r v}
= \frac{e R E / v}{6\pi r v}
= \frac{e R E}{6\pi r v^2}.
$$

Using $R = v/s$ we get

$$
\mu = \frac{e (v/s) E}{6\pi r v^2}
    = \frac{e E}{6\pi r v s}.
$$

Again, use SI units for all quantities:

- $r$ in meters  
- $v$ in m/s  
- $s$ in meters  
- $E$ in joules per ATP molecule

In this experiment, we cannot distinguish between kinesin and myosin motors, so we compute $\mu$ for both:

- Kinesin: $s = 8\,\text{nm}$  
- Myosin: $s = 10\,\text{nm}$  

The calculated values can then be compared with the viscosity of water,

$$
\mu_{\text{water}} \approx 8.6 \times 10^{-4}\ \text{Pa·s}.
$$

A significantly larger effective viscosity suggests that the cytosol behaves as a more crowded and structured medium than pure water.

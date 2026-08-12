<style>
  .research-intro {
    font-size: 1.08rem;
    line-height: 1.75;
    margin-bottom: 1.5rem;
  }

  .research-section {
    margin: 2.4rem 0;
  }

  .research-section p {
    line-height: 1.75;
    text-align: justify;
  }

  .research-figure {
    margin: 1.8rem auto 2.2rem auto;
    text-align: center;
  }

  .research-figure img {
    display: block;
    max-width: 100%;
    height: auto;
    margin: 0 auto;
    background: #ffffff;
    border-radius: 12px;
    padding: 0.35rem;
    box-shadow: 0 8px 24px rgba(0,0,0,0.35);
  }

  .research-figure figcaption {
    margin-top: 0.75rem;
    font-size: 0.92rem;
    line-height: 1.5;
    opacity: 0.82;
  }

  .research-grid {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 1.25rem;
    margin: 1.5rem 0 2rem 0;
  }

  .research-card {
    border: 1px solid rgba(255,255,255,0.12);
    border-radius: 12px;
    padding: 1rem 1.15rem;
    background: rgba(255,255,255,0.025);
  }

  .research-card h3 {
    margin-top: 0;
  }

  .research-card p,
  .research-card li {
    line-height: 1.6;
  }

  .research-button {
    display: inline-block;
    padding: 0.6rem 1rem;
    margin: 0.35rem 0.4rem 0.35rem 0;
    border: 1px solid rgba(122,162,255,0.75);
    border-radius: 8px;
    text-decoration: none;
  }

  .research-button:hover {
    text-decoration: none;
  }

  .wide-figure img {
    width: 100%;
  }

  @media (max-width: 768px) {
    .research-grid {
      grid-template-columns: 1fr;
    }

    .research-section p {
      text-align: left;
    }
  }
</style>

<div class="research-intro">
My research lies at the intersection of <strong>condensed matter physics, superconductivity, and quantum transport</strong>. My doctoral work focused on non-reciprocal superconducting transport in gated semiconductor-superconductor planar Josephson junctions, with particular emphasis on the <strong>superconducting diode effect (SDE)</strong>. I am interested in how symmetry, spin-orbit coupling, magnetic fields, electrostatic gating, junction transparency, and disorder can be used to understand and control transport in low-dimensional quantum systems.
</div>

<a class="research-button" href="/doc/Abhishek_Dissertation_2026.pdf" target="_blank" rel="noopener noreferrer">Ph.D. Dissertation →</a><a class="research-button" href="/publications/">Publications →</a>

<div class="research-section">

Planar semiconductor-superconductor Josephson junctions

A conventional Josephson junction consists of two superconductors separated by a weak link. In the systems I study, the weak link is formed in a high-mobility semiconductor two-dimensional electron gas (2DEG) that is proximitized by superconducting electrodes. Superconducting correlations extend into the semiconductor through the proximity effect, allowing a dissipationless Josephson current to flow through a region that is not intrinsically superconducting.

Planar junctions are particularly attractive because the semiconductor weak link can be highly transparent and strongly tunable. A top gate can modify the carrier density and the junction potential, while an in-plane magnetic field couples strongly to the electronic spin through the large effective g-factor of the semiconductor. Materials such as InAs and InSb can also host strong Rashba and Dresselhaus spin-orbit coupling. Together, these ingredients provide several experimentally controllable parameters for manipulating the Andreev spectrum and the Josephson current.

<figure class="research-figure wide-figure">
  <a href="/assets/img/research/planar_jj_geometry.png" target="_blank" rel="noopener noreferrer">
    <img src="/assets/img/research/planar_jj_geometry.png" alt="Schematic of a gated planar Josephson junction, coordinate system, and tight-binding lattice">
  </a>
  <figcaption>
    Geometry used in my theoretical modeling: a gated planar Josephson junction formed in a proximitized 2DEG, together with the magnetic-field and crystallographic angles and the square-lattice discretization used in the tight-binding calculations. Figure extracted from my dissertation (Fig. 8).
  </figcaption>
</figure>

</div>

<div class="research-section">

Superconducting diode effect

The superconducting diode effect is a non-reciprocal form of Josephson transport in which the maximum dissipationless current depends on the direction of current flow. If the forward and reverse critical-current magnitudes are denoted by (I_c^+) and (|I_c^-|), respectively, the SDE occurs when

$$|I_c^+| \neq |I_c^-|.$$

I characterize the strength and polarity of this response using the diode efficiency

$$\eta(B)=\frac{|I_c^+(B)|-|I_c^-(B)|}{I_0},$$

where (I_0) is the zero-field critical current. A nonzero (\eta) indicates non-reciprocal critical currents, while a change in the sign of (\eta) corresponds to a reversal of the diode polarity.

A central question in my dissertation was not simply whether a diode effect exists, but <strong>what microscopic mechanism produces it</strong>. In the mechanism I investigated, inversion symmetry is broken by Rashba and/or Dresselhaus spin-orbit coupling, while time-reversal symmetry is broken by an in-plane magnetic field through the Zeeman interaction. Their interplay modifies the spin-dependent Fermi contours and the Andreev spectrum, producing a non-reciprocal current-phase relation.

</div>

<div class="research-section">

Finite-momentum Cooper pairing and symmetry

One useful microscopic picture is the formation of Cooper pairs with a finite center-of-mass momentum. Rashba spin-orbit coupling creates a momentum-dependent spin texture, and an in-plane Zeeman field distorts the spin-split Fermi contours. For appropriate field orientations, the electronic states that pair no longer have exactly opposite momenta, allowing the Cooper pair to acquire a finite momentum along the current direction.

An important point, however, is that <strong>finite Cooper-pair momentum alone is not sufficient to create a phase-unbiased superconducting diode effect</strong>. A simple phase-shifted sinusoidal current-phase relation can have an anomalous ground-state phase while still producing equal forward and reverse critical-current magnitudes. The diode effect requires an additional asymmetry of the phase-dependent spectrum and, in practice, contributions beyond a single sinusoidal harmonic.

<figure class="research-figure">
  <a href="/assets/img/research/cooper_pair_momentum.png" target="_blank" rel="noopener noreferrer">
    <img src="/assets/img/research/cooper_pair_momentum.png" alt="Spin-split Fermi contours illustrating finite Cooper-pair momentum and the superconducting diode effect">
  </a>
  <figcaption>
    Qualitative Fermi-contour picture showing how Rashba spin-orbit coupling and magnetic-field orientation determine the Cooper-pair momentum. The SDE is symmetry-allowed when Rashba SOC and a field along the junction coexist, while other configurations suppress the diode response. Figure extracted from my dissertation (Fig. 12).
  </figcaption>
</figure>

</div>

<div class="research-section">

Analytical and numerical modeling

I use complementary analytical and numerical approaches based on the Bogoliubov-de Gennes (BdG) formalism. The analytical treatment considers a short-junction limit and provides compact expressions that reveal how spin-orbit coupling, Zeeman energy, and junction transparency enter the Andreev spectrum and the critical currents. This approach is particularly useful for identifying symmetry relations and understanding low-field trends.

For realistic geometries, I discretize the continuum BdG Hamiltonian on a square lattice and solve the resulting tight-binding problem using <strong>Kwant</strong> and numerical diagonalization routines. From the phase-dependent quasiparticle spectrum, I calculate the free energy and obtain the Josephson current from its phase derivative. This framework allows the inclusion of realistic device dimensions, finite magnetic fields, Rashba and Dresselhaus spin-orbit coupling, gate-induced potential changes, and disorder.

<div class="research-grid">
  <div class="research-card">
    <h3>Analytical tools</h3>
    <ul>
      <li>Short-junction and delta-barrier models</li>
      <li>Andreev-bound-state spectra</li>
      <li>Symmetry analysis</li>
      <li>Low-field expansions of critical current and diode efficiency</li>
    </ul>
  </div>
  <div class="research-card">
    <h3>Computational tools</h3>
    <ul>
      <li>Bogoliubov-de Gennes Hamiltonians</li>
      <li>Tight-binding discretization</li>
      <li>Kwant and Python-based numerical simulations</li>
      <li>Free-energy and current-phase-relation calculations</li>
    </ul>
  </div>
</div>

</div>

<div class="research-section">

Magneto-current-phase relation and Rashba spin-orbit coupling

The full current-phase relation contains substantially more information than the critical current alone. I studied the <strong>magneto-current-phase relation (magneto-CPR)</strong>, in which the Josephson current is resolved simultaneously as a function of superconducting phase difference and magnetic field.

The phase-resolved current asymmetry reveals regions of positive and negative non-reciprocity and also determines the equilibrium ground-state phase of a phase-unbiased junction. As the Zeeman energy is varied, the ground-state phase can undergo discontinuous, 0-(\pi)-like jumps. In the analytical model, the size of these jumps depends strongly on the Rashba spin-orbit-coupling strength. This provides a possible way to extract microscopic SOC information from phase-sensitive Josephson measurements.

<div class="research-grid">
  <figure class="research-figure">
    <a href="/assets/img/research/magneto_cpr.png" target="_blank" rel="noopener noreferrer">
      <img src="/assets/img/research/magneto_cpr.png" alt="Magneto-current-phase relation and phase-resolved current asymmetry">
    </a>
    <figcaption>
      Numerical magneto-CPR signatures of non-reciprocity and the ground-state phase trajectory. Figure extracted from my dissertation (Fig. 16; adapted there from Ref. 61).
    </figcaption>
  </figure>

  <figure class="research-figure">
    <a href="/assets/img/research/rashba_soc_phase_jump.png" target="_blank" rel="noopener noreferrer">
      <img src="/assets/img/research/rashba_soc_phase_jump.png" alt="Relation between Rashba spin-orbit coupling and the ground-state phase jump">
    </a>
    <figcaption>
      Analytical and tight-binding relation between the normalized Rashba SOC wave vector and the size of the ground-state phase jump. Figure extracted from my dissertation (Fig. 17; adapted there from Ref. 61).
    </figcaption>
  </figure>
</div>

</div>

<div class="research-section">

Magnetic and crystalline anisotropy

A major part of my doctoral work was devoted to using anisotropy as a diagnostic of the microscopic origin of non-reciprocal transport. Rashba and Dresselhaus spin-orbit couplings have different symmetry properties, and this difference produces experimentally distinguishable angular signatures.

For <strong>pure Rashba SOC</strong>, the spin-orbit interaction is rotationally invariant within the plane of the 2DEG. The diode effect therefore exhibits strong <strong>magnetic anisotropy</strong>: rotating the in-plane magnetic field changes the Cooper-pair momentum and can completely suppress the SDE for symmetry-selected field directions. By contrast, there is no intrinsic crystalline anisotropy in the pure-Rashba limit.

<figure class="research-figure">
  <a href="/assets/img/research/rashba_anisotropy.png" target="_blank" rel="noopener noreferrer">
    <img src="/assets/img/research/rashba_anisotropy.png" alt="Magnetic anisotropy of the superconducting diode effect for Rashba spin-orbit coupling">
  </a>
  <figcaption>
    Magneto-anisotropic diode efficiency for a Rashba-dominated Al/InAs junction. Numerical and analytical calculations show symmetry-imposed directions along which the diode effect is suppressed. Figure extracted from my dissertation (Fig. 20).
  </figcaption>
</figure>

For <strong>Dresselhaus SOC</strong>, rotational symmetry is broken by the underlying crystal. The diode response then depends not only on the magnetic-field direction but also on the orientation of the junction relative to the crystallographic axes. This produces a <strong>magneto-crystalline anisotropy</strong> that can be used to distinguish Rashba- and Dresselhaus-dominated regimes and to identify symmetry-imposed zeros and polarity reversals of the SDE.

<figure class="research-figure">
  <a href="/assets/img/research/dresselhaus_anisotropy.png" target="_blank" rel="noopener noreferrer">
    <img src="/assets/img/research/dresselhaus_anisotropy.png" alt="Crystalline anisotropy of the superconducting diode effect for Dresselhaus spin-orbit coupling">
  </a>
  <figcaption>
    Crystalline anisotropy of the diode efficiency in an Al/InSb junction with pure Dresselhaus SOC. The green directions correspond to symmetry-imposed suppression of the SDE. Figure extracted from my dissertation (Fig. 22).
  </figcaption>
</figure>

</div>

<div class="research-section">

Gate control, junction transparency, and polarity reversal

Electrostatic gating provides another way to control the superconducting diode response. In the analytical model, changing the junction potential modifies the transparency of the weak link. In a nearly transparent junction, the critical-current maxima remain close to zero magnetic field; reducing the transparency shifts these maxima to finite fields and changes the low-field behavior of the diode efficiency.

In my numerical tight-binding calculations, the gate is modeled by changing the chemical potential in the non-proximitized region relative to the superconducting regions. Even in a purely Rashba system, tuning this potential can substantially modify the diode response and generate additional <strong>low-field polarity reversals</strong>. These reversals occur where the forward and reverse critical-current branches cross.

<figure class="research-figure">
  <a href="/assets/img/research/gate_tuning.png" target="_blank" rel="noopener noreferrer">
    <img src="/assets/img/research/gate_tuning.png" alt="Gate-dependent tuning and polarity reversal of the superconducting diode effect">
  </a>
  <figcaption>
    Numerical gate-potential dependence of the diode efficiency and critical currents in a Rashba Al/InAs junction. Gate-induced changes in the junction potential can create additional low-field polarity reversals. Figure extracted from my dissertation (Fig. 28).
  </figcaption>
</figure>

</div>

<div class="research-section">

Disorder and microscopic details of the weak link

I also investigated how disorder modifies non-reciprocal transport by introducing spatially distributed impurity potentials into the tight-binding model. Weak disorder changes the detailed magnetic-field dependence while preserving a finite diode response. Stronger disorder can reshape the critical-current curves and produce additional polarity reversals.

These calculations show that the SDE is sensitive not only to global control parameters such as magnetic field and gate voltage, but also to the microscopic potential landscape of the weak link. A systematic statistical treatment over many impurity realizations would be a natural extension of this work.

<figure class="research-figure">
  <a href="/assets/img/research/disorder_sde.png" target="_blank" rel="noopener noreferrer">
    <img src="/assets/img/research/disorder_sde.png" alt="Effect of weak and strong disorder on the superconducting diode efficiency and critical currents">
  </a>
  <figcaption>
    Magnetic-field dependence of the diode efficiency and critical currents for a clean junction and for two disorder strengths. Figure extracted from my dissertation (Fig. 30).
  </figcaption>
</figure>

</div>

<div class="research-section">

Current and recent research interests

<div class="research-grid">
  <div class="research-card">
    <h3>Superconductivity & Josephson junctions</h3>
    <ul>
      <li>Planar semiconductor-superconductor Josephson junctions in proximitized 2DEGs</li>
      <li>Non-reciprocal supercurrent and the superconducting diode effect</li>
      <li>Andreev bound states and phase-dependent transport</li>
      <li>Magnetic-field, temperature, and transparency dependence of Josephson transport</li>
    </ul>
  </div>

  <div class="research-card">
    <h3>Spin-orbit coupling & anisotropy</h3>
    <ul>
      <li>Rashba and Dresselhaus spin-orbit coupling</li>
      <li>Magnetic and crystalline anisotropies</li>
      <li>Symmetry-controlled suppression and polarity reversal of non-reciprocal transport</li>
      <li>Spin-dependent transport in semiconductor heterostructures</li>
    </ul>
  </div>

  <div class="research-card">
    <h3>Quantum transport</h3>
    <ul>
      <li>Mesoscopic and low-dimensional transport</li>
      <li>Semiconductor-superconductor hybrid systems</li>
      <li>Phase-sensitive superconducting transport</li>
      <li>Gate-tunable quantum devices</li>
    </ul>
  </div>

  <div class="research-card">
    <h3>Computational & theoretical physics</h3>
    <ul>
      <li>Tight-binding and finite-difference models</li>
      <li>Bogoliubov-de Gennes theory</li>
      <li>Kwant and Python-based scientific computing</li>
      <li>Analytical modeling of quantum and superconducting systems</li>
    </ul>
  </div>
</div>

</div>

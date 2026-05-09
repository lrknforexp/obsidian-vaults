---
tags: [chemistry, honors, science, lab, periodic-table, reactions, stoichiometry, bonding]
subject: Chemistry Honors Lec/Lab
created: 2025-01-01
updated: 2025-01-01
status: active
---

# ⚗️ Chemistry Honors Lec/Lab

> [!abstract] Course Overview
> Chemistry Honors Lecture/Lab is a rigorous, college-preparatory study of matter and its transformations. Topics include atomic structure, the periodic table, chemical bonding, reactions and stoichiometry, gas laws, solutions, thermodynamics, reaction kinetics, equilibrium, acids and bases, electrochemistry, and organic chemistry. Lab work emphasizes the scientific method, safe practices, data analysis, and quantitative reasoning.

---

## 🔬 Matter & Measurement

### States of Matter

| State | Particle Arrangement | Shape | Volume | Compressible? |
|---|---|---|---|---|
| **Solid** | Closely packed; rigid lattice | Fixed | Fixed | No |
| **Liquid** | Closely packed; can flow | Takes container shape | Fixed | No |
| **Gas** | Far apart; random motion | Takes container shape | Takes container shape | Yes |
| **Plasma** | Ionized gas; high energy | Variable | Variable | Yes |

### Phase Changes
```
                  Melting  →
SOLID ←→ Liquid ←→ GAS
       ← Freezing    Condensation ←
                  ↑ Sublimation ↑
                  ↓ Deposition  ↓
```

| Change | Direction | Energy |
|---|---|---|
| Melting | Solid → Liquid | Absorbed (endothermic) |
| Freezing | Liquid → Solid | Released (exothermic) |
| Vaporization/Boiling | Liquid → Gas | Absorbed (endothermic) |
| Condensation | Gas → Liquid | Released (exothermic) |
| Sublimation | Solid → Gas | Absorbed (endothermic) |
| Deposition | Gas → Solid | Released (exothermic) |

### Physical vs. Chemical Properties

**Physical Properties** — Observed without changing chemical composition:
- Color, odor, density, melting point, boiling point, solubility, conductivity, malleability

**Chemical Properties** — Describes ability to undergo chemical change:
- Flammability, reactivity with acid, oxidation, toxicity

**Intensive vs. Extensive Properties:**
- **Intensive** — Independent of sample size: density, temperature, boiling point, color
- **Extensive** — Depend on sample size: mass, volume, length, energy

### Significant Figures Rules

> [!tip] Sig Fig Rules
> 1. Non-zero digits are always significant
> 2. Zeros between non-zeros are significant (1003 = 4 sig figs)
> 3. Leading zeros are NOT significant (0.0023 = 2 sig figs)
> 4. Trailing zeros after decimal ARE significant (1.200 = 4 sig figs)
> 5. Trailing zeros without decimal are ambiguous (use scientific notation)

**Operations:**
- **Multiplication/Division** — Answer has same sig figs as measurement with FEWEST sig figs
- **Addition/Subtraction** — Answer has same decimal places as measurement with FEWEST decimal places

### Scientific Notation
> A number in the form: **M × 10ⁿ**
> Where 1 ≤ M < 10 and n is an integer

- 6,022,000,000,000,000,000,000,000 = 6.022 × 10²³ (Avogadro's number)
- 0.000000001 m = 1 × 10⁻⁹ m (1 nanometer)

### SI Units (International System)

| Quantity | SI Unit | Symbol |
|---|---|---|
| Length | Meter | m |
| Mass | Kilogram | kg |
| Time | Second | s |
| Temperature | Kelvin | K |
| Amount of substance | Mole | mol |
| Electric current | Ampere | A |
| Luminous intensity | Candela | cd |

**Prefixes:**
| Prefix | Symbol | Multiplier |
|---|---|---|
| Giga | G | 10⁹ |
| Mega | M | 10⁶ |
| Kilo | k | 10³ |
| Deci | d | 10⁻¹ |
| Centi | c | 10⁻² |
| Milli | m | 10⁻³ |
| Micro | μ | 10⁻⁶ |
| Nano | n | 10⁻⁹ |

### Temperature Conversions
- °C = (°F − 32) × 5/9
- °F = (°C × 9/5) + 32
- K = °C + 273.15
- **Absolute Zero** = 0 K = −273.15°C (no thermal motion)

---

## ⚛️ Atomic Structure

### History of the Atomic Model

| Model | Scientist | Year | Description |
|---|---|---|---|
| **Solid Sphere** | John Dalton | 1803 | Atoms as indivisible solid spheres |
| **Plum Pudding** | J.J. Thomson | 1897 | Electrons embedded in positive sphere; discovered electron via cathode ray |
| **Nuclear** | Ernest Rutherford | 1911 | Dense positive nucleus; gold foil experiment; mostly empty space |
| **Planetary/Bohr** | Niels Bohr | 1913 | Electrons orbit nucleus in fixed energy levels; explains hydrogen spectrum |
| **Quantum Mechanical** | Schrödinger/Heisenberg | 1926+ | Electron probability clouds (orbitals); uncertainty principle |

### Subatomic Particles

| Particle | Symbol | Charge | Mass (amu) | Location |
|---|---|---|---|---|
| **Proton** | p⁺ | +1 | 1.0073 | Nucleus |
| **Neutron** | n⁰ | 0 | 1.0087 | Nucleus |
| **Electron** | e⁻ | −1 | 0.000549 | Electron cloud |

> [!info] Key Definitions
> - **Atomic Number (Z)** — Number of protons; defines the element; found on periodic table
> - **Mass Number (A)** — Protons + neutrons = nucleons
> - **Isotopes** — Same element (same protons); different neutrons; same chemical properties; different masses
> - **Ions** — Atom that has gained or lost electrons
>   - *Cation* (+) — Lost electrons (metals)
>   - *Anion* (−) — Gained electrons (nonmetals)

### Average Atomic Mass
> Weighted average of all isotopes' masses based on natural abundance
> **Avg. mass = Σ (fractional abundance × isotope mass)**

Example: Chlorine-35 (75.77%) and Chlorine-37 (24.23%):
= (0.7577 × 34.969) + (0.2423 × 36.966) = **35.45 amu**

### Electron Configuration

**Quantum Numbers:**
1. **Principal (n)** — Energy level; n = 1, 2, 3... (shell)
2. **Angular momentum (ℓ)** — Subshell shape; ℓ = 0 to n-1 (s, p, d, f)
3. **Magnetic (mℓ)** — Orbital orientation; mℓ = −ℓ to +ℓ
4. **Spin (ms)** — +½ or −½ (Pauli exclusion: no two electrons same 4 quantum numbers)

**Subshell Capacities:**
| Subshell | ℓ | # of orbitals | Max electrons |
|---|---|---|---|
| s | 0 | 1 | 2 |
| p | 1 | 3 | 6 |
| d | 2 | 5 | 10 |
| f | 3 | 7 | 14 |

**Filling Order (Aufbau Principle):**
1s → 2s → 2p → 3s → 3p → 4s → 3d → 4p → 5s → 4d → 5p → 6s → 4f → 5d → 6p...

**Hund's Rule:** Electrons fill orbitals singly before pairing (like seats on a bus)

**Pauli Exclusion Principle:** No two electrons can have the same 4 quantum numbers; max 2 electrons per orbital

**Example:** Sodium (Na, Z=11): 1s² 2s² 2p⁶ 3s¹ (or [Ne] 3s¹)

---

## 📊 The Periodic Table

### Organization
- **Periods (rows)** — 7 horizontal rows; elements in same period have same number of electron shells
- **Groups/Families (columns)** — 18 vertical columns; elements in same group have same valence electrons → similar chemical properties

### Key Groups

| Group | Name | Valence e⁻ | Properties |
|---|---|---|---|
| 1 (IA) | Alkali metals | 1 | Highly reactive; soft; react vigorously with water |
| 2 (IIA) | Alkaline earth metals | 2 | Reactive; harder than group 1 |
| 3–12 | Transition metals | Varies | Multiple oxidation states; colored compounds; good conductors |
| 13 (IIIA) | Boron group | 3 | Metalloids, metals |
| 14 (IVA) | Carbon group | 4 | From nonmetals to metals; carbon = basis of life |
| 15 (VA) | Nitrogen group (Pnictogens) | 5 | Nonmetals to metalloids to metals |
| 16 (VIA) | Oxygen group (Chalcogens) | 6 | Highly electronegative |
| 17 (VIIA) | Halogens | 7 | Most reactive nonmetals; form salts with metals |
| 18 (VIIIA/0) | Noble gases | 8 (or 0) | Inert; full valence shell; very low reactivity |

### Periodic Trends

> [!note] Periodic Trends Summary
> As you move **across a period (left → right):** Atomic radius decreases; ionization energy increases; electronegativity increases
> As you move **down a group (top → bottom):** Atomic radius increases; ionization energy decreases; electronegativity decreases

**Atomic Radius:**
- Decreases left → right (more protons pulling electrons in; same shell)
- Increases top → bottom (more electron shells added)

**Ionization Energy (IE):** Energy required to remove an electron from a gaseous atom
- Increases left → right (harder to remove from more strongly attracted electrons)
- Decreases top → bottom (valence electrons farther from nucleus)

**Electronegativity:** Ability of an atom to attract electrons in a bond (Pauling scale)
- Increases left → right, decreases top → bottom
- Most electronegative: Fluorine (F) = 3.98
- Least electronegative (among metals): Cesium (Cs) = 0.79

**Electron Affinity:** Energy change when an atom gains an electron
- Generally increases left → right

**Ionic Radius:**
- Cations are smaller than parent atom (lost electrons, same/fewer shells)
- Anions are larger than parent atom (gained electrons, more repulsion)

### Metals, Metalloids, Nonmetals

| Property | Metals | Metalloids | Nonmetals |
|---|---|---|---|
| Location | Left/center | Staircase border | Right |
| Appearance | Lustrous, shiny | Variable | Dull (except iodine) |
| Conductivity | Good conductors | Semiconductors | Poor conductors |
| Malleability | Malleable/ductile | Brittle | Brittle (solid) |
| Ionization tendency | Lose electrons (+) | Variable | Gain electrons (−) |

---

## 🔗 Chemical Bonding

### Types of Chemical Bonds

**Ionic Bonds:**
- Transfer of electrons from metal to nonmetal
- Forms oppositely charged ions (cation + anion) attracted by electrostatic forces
- Form a crystal lattice structure
- High melting/boiling points; conduct electricity when dissolved in water or molten
- Example: NaCl (sodium chloride); Na⁺ + Cl⁻

**Covalent Bonds:**
- Sharing of electrons between nonmetals
- **Nonpolar covalent** — Equal sharing; same element or similar electronegativities (ΔEN < 0.5)
- **Polar covalent** — Unequal sharing; different electronegativities (ΔEN 0.5–1.7)
- **Coordinate covalent** — One atom donates both electrons of the bond

**Metallic Bonds:**
- Metal cations in a "sea of delocalized electrons"
- Explains conductivity, malleability, ductility, and luster of metals

### Electronegativity & Bond Type
| ΔEN | Bond Type |
|---|---|
| 0 | Nonpolar covalent |
| 0.1–0.4 | Slightly polar covalent |
| 0.5–1.7 | Polar covalent |
| > 1.7 | Ionic |

### Lewis Dot Structures

> [!tip] Steps for Drawing Lewis Structures
> 1. Count total valence electrons
> 2. Place least electronegative element in center
> 3. Connect atoms with single bonds (use 2e⁻ per bond)
> 4. Complete octets on outer atoms (H needs only 2)
> 5. Place remaining electrons on central atom
> 6. If central atom lacks octet, convert lone pairs to multiple bonds

**Octet Rule:** Atoms tend to gain/lose/share electrons to achieve 8 valence electrons (stable like noble gases)
**Exceptions:** H (needs 2), Be (4), B (6), P/S (can expand octet beyond 8)

### VSEPR Theory (Valence Shell Electron Pair Repulsion)

> Electron pairs (bonding and lone) arrange themselves to minimize repulsion → determines molecular geometry

| Electron Groups | Lone Pairs | Geometry | Bond Angle | Example |
|---|---|---|---|---|
| 2 | 0 | Linear | 180° | CO₂, BeCl₂ |
| 3 | 0 | Trigonal planar | 120° | BF₃ |
| 3 | 1 | Bent | ~117° | SO₂ |
| 4 | 0 | Tetrahedral | 109.5° | CH₄, SiCl₄ |
| 4 | 1 | Trigonal pyramidal | ~107° | NH₃ |
| 4 | 2 | Bent | ~104.5° | H₂O |
| 5 | 0 | Trigonal bipyramidal | 90°/120° | PCl₅ |
| 6 | 0 | Octahedral | 90° | SF₆ |

**Lone pairs repel more than bonding pairs** → compress bond angles

### Molecular Polarity
- **Polar molecule** — Has net dipole moment; asymmetrical arrangement of polar bonds
- **Nonpolar molecule** — Symmetrical polar bonds cancel out (CO₂, CCl₄) OR all bonds nonpolar

### Intermolecular Forces (IMFs)

> [!info] Intermolecular Forces — Weakest to Strongest
> 1. **London Dispersion Forces (LDF)** — Temporary dipoles; present in ALL molecules; larger/heavier molecules = stronger LDF
> 2. **Dipole-Dipole** — Between polar molecules; positive end attracts negative end
> 3. **Hydrogen Bonding** — Special dipole-dipole; H bonded to F, O, or N; strongest IMF; explains water's anomalous properties

**Effects of IMFs:**
- Stronger IMFs → Higher boiling point, melting point, viscosity, surface tension
- Lower vapor pressure
- Less volatile

---

## ⚖️ Chemical Reactions & Stoichiometry

### Types of Chemical Reactions

| Type | General Form | Example |
|---|---|---|
| **Synthesis (Combination)** | A + B → AB | 2H₂ + O₂ → 2H₂O |
| **Decomposition** | AB → A + B | 2H₂O → 2H₂ + O₂ |
| **Single Replacement** | A + BC → AC + B | Zn + 2HCl → ZnCl₂ + H₂ |
| **Double Replacement** | AB + CD → AD + CB | NaCl + AgNO₃ → AgCl↓ + NaNO₃ |
| **Combustion** | CₓHᵧ + O₂ → CO₂ + H₂O | CH₄ + 2O₂ → CO₂ + 2H₂O |

### Balancing Chemical Equations

**Law of Conservation of Mass:** Matter is neither created nor destroyed; atoms are rearranged.

> [!tip] Steps to Balance
> 1. Write correct formulas for reactants and products
> 2. Count atoms of each element on both sides
> 3. Add coefficients (not subscripts!) to balance; start with the most complex molecule
> 4. Balance H and O last
> 5. Verify all atoms balance; reduce to lowest whole-number ratios

Example: ___Fe + ___O₂ → ___Fe₂O₃
Balanced: **4Fe + 3O₂ → 2Fe₂O₃** ✓ (4 Fe, 6 O each side)

### The Mole Concept

> [!success] The Mole
> **1 mole = 6.022 × 10²³ particles** (Avogadro's Number)
> A mole is the number of atoms in exactly 12 grams of Carbon-12.

**Molar Mass (M):** Mass (in grams) of 1 mole of a substance; numerically equal to atomic/molecular mass in amu

**Mole Conversions:**
```
         × molar mass          × 6.022×10²³
Moles ←————————————→ Grams    Moles ←—————————————→ Particles
       ÷ molar mass              ÷ 6.022×10²³
```

**Mole-Mole Ratios from Balanced Equations:**
The coefficients give the molar ratios. In: **N₂ + 3H₂ → 2NH₃**
- 1 mol N₂ : 3 mol H₂ : 2 mol NH₃

### Stoichiometry Steps

> [!tip] The Stoichiometry Roadmap
> **Given** (with units) → **Moles of given** → **Moles of wanted** → **Wanted** (with units)
>
> 1. Convert given amount to moles (÷ molar mass if grams; ÷ Avogadro if particles)
> 2. Use mole ratio from balanced equation
> 3. Convert moles to desired units (× molar mass if grams; × Avogadro if particles)

### Percent Composition
> **% composition = (mass of element / molar mass of compound) × 100%**

### Empirical & Molecular Formulas
- **Empirical formula** — Simplest whole-number ratio of atoms (CH₂O for glucose)
- **Molecular formula** — Actual number of atoms (C₆H₁₂O₆ for glucose)

**Finding Empirical Formula from % composition:**
1. Assume 100g sample → grams = percentages
2. Convert grams to moles (÷ molar mass)
3. Divide all moles by smallest value
4. Round to nearest whole number (multiply if needed)

**Finding Molecular Formula:**
- n = Molar mass (given) / Empirical formula mass
- Multiply empirical formula by n

### Limiting Reagent & Percent Yield

**Limiting Reagent (Reactant):** The reactant that runs out first; determines maximum product

**Steps:**
1. Convert both reactants to moles
2. Use stoichiometry to find how much product each produces
3. The reactant producing LESS product is the limiting reagent
4. The other reactant is in excess

**Theoretical Yield** — Maximum product calculated from limiting reagent (stoichiometry)
**Actual Yield** — What you actually collect in the lab
**Percent Yield = (Actual Yield / Theoretical Yield) × 100%**

---

## 💨 Gas Laws

> [!abstract] Kinetic Molecular Theory (KMT)
> Gases consist of tiny particles in constant, random motion. Assumptions:
> 1. Gas particles have negligible volume
> 2. No attractive/repulsive forces between particles
> 3. Collisions are elastic (no kinetic energy lost)
> 4. Average KE is proportional to absolute temperature (in K)

### The Gas Laws

| Law | Relationship | Formula | Constant | Variables |
|---|---|---|---|---|
| **Boyle's Law** | P and V inversely proportional | P₁V₁ = P₂V₂ | T, n | P, V |
| **Charles's Law** | V and T directly proportional | V₁/T₁ = V₂/T₂ | P, n | V, T |
| **Gay-Lussac's Law** | P and T directly proportional | P₁/T₁ = P₂/T₂ | V, n | P, T |
| **Avogadro's Law** | V and n directly proportional | V₁/n₁ = V₂/n₂ | T, P | V, n |
| **Combined Gas Law** | P, V, T relationship | P₁V₁/T₁ = P₂V₂/T₂ | n | P, V, T |

> [!warning] Temperature MUST always be in Kelvin (K) for gas law calculations!

### Ideal Gas Law
> **PV = nRT**
>
> - P = pressure (atm)
> - V = volume (L)
> - n = moles of gas (mol)
> - R = gas constant = **0.08206 L·atm/mol·K**
> - T = temperature (K)

**STP (Standard Temperature and Pressure):** 0°C (273.15 K) and 1 atm; 1 mol ideal gas = 22.4 L

### Dalton's Law of Partial Pressures
> **P_total = P₁ + P₂ + P₃ + ...**
> Each gas in a mixture exerts pressure independently

### Graham's Law of Effusion/Diffusion
> Gases with lower molar mass effuse/diffuse faster
> **rate₁/rate₂ = √(M₂/M₁)**

---

## 💧 Solutions & Concentration

### Types of Mixtures
- **Homogeneous (Solution)** — Uniform throughout; single phase (saltwater, air)
- **Heterogeneous** — Visibly non-uniform (salad, gravel in water)
- **Colloid** — Particles 1–1000 nm; scattered light (Tyndall effect); milk, fog, gelatin
- **Suspension** — Particles > 1000 nm; settle over time; muddy water

**Solute** — Substance dissolved (less amount)
**Solvent** — Substance doing dissolving (more amount)
**"Like dissolves like"** — Polar solvents dissolve polar/ionic solutes; nonpolar solvents dissolve nonpolar solutes

### Concentration Units

**Molarity (M):**
> **M = moles of solute / liters of solution**

Most common unit in chemistry; temperature dependent

**Molality (m):**
> **m = moles of solute / kilograms of solvent**

Temperature independent; used for colligative properties

**Percent Concentration:**
- % by mass = (mass solute / mass solution) × 100
- % by volume = (volume solute / volume solution) × 100

### Dilution
> **M₁V₁ = M₂V₂** (moles of solute constant)

### Colligative Properties
Properties that depend only on the NUMBER of solute particles, not their identity:

1. **Vapor Pressure Lowering** — Adding solute lowers vapor pressure of solvent (Raoult's Law)
2. **Boiling Point Elevation** — ΔTb = kb × m × i (i = van't Hoff factor = number of ions)
3. **Freezing Point Depression** — ΔTf = kf × m × i (antifreeze works this way; salt on ice)
4. **Osmotic Pressure** — Π = iMRT (water moves across semipermeable membrane from low to high solute concentration)

---

## 🔥 Thermodynamics & Thermochemistry

### Energy Concepts
- **Thermodynamics** — Study of energy and its transformations
- **System** — The part of the universe under study
- **Surroundings** — Everything else
- **Endothermic** — System absorbs energy from surroundings; ΔH > 0 (positive)
- **Exothermic** — System releases energy to surroundings; ΔH < 0 (negative)

### Heat Calculations

**Specific Heat Capacity (c):** Energy needed to raise 1 g of substance by 1°C
- Water: c = 4.184 J/(g·°C) — highest of common substances; reason for Earth's climate moderation

> **q = mcΔT**
> - q = heat (Joules)
> - m = mass (grams)
> - c = specific heat capacity
> - ΔT = T_final − T_initial

### Hess's Law
> Enthalpy is a state function; ΔH for a reaction = sum of ΔH values of any series of steps that lead from reactants to products

**Manipulating reactions:**
- Reversing a reaction: flip sign of ΔH
- Multiplying reaction: multiply ΔH by same factor
- Add the equations and their ΔH values

### Standard Enthalpy of Formation (ΔH°f)
> Enthalpy change when 1 mole of compound is formed from elements in standard states
> Elements in standard state: ΔH°f = 0

> **ΔH°rxn = Σ ΔH°f(products) − Σ ΔH°f(reactants)**

### Entropy (S) & Gibbs Free Energy (G)

**Entropy** — Measure of disorder/randomness in a system
- Increases when: solid → liquid → gas; dissolving; temperature increases; more moles of gas produced

**Gibbs Free Energy (G):**
> **ΔG = ΔH − TΔS**
>
> - ΔG < 0 → **Spontaneous** (thermodynamically favorable)
> - ΔG > 0 → **Non-spontaneous**
> - ΔG = 0 → **Equilibrium**

| ΔH | ΔS | Spontaneous? |
|---|---|---|
| − (exo) | + (increase) | Always |
| + (endo) | − (decrease) | Never |
| − (exo) | − (decrease) | At low T |
| + (endo) | + (increase) | At high T |

---

## ⚡ Acids & Bases

### Definitions

| Theory | Acid | Base |
|---|---|---|
| **Arrhenius** | Produces H⁺ in water | Produces OH⁻ in water |
| **Brønsted-Lowry** | Proton (H⁺) donor | Proton (H⁺) acceptor |
| **Lewis** | Electron pair acceptor | Electron pair donor |

**Conjugate Acid-Base Pairs:** An acid donates H⁺ → conjugate base; a base accepts H⁺ → conjugate acid

### pH Scale

> **pH = −log[H⁺]** (concentration of H⁺ ions in mol/L)
> **pOH = −log[OH⁻]**
> **pH + pOH = 14** (at 25°C)
> **Kw = [H⁺][OH⁻] = 1.0 × 10⁻¹⁴** (at 25°C)

| pH | Solution | [H⁺] |
|---|---|---|
| 0 | Strongly acidic | 1.0 M |
| 7 | Neutral | 1.0 × 10⁻⁷ M |
| 14 | Strongly basic | 1.0 × 10⁻¹⁴ M |

### Strong vs. Weak Acids/Bases

**Strong Acids** (fully dissociate, memorize these 6):
- HCl, HBr, HI, HNO₃, H₂SO₄, HClO₄

**Strong Bases** (fully dissociate):
- Group 1 hydroxides (NaOH, KOH, LiOH); Group 2 hydroxides (Ca(OH)₂, Ba(OH)₂)

**Weak Acids** — Partially dissociate; have Ka (acid dissociation constant)
- CH₃COOH (acetic acid), HF, H₂CO₃, H₃PO₄, HNO₂

**Weak Bases** — Partially dissociate; have Kb
- NH₃, amines

### Neutralization & Titration

**Neutralization:** Acid + Base → Salt + Water
HCl + NaOH → NaCl + H₂O

**Titration:** Adding measured volume of known concentration (titrant) to unknown concentration until equivalence point
**Equivalence point:** Moles of acid = moles of base
**Indicator:** Changes color at/near equivalence point
**Titration formula:** M_a × V_a = M_b × V_b (for monoprotic acid/base)

### Buffers
- Solution that resists changes in pH when acid or base is added
- Contains weak acid + its conjugate base (or weak base + its conjugate acid)
- **Henderson-Hasselbalch:** pH = pKa + log([A⁻]/[HA])
- Example: acetic acid/acetate buffer; carbonic acid/bicarbonate (in blood)

---

## ⚖️ Chemical Equilibrium

### Dynamic Equilibrium
> When forward reaction rate = reverse reaction rate; concentrations remain constant (but not equal)
>
> For: **aA + bB ⇌ cC + dD**

### Equilibrium Constant (Keq)
> **Keq = [C]ᶜ[D]ᵈ / [A]ᵃ[B]ᵇ**

Note: **Pure solids and liquids are NOT included** in the expression (activity = 1)

**Kc** — Concentrations (mol/L)
**Kp** — Partial pressures (for gases)
**Ka** — Acid dissociation constant
**Kb** — Base dissociation constant
**Ksp** — Solubility product constant (for sparingly soluble salts)

**Interpreting Keq:**
- K >> 1 → Products favored (reaction goes mostly to completion)
- K << 1 → Reactants favored (equilibrium lies to the left)
- K ≈ 1 → Neither strongly favored

### Le Chatelier's Principle

> [!success] Le Chatelier's Principle
> If a system at equilibrium is disturbed (stress applied), it will shift in the direction that **minimizes the disturbance**.

| Stress | Shift Direction |
|---|---|
| Add reactant | → Right (toward products) |
| Remove reactant | → Left (toward reactants) |
| Add product | → Left |
| Remove product | → Right |
| Increase pressure (gases) | → Side with FEWER moles of gas |
| Decrease pressure | → Side with MORE moles of gas |
| Increase temperature | → Endothermic direction (away from heat) |
| Decrease temperature | → Exothermic direction |
| Add catalyst | No shift; equilibrium reached faster |

---

## 🔋 Electrochemistry

### Oxidation-Reduction (Redox) Reactions

> [!tip] OIL RIG
> **O**xidation **I**s **L**oss (of electrons)
> **R**eduction **I**s **G**ain (of electrons)

- **Oxidizing agent** — Causes oxidation; itself gets reduced; gains electrons
- **Reducing agent** — Causes reduction; itself gets oxidized; loses electrons

### Oxidation Numbers (Rules)
1. Pure element: oxidation number = 0
2. Monatomic ion: oxidation number = ion charge
3. O usually = −2 (except in peroxides: −1, and OF₂: +2)
4. H usually = +1 (except with metals in metal hydrides: −1)
5. Sum of oxidation numbers = charge of the species

### Galvanic (Voltaic) Cells
- Convert chemical energy → electrical energy (spontaneous; ΔG < 0)
- **Anode (−)** — Oxidation occurs; loses electrons; negative pole
- **Cathode (+)** — Reduction occurs; gains electrons; positive pole
- Electrons flow from anode → wire → cathode
- Salt bridge maintains electrical neutrality

### Standard Reduction Potentials (E°)
> **E°cell = E°cathode − E°anode**
> If E°cell > 0, reaction is spontaneous

**Relationship to Gibbs Free Energy:**
> **ΔG° = −nFE°**
> - n = moles of electrons transferred
> - F = Faraday's constant = 96,485 C/mol e⁻

### Electrolytic Cells
- Use electrical energy → drive non-spontaneous chemical reaction
- **Electrolysis of water:** 2H₂O → 2H₂ + O₂
- **Electroplating** — Coating metal objects with another metal layer

---

## 🧪 Lab Skills & Safety

### Lab Safety Rules
1. Always wear **safety goggles** and appropriate clothing (closed-toe shoes, lab coat/apron)
2. Know the location of safety equipment: eyewash station, fire extinguisher (PASS: Pull, Aim, Squeeze, Sweep), safety shower, fire blanket, first aid kit
3. Never eat, drink, or smell chemicals directly (waft toward nose)
4. Never pipette by mouth
5. Handle glassware carefully; inspect for cracks before use
6. Dispose of chemicals properly — never pour acids/bases directly down drain without neutralization
7. Report all accidents and spills to teacher immediately

### Acid/Base Spill Procedure
- **Acid spill:** Neutralize with sodium bicarbonate (baking soda, NaHCO₃)
- **Base spill:** Neutralize with dilute boric acid or vinegar
- Flush skin/eyes with large amounts of water for 15+ minutes

### Labeling Chemicals (GHS/OSHA Hazard Communication)
**GHS Pictograms (9 total):**
- Flame: flammable
- Skull/crossbones: acute toxicity
- Corrosion: skin/metal corrosion
- Exclamation mark: irritant, harmful
- Health hazard: carcinogen, reproductive toxicant
- Environment: aquatic toxicity
- Gas cylinder: compressed gas
- Exploding bomb: explosives
- Flame over circle: oxidizer

### Common Lab Equipment

| Equipment | Use |
|---|---|
| **Beaker** | Holding/mixing liquids; graduated but not precise |
| **Erlenmeyer flask** | Reactions; easy to swirl; graduated but not precise |
| **Graduated cylinder** | Measuring liquid volumes (read at bottom of meniscus) |
| **Burette** | Precise volume delivery (titrations); read from top |
| **Pipette** | Transferring precise volumes |
| **Volumetric flask** | Preparing precise concentrations |
| **Bunsen burner** | Heating; blue flame = complete combustion |
| **Ring stand + clamps** | Holding equipment |
| **Crucible** | Heating solid substances at high temperatures |
| **Centrifuge** | Separating by density |
| **Spectrophotometer** | Measuring light absorbance; Beer-Lambert Law: A = εlc |

### Significant Lab Techniques

**Filtration** — Separates solid from liquid using filter paper
**Distillation** — Separates liquids by different boiling points
**Chromatography** — Separates mixtures based on movement through a stationary phase; Rf = distance by spot / distance by solvent
**Titration** — Quantitative acid-base (or redox) analysis
**Calorimetry** — Measuring heat changes; q_solution = −q_reaction

---

## 🧬 Organic Chemistry Introduction

### Hydrocarbons

**Alkanes (CₙH₂ₙ₊₂):** Single bonds only; saturated; methane (CH₄), ethane (C₂H₆), propane, butane
**Alkenes (CₙH₂ₙ):** At least one C=C double bond; unsaturated; ethene (CH₂=CH₂)
**Alkynes (CₙH₂ₙ₋₂):** At least one C≡C triple bond; unsaturated; ethyne/acetylene (HC≡CH)
**Aromatics:** Benzene ring (alternating single/double bonds, delocalized); benzene (C₆H₆)

### Functional Groups

| Functional Group | Suffix/Prefix | Example |
|---|---|---|
| Hydroxyl (−OH) | -ol | Ethanol (C₂H₅OH) |
| Carbonyl (C=O, end of chain) | -al (aldehyde) | Formaldehyde (HCHO) |
| Carbonyl (C=O, middle of chain) | -one (ketone) | Acetone (CH₃COCH₃) |
| Carboxyl (−COOH) | -oic acid | Acetic acid (CH₃COOH) |
| Amine (−NH₂) | -amine | Methylamine |
| Ester (−COO−) | -oate | Ethyl acetate |
| Ether (−O−) | -ether / oxy- | Diethyl ether |
| Halide (−X) | halo- | Chloromethane |

### IUPAC Naming (Alkanes)
1. Find longest carbon chain → parent name
2. Identify substituents; number chain to give substituents lowest numbers
3. Name substituents as prefixes (methyl-, ethyl-, chloro-, etc.)
4. List substituents alphabetically (ignoring di-, tri-)

Prefixes: meth-(1), eth-(2), prop-(3), but-(4), pent-(5), hex-(6), hept-(7), oct-(8), non-(9), dec-(10)

---

## 🔗 Internal Links
- [[AP US History 2]]
- [[Geometry Honors]]
- [[Health 2 Drivers Ed]]
- [[IB Design Technology 1]]
- [[Intro to Engineering Design]]
- [[Mandarin 2]]

---

*Last updated: 2025 | Aligned with AP Chemistry/Honors Chemistry curriculum standards*

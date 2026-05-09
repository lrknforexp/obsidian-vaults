---
tags: [geometry, math, honors, euclidean, proofs, trigonometry]
subject: Geometry Honors
created: 2025-01-01
updated: 2025-01-01
status: active
---

# 📐 Geometry Honors

> [!abstract] Course Overview
> Geometry Honors is a rigorous study of shapes, space, and the logical reasoning used to prove geometric truths. Topics include Euclidean plane geometry, two- and three-dimensional figures, transformations, similarity, congruence, trigonometry, circles, and coordinate geometry. The course emphasizes **formal proofs** and abstract reasoning.

---

## 🏛️ Foundations of Geometry

### Undefined Terms
The foundation of all geometry; these terms are accepted without formal definition:
- **Point** — has no dimension; represents a location; denoted by a capital letter (e.g., point *A*)
- **Line** — has one dimension (length); extends infinitely in both directions; two points determine a line
- **Plane** — has two dimensions; extends infinitely in all directions; three non-collinear points determine a plane

### Defined Terms
- **Line Segment** — part of a line with two endpoints (AB̄)
- **Ray** — part of a line with one endpoint extending infinitely in one direction (AB⃗)
- **Angle** — formed by two rays with a common endpoint (vertex)
- **Collinear Points** — points that lie on the same line
- **Coplanar Points** — points that lie in the same plane
- **Midpoint** — point that divides a segment into two equal parts
- **Bisector** — line, ray, or segment that divides something into two equal parts

### Postulates vs. Theorems
| | Definition | Example |
|---|---|---|
| **Postulate (Axiom)** | Accepted as true without proof | Two points determine exactly one line |
| **Theorem** | Proven using postulates, definitions, and previously proven theorems | Vertical Angle Theorem |

---

## 📏 Angles & Lines

### Types of Angles

| Angle Type | Measure | Description |
|---|---|---|
| **Acute** | 0° < x < 90° | Less than a right angle |
| **Right** | Exactly 90° | Formed by perpendicular lines |
| **Obtuse** | 90° < x < 180° | Greater than right, less than straight |
| **Straight** | Exactly 180° | A straight line |
| **Reflex** | 180° < x < 360° | Greater than a straight angle |

### Angle Pairs

- **Complementary Angles** — Two angles that sum to **90°**
- **Supplementary Angles** — Two angles that sum to **180°**
- **Vertical Angles** — Opposite angles formed by two intersecting lines; **always congruent**
- **Adjacent Angles** — Share a vertex and side; do not overlap
- **Linear Pair** — Two adjacent angles forming a straight line; supplementary

### Parallel Lines Cut by a Transversal

When a transversal crosses two parallel lines, the following angle pairs are formed:

> [!info] Key Angle Relationships
> Let lines *l ∥ m* be cut by transversal *t*:

| Pair | Definition | Relationship |
|---|---|---|
| **Corresponding Angles** | Same position at each intersection | **Congruent** (≅) |
| **Alternate Interior Angles** | Between the parallel lines, opposite sides of transversal | **Congruent** (≅) |
| **Alternate Exterior Angles** | Outside the parallel lines, opposite sides | **Congruent** (≅) |
| **Co-interior (Same-side interior)** | Between parallel lines, same side of transversal | **Supplementary** (sum = 180°) |

### Proving Lines Parallel (Converses)
If any of the above relationships hold, the lines **are** parallel:
- Congruent corresponding angles → lines parallel
- Congruent alternate interior angles → lines parallel
- Supplementary co-interior angles → lines parallel

---

## 🔺 Triangles

### Classification by Sides

| Type | Description |
|---|---|
| **Scalene** | All three sides different lengths |
| **Isosceles** | Exactly two sides equal; base angles congruent |
| **Equilateral** | All three sides equal; all angles = 60° |

### Classification by Angles

| Type | Description |
|---|---|
| **Acute** | All angles less than 90° |
| **Right** | One angle exactly 90° |
| **Obtuse** | One angle greater than 90° |

### Triangle Angle Sum Theorem
> The sum of interior angles of any triangle = **180°**

### Exterior Angle Theorem
> An exterior angle of a triangle equals the sum of the two non-adjacent interior angles.

### Triangle Inequality Theorem
> The sum of any two sides of a triangle must be **greater than** the third side.
> - a + b > c
> - a + c > b
> - b + c > a

---

## 🔷 Triangle Congruence

> [!note] Two triangles are congruent (≅) if all corresponding sides and angles are equal.

### Congruence Postulates & Theorems

| Shorthand | Name | What It Requires |
|---|---|---|
| **SSS** | Side-Side-Side | All three pairs of sides congruent |
| **SAS** | Side-Angle-Side | Two sides and the **included** angle congruent |
| **ASA** | Angle-Side-Angle | Two angles and the **included** side congruent |
| **AAS** | Angle-Angle-Side | Two angles and a **non-included** side congruent |
| **HL** | Hypotenuse-Leg | Right triangles only; hypotenuse and one leg congruent |

> [!warning] NOT Valid Congruence Methods
> - **AAA** (Angle-Angle-Angle) — proves similarity, NOT congruence
> - **SSA** (Side-Side-Angle) — the "ambiguous case"; does NOT guarantee congruence

---

## 📐 Triangle Similarity

> [!note] Two triangles are similar (~) if all corresponding angles are equal and corresponding sides are proportional.

### Similarity Postulates & Theorems

| Shorthand | Name | What It Requires |
|---|---|---|
| **AA** | Angle-Angle | Two pairs of corresponding angles congruent |
| **SSS~** | Side-Side-Side Similarity | All three pairs of sides in proportion |
| **SAS~** | Side-Angle-Side Similarity | Two sides proportional and included angle congruent |

### Scale Factor
- If triangles ABC ~ DEF with scale factor k:
  - AB/DE = BC/EF = AC/DF = k
  - Perimeters ratio = k
  - Areas ratio = k²

---

## 📐 The Pythagorean Theorem

> [!success] Pythagorean Theorem
> In a **right triangle**, the square of the hypotenuse equals the sum of squares of the two legs:
> **a² + b² = c²**
> where *c* is the hypotenuse (longest side, opposite the right angle)

### Common Pythagorean Triples
| a | b | c |
|---|---|---|
| 3 | 4 | 5 |
| 5 | 12 | 13 |
| 8 | 15 | 17 |
| 7 | 24 | 25 |

And any multiples of these: 6-8-10, 9-12-15, etc.

### Converse of the Pythagorean Theorem
- If a² + b² = c² → **right** triangle
- If a² + b² > c² → **acute** triangle
- If a² + b² < c² → **obtuse** triangle

### Special Right Triangles

> [!tip] Memorize These!

**45°-45°-90° Triangle:**
- Legs: x, x
- Hypotenuse: x√2
- Example: leg = 5 → hypotenuse = 5√2

**30°-60°-90° Triangle:**
- Short leg (opposite 30°): x
- Long leg (opposite 60°): x√3
- Hypotenuse (opposite 90°): 2x
- Example: short leg = 4 → long leg = 4√3, hypotenuse = 8

---

## 📊 Quadrilaterals & Polygons

### Polygon Interior Angle Sum
> Sum of interior angles of a polygon with n sides = **(n − 2) × 180°**

| Polygon | Sides | Interior Angle Sum | Each Interior Angle (regular) |
|---|---|---|---|
| Triangle | 3 | 180° | 60° |
| Quadrilateral | 4 | 360° | 90° |
| Pentagon | 5 | 540° | 108° |
| Hexagon | 6 | 720° | 120° |
| Octagon | 8 | 1080° | 135° |
| Decagon | 10 | 1440° | 144° |
| n-gon | n | (n-2)×180° | (n-2)×180°/n |

### Exterior Angle Sum
> The sum of exterior angles of **any** convex polygon = **360°**

### Quadrilateral Hierarchy

```
Quadrilateral
└── Trapezoid (1 pair parallel sides)
    └── Isosceles Trapezoid (legs equal)
└── Parallelogram (2 pairs parallel sides)
    ├── Rectangle (4 right angles)
    │   └── Square (4 right angles + 4 equal sides)
    ├── Rhombus (4 equal sides)
    │   └── Square
    └── Square
```

### Properties of Parallelograms
A quadrilateral is a parallelogram if:
1. Both pairs of opposite sides are parallel
2. Both pairs of opposite sides are congruent
3. Both pairs of opposite angles are congruent
4. Diagonals bisect each other
5. One pair of sides is both parallel and congruent

### Special Parallelograms

| Shape | Special Properties |
|---|---|
| **Rectangle** | All angles = 90°; diagonals are congruent |
| **Rhombus** | All sides congruent; diagonals are perpendicular bisectors of each other; diagonals bisect angles |
| **Square** | All properties of rectangle + rhombus |

### Trapezoids
- **Trapezoid** — Exactly one pair of parallel sides (bases); legs are non-parallel sides
- **Isosceles Trapezoid** — Legs are congruent; base angles congruent; diagonals congruent
- **Midsegment Theorem** — Midsegment of a trapezoid is parallel to bases; length = average of bases: m = (b₁ + b₂)/2

---

## ⭕ Circles

> [!abstract] Circle Vocabulary

| Term | Definition |
|---|---|
| **Center** | The fixed point equidistant from all points on the circle |
| **Radius (r)** | Distance from center to any point on circle |
| **Diameter (d)** | Chord through center; d = 2r |
| **Chord** | Segment with both endpoints on circle |
| **Secant** | Line that intersects circle at two points |
| **Tangent** | Line that touches circle at exactly one point (point of tangency) |
| **Arc** | Part of the circle's circumference |
| **Central Angle** | Angle formed at center; equals intercepted arc measure |
| **Inscribed Angle** | Angle formed by two chords with vertex on circle |
| **Sector** | "Pie slice" — region bounded by two radii and an arc |
| **Segment** | Region bounded by a chord and an arc |

### Circle Formulas

| Measurement | Formula |
|---|---|
| **Circumference** | C = 2πr = πd |
| **Area** | A = πr² |
| **Arc Length** | L = (θ/360°) × 2πr |
| **Sector Area** | A = (θ/360°) × πr² |

### Inscribed Angle Theorem
> An inscribed angle is **half** the central angle that intercepts the same arc.
> - Inscribed angle = (1/2) × intercepted arc

**Corollaries:**
- All inscribed angles that intercept the same arc are congruent
- Inscribed angle in a semicircle = 90° (Thales' Theorem)

### Tangent-Chord Angle
> Angle = (1/2) × intercepted arc

### Angles Formed by Two Chords (Inside Circle)
> Angle = (1/2)(arc₁ + arc₂)

### Angles Formed by Two Secants/Tangents (Outside Circle)
> Angle = (1/2)|arc₁ − arc₂|

### Power of a Point (Chord-Chord)
> If two chords intersect inside a circle: **a × b = c × d**
> (product of segments of one chord = product of segments of other)

### Tangent-Secant from External Point
> tangent² = external × whole secant

---

## 📏 Area & Perimeter Formulas

| Shape | Perimeter | Area |
|---|---|---|
| Square (side s) | P = 4s | A = s² |
| Rectangle (l × w) | P = 2l + 2w | A = lw |
| Triangle (base b, height h) | P = a + b + c | A = ½bh |
| Parallelogram | P = 2a + 2b | A = bh |
| Trapezoid | P = a + b₁ + b₂ + c | A = ½(b₁ + b₂)h |
| Circle | C = 2πr | A = πr² |
| Regular Polygon (n sides, s side, a apothem) | P = ns | A = ½aP |

### Heron's Formula (Triangle, given all 3 sides)
> s = (a + b + c)/2 (semi-perimeter)
> A = √[s(s−a)(s−b)(s−c)]

---

## 🧊 3D Geometry: Surface Area & Volume

### Prisms & Cylinders

| Shape | Lateral Area | Total Surface Area | Volume |
|---|---|---|---|
| Prism | LA = Ph | SA = LA + 2B | V = Bh |
| Cylinder | LA = 2πrh | SA = 2πrh + 2πr² | V = πr²h |

*P = perimeter of base, B = area of base, h = height*

### Pyramids & Cones

| Shape | Lateral Area | Total Surface Area | Volume |
|---|---|---|---|
| Pyramid | LA = ½Pl | SA = LA + B | V = ⅓Bh |
| Cone | LA = πrl | SA = πrl + πr² | V = ⅓πr²h |

*l = slant height*

### Sphere

| Measurement | Formula |
|---|---|
| **Surface Area** | SA = 4πr² |
| **Volume** | V = (4/3)πr³ |

### Cavalieri's Principle
> If two solids have equal heights and equal cross-sectional areas at every height, they have equal volumes.

---

## 🔄 Transformations

> [!info] Types of Transformations
> A **transformation** moves or changes a figure. The original figure is the **pre-image**; the result is the **image**.

### Rigid (Isometric) Transformations — Preserve size and shape

**Translation (Slide):**
- Moves every point the same distance in the same direction
- Notation: (x, y) → (x + a, y + b)
- Preserves: size, shape, orientation

**Reflection (Flip):**
- Flips figure over a line (line of reflection)
- Common reflections:
  - Over x-axis: (x, y) → (x, −y)
  - Over y-axis: (x, y) → (−x, y)
  - Over y = x: (x, y) → (y, x)
  - Over y = −x: (x, y) → (−y, −x)
- Preserves: size, shape; reverses orientation

**Rotation:**
- Turns figure around a point (center of rotation) by an angle
- Common rotations (counterclockwise, about origin):
  - 90°: (x, y) → (−y, x)
  - 180°: (x, y) → (−x, −y)
  - 270°: (x, y) → (y, −x)
- Preserves: size, shape, orientation

### Non-Rigid Transformations — Change size

**Dilation:**
- Enlarges or shrinks figure by scale factor k from center of dilation
- (x, y) → (kx, ky) (when center is origin)
- If k > 1: enlargement; 0 < k < 1: reduction; k < 0: dilation with reflection
- Preserves: shape and angle measures; changes size

### Symmetry
- **Line Symmetry (Reflective)** — Figure maps onto itself when reflected over a line
- **Rotational Symmetry** — Figure maps onto itself when rotated less than 360°; order = number of positions

---

## 📍 Coordinate Geometry

### Distance Formula
> Distance between (x₁, y₁) and (x₂, y₂):
> **d = √[(x₂−x₁)² + (y₂−y₁)²]**
> (Derived from Pythagorean Theorem)

### Midpoint Formula
> Midpoint of segment from (x₁, y₁) to (x₂, y₂):
> **M = ((x₁+x₂)/2, (y₁+y₂)/2)**

### Slope Formula
> **m = (y₂−y₁)/(x₂−x₁)**

| Relationship | Slopes |
|---|---|
| Parallel lines | Slopes equal: m₁ = m₂ |
| Perpendicular lines | Slopes are negative reciprocals: m₁ × m₂ = −1 |
| Horizontal line | Slope = 0 |
| Vertical line | Slope = undefined |

### Equations of Lines
| Form | Equation | Notes |
|---|---|---|
| **Slope-Intercept** | y = mx + b | m = slope, b = y-intercept |
| **Point-Slope** | y − y₁ = m(x − x₁) | given slope and a point |
| **Standard** | Ax + By = C | integers; A > 0 |

### Equation of a Circle
> Center (h, k), radius r:
> **(x − h)² + (y − k)² = r²**

---

## 📐 Trigonometry (Right Triangle Trig)

> [!tip] SOH-CAH-TOA
> For a right triangle with angle θ:
> - **Sin θ = Opposite / Hypotenuse**
> - **Cos θ = Adjacent / Hypotenuse**
> - **Tan θ = Opposite / Adjacent**
>
> Memory aid: **S**ome **O**ld **H**ippo **C**aught **A** **H**ippopotamus **T**ossing **O**ranges **A**round

### Inverse Trig Functions
Used to find angles when side lengths are known:
- θ = sin⁻¹(opp/hyp) = arcsin(opp/hyp)
- θ = cos⁻¹(adj/hyp) = arccos(adj/hyp)
- θ = tan⁻¹(opp/adj) = arctan(opp/adj)

### Common Trig Values

| Angle | Sin | Cos | Tan |
|---|---|---|---|
| 0° | 0 | 1 | 0 |
| 30° | 1/2 | √3/2 | 1/√3 = √3/3 |
| 45° | √2/2 | √2/2 | 1 |
| 60° | √3/2 | 1/2 | √3 |
| 90° | 1 | 0 | undefined |

### Angles of Elevation & Depression
- **Angle of Elevation** — angle measured upward from horizontal to an object above
- **Angle of Depression** — angle measured downward from horizontal to an object below
- Both are measured from the horizontal; used with SOH-CAH-TOA to find distances or heights

### Law of Sines (Non-Right Triangles)
> **a/sin A = b/sin B = c/sin C**

Use when: AAS, ASA, or SSA (ambiguous case)

### Law of Cosines (Non-Right Triangles)
> **c² = a² + b² − 2ab·cos C**
> (Can rearrange for a² or b²)

Use when: SAS or SSS

---

## 📝 Geometric Proofs

> [!info] Types of Proofs
> - **Two-Column Proof** — Statements in one column, reasons in another
> - **Paragraph Proof** — Written in full sentences
> - **Flow Proof** — Uses arrows to show logical flow

### Common Proof Reasons

| Reason | When Used |
|---|---|
| **Given** | Information stated in the problem |
| **Definition of ___** | Using the meaning of a defined term |
| **Reflexive Property** | A = A; a segment/angle is ≅ to itself |
| **Symmetric Property** | If A = B, then B = A |
| **Transitive Property** | If A = B and B = C, then A = C |
| **Addition/Subtraction Property** | Adding or subtracting equal quantities |
| **Multiplication/Division Property** | Multiplying or dividing equal quantities |
| **Substitution Property** | Replacing with equal value |
| **Segment Addition Postulate** | If B is between A and C, then AB + BC = AC |
| **Angle Addition Postulate** | Angles can be added |
| **Vertical Angles Theorem** | Vertical angles are ≅ |
| **Alternate Interior Angles Theorem** | Parallel lines → alt. int. ∠s ≅ |
| **CPCTC** | Corresponding Parts of Congruent Triangles are Congruent |

### CPCTC Strategy
1. Prove triangles congruent (SSS, SAS, ASA, AAS, HL)
2. Then conclude specific parts are congruent using CPCTC

---

## 🔢 Key Theorems Summary

> [!tip] Must-Know Theorems

1. **Triangle Angle Sum** — Angles sum to 180°
2. **Exterior Angle Theorem** — Exterior angle = sum of remote interior angles
3. **Isosceles Triangle Theorem** — Base angles are congruent; converse also true
4. **Mid-segment Theorem** — Triangle midsegment parallel to base; length = ½ base
5. **Pythagorean Theorem** — a² + b² = c²
6. **Inscribed Angle Theorem** — Inscribed angle = ½ central angle (same arc)
7. **Thales' Theorem** — Angle inscribed in semicircle = 90°
8. **Parallel Lines Proportionality Theorem** — If a line is parallel to one side of a triangle and intersects the other two sides, it divides them proportionally
9. **Angle Bisector Theorem** — Bisector of an angle divides opposite side proportionally to adjacent sides
10. **Perpendicular Bisector Theorem** — Any point on perp. bisector is equidistant from endpoints; converse also true

---

## 🔗 Internal Links
- [[AP US History 2]]
- [[Health 2 Drivers Ed]]
- [[Chemistry Honors]]
- [[IB Design Technology 1]]
- [[Intro to Engineering Design]]
- [[Mandarin 2]]

---

*Last updated: 2025 | Aligned with Common Core State Standards for Mathematics*

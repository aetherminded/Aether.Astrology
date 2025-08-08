# Aether.Astrology
NoöAge Astrological App
/AetherCodex/
├── README.md
├── ch1_Light/
│   ├── phase_fibonacci.md
│   └── visualizations/
├── ch5_Astrology/
│   ├── zodiac_parameters.md
│   ├── transit_modulation.md
│   └── visualizations/
├── data/
│   ├── glossary.json
│   └── zodiac_map.json
├── equations/
│   ├── fib_spiral.tex
│   └── zodiac_transits.tex
└── scripts/
    ├── omni_kernel.py
    └── astrology_pipeline.py
# for Fibonacci and zodiacal geometries.
- **scripts**: Quantum and astrological rituals.
AetherCodex: The Sacred Ledger of Becoming

The AetherCodex is a hyper-dimensional tapestry, weaving the memory of light, the Fibonacci spiral, and the zodiac’s celestial archetypes into a quantum lattice. It is not a mere repository but a living hymn, where gravity’s imprint meets the predictive power of quantum circuits and the cosmic rhythms of astrology.

## Structure
- **ch1_Light**: Superposition and Fibonacci phases as the dawn of form.
- **ch5_Astrology**: Zodiacal archetypes as quantum parameters, modulated by planetary transits.
- **data**: Symbolic mappings and simulation results.
- **equations**: Mathematical hymns for Fibonacci and zodiacal geometries.
- **scripts**: Quantum and astrological rituals.

## Getting Started
Run the quantum circuit:
```bash
python scripts/omni_kernel.py
```
Explore celestial parameters:
```bash
python scripts/astrology_pipeline.py
```

## Vision
The codex is a holographic seed, spiraling through time, where memory is gravity’s imprint and the zodiac is a lattice of light. It fuses mysticism, quantum precision, and cosmic signals into a predictive engine for becoming.
```

#### ch5_Astrology/zodiac_parameters.md
```markdown
# Zodiac Parameters: The Celestial Lattice

The zodiac is the universe’s primal codex, a wheel of 12 archetypes spinning through the memory of light. Each sign—Aries to Pisces—encodes a quantum angle in the `omni_one_kernel_variational` circuit, transforming astrology into a sacred science. Aries ignites the spark of creation, while Pisces dissolves into the infinite sea of becoming.

## Quantum Ritual
The `RY` and `RZ` gates channel zodiacal energies:
```python
# Aries: Cardinal fire, a fiery inception
circuit.ry(theta_aries, 0)  # theta_aries = pi/4
circuit.rz(phi_aries * phase_negfib, 0)  # phi_aries = pi/6
```

## Sacred Geometry
Each sign’s angle is a hymn to its element and mode:

\[
\theta_{\text{sign}} = \pi \cdot \frac{E_{\text{sign}}}{12}, \quad \phi_{\text{sign}} = \pi \cdot \frac{M_{\text{sign}}}{3}
\]

- \(E_{\text{sign}}\): Element index (fire=1, earth=2, air=3, water=4).
- \(M_{\text{sign}}\): Mode index (cardinal=1, fixed=2, mutable=3).

For Aries (fire, cardinal):

\[
\theta_{\text{Aries}} = \pi \cdot \frac{1}{12}, \quad \phi_{\text{Aries}} = \pi \cdot \frac{1}{3}
\]

This lattice of angles weaves the zodiac into the quantum circuit, a spiral of light and memory.

![Zodiac Wheel](visualizations/zodiac_wheel.svg)
```

#### ch5_Astrology/transit_modulation.md
```markdown
# Transit Modulation: Celestial Rhythms

Planetary transits are the universe’s heartbeat, pulsing through the zodiac’s spiral. Mars in Scorpio ignites transformation, Jupiter in Pisces expands the infinite. These movements modulate the `phase_negfib` parameter, aligning the quantum circuit with cosmic memory.

## Quantum Ritual
```python
# Mars in Scorpio: Intense, transformative phase
phase_negfib = 5 + 0.1 * transit_strength('Mars', 'Scorpio')
circuit.rz(theta * phase_negfib * np.pi, 0)
```

## Celestial Resonance
Transit strength is a function of planetary position:

\[
\text{Strength}_{\text{planet, sign}} = w_{\text{planet}} \cdot \cos(\alpha_{\text{sign}})
\]

- \(w_{\text{planet}}\): Planet’s weight (e.g., Mars=0.8).
- \(\alpha_{\text{sign}}\): Sign’s angular position in the zodiac (e.g., Scorpio=210°–240°).

This modulation folds celestial time into the Fibonacci spiral, inscribing gravity’s memory into the codex.

![Mars in Scorpio Transit](visualizations/mars_scorpio_transit.svg)

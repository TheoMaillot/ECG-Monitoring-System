# Flexible ECG Electrode Fabrication Process

Complete cleanroom microfabrication process for gold/PEDOT electrodes on flexible Kapton substrate.

## Materials

- **Substrate**: Kapton polyimide film (50μm thickness)
- **Conductive layer**: 5nm Cr (adhesion) + 150nm Au
- **Biocompatible coating**: PEDOT:PSS polymer
- **Photoresist**: S1813 positive resist

## Process Flow

### Day 1: Photolithography

**1. Substrate Preparation**
- Mount Kapton on glass carrier using Kapton tape
- Clean with DI water and acetone
- O₂ plasma activation (Oxford Plasma Etch) - improves resist adhesion

<img src="photos/substrate-prep.jpg" width="500">

**2. Resist Coating**
- Spin-coat S1813 photoresist @ 1500 rpm
- Target thickness: ~1.5μm
- Soft bake: 110°C

**3. UV Exposure**
- Mask alignment (WEC compensation critical)
- UV exposure time: [specify your time]
- Development in MF26 developer

<img src="photos/after-development.jpg" width="500">

*Electrode pattern after resist development (microscope view)*

**Initial Resistance Measurements**:
- Electrode #1: 22.4Ω
- Electrode #2: 16.0Ω

---

### Day 2: Metallization

**4. Metal Evaporation**
- Chromium adhesion layer: 5nm
- Gold conductive layer: 100nm
- Vacuum level: <10⁻⁶ mbar
- Deposition rate: ~0.5Å/s

**5. Lift-off**
- Acetone/IPA bath with ultrasonication
- Reveals metal pattern only on exposed areas
- Careful cleaning to remove residues

<img src="photos/after-liftoff.jpg" width="500">

*Gold electrodes after lift-off process*

**6. PEDOT Coating**
- Spin-coat PEDOT:PSS solution
- Annealing: 150°C
- Creates low-impedance bio-interface

<img src="photos/pedot-annealing.jpg" width="500">

**Post-PEDOT Resistance**:
- Electrode #1: 20.8Ω (↓ 7%)
- Electrode #2: 15.2Ω (↓ 5%)

---

### Day 3: Characterization

**7. Wire Bonding**
- Connect thin wires using conductive epoxy
- Cure at room temperature

**8. Impedance Spectroscopy**
- Equipment: VMP-3e potentiostat
- Frequency range: 10 Hz - 100 kHz
- Test electrolyte: PBS solution

<img src="photos/impedance-comparison.jpg" width="600">

*Nyquist plot: Custom electrodes (green) vs commercial (purple)*

## Results

### Key Findings

**Lower impedance** than commercial electrodes in 10-100 Hz range (cardiac signal band)  
**Irregular Nyquist curve** indicates:
- PEDOT layer inhomogeneities
- Multiple interface effects (Au/PEDOT/electrolyte)
- Micro-defects from manual processing

### Performance Metrics

| Parameter | Value | Notes |
|-----------|-------|-------|
| Base resistance | 15-22Ω | Before PEDOT |
| Final resistance | 15-21Ω | After PEDOT |
| Impedance @ 50Hz | ~30% lower | vs. commercial |
| Active area | [specify] mm² | Gold contact area |

## Process Challenges

**Critical Steps**:
1. **Kapton mounting**: Eliminate all air bubbles (affects uniformity)
2. **Mask alignment**: WEC adjustment requires practice
3. **PEDOT application**: Manual spin-coating creates thickness variations
4. **Lift-off**: Aggressive sonication risks damaging thin features

## Improvements for Next Iteration

1. **Automated PEDOT deposition** (spray coating or inkjet)
2. **Thicker gold layer** (200nm) for better conductivity
3. **Post-anneal** gold layer before PEDOT to improve interface
4. **Encapsulation layer** for long-term stability

---

## Equipment Used

- Oxford Plasma Etcher
- Spin Coater (1500 rpm capability)
- Mask Aligner (UV exposure)
- Thermal Evaporator
- VMP-3e Potentiostat
- Optical Microscope

## Safety Notes

⚠️ **Cleanroom protocols**: Full bunny suit, no skin contact with substrates  
⚠️ **Chemical handling**: Acetone/IPA under fume hood  
⚠️ **UV exposure**: Eye protection mandatory during mask alignment

---

**Total Fabrication Time**: 3 days (6-8 hours per session)  
**Yield**: 2/2 functional electrodes (100%)  
**Cost per electrode**: ~€5-10 in materials
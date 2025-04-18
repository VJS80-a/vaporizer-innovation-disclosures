# Spiral & Multi‑Foil Heater – Comprehensive Technical Disclosure

**Date of Disclosure:** 2025-04-18  
**Inventor:** Ville Johannes Savolainen  
**Disclosure Type:** Public Prior Art

---

## 1. Background

A thin‑foil spiral heater has been employed in compact herbal vaporizers marketed under the Ti N YM ig ht brand since 2019.  
The heater is typically fabricated from **0.05 mm stainless‑steel foil**, although other thicknesses can be selected to meet power and geometry targets.

---

## 2. Core Heater Construction

| Element | Typical Implementation | Variations / Options |
|---------|------------------------|----------------------|
| **Foil** | Stainless‑steel sheet (≈0.05 mm) | Other metals & thicknesses |
| **Central Support** | Steel or SS **rod / axle**; foil spot‑welded to it | Omitted entirely; replaced by high‑conductivity wire; stamped foil tongue |
| **Spiral Formation** | Foil is rolled into a spiral so layers do **not touch**, creating a controlled air gap | Non‑spiral geometries possible (e.g., concentric rings) |
| **Electrical Path** | Current flows from the centre conductor → through spiral → to outer termination (e.g., spot‑welded nickel strip) | Silver or copper wire, laser‑welded lugs, conductive adhesive, soldered joints, shaped foil ends |

### 2.1 Maintaining Spiral Spacing & Shape

1. **Perforated‑foil + Rods (most common)**  
   *Holes* are laser‑cut so that, once rolled, **zirconia ceramic rods** pass through and lock layer spacing.  
   • Simple assembly • Robust under heat cycles.

2. **Heat‑Setting in Moulds**  
   Foil is rolled inside a **spacing jig / mould**, heat‑treated to memorise shape, jig removed.

3. **Sacrificial Spacers**  
   Temporary spacers inserted during rolling; removed **mechanically**, **thermally** (burn‑off), or **chemically** (etch‑out), then permanent rods inserted.

### 2.2 Geometry Tweaks

- **Variable hole pitch** → variable layer height along the spiral.  
- **Foil width modulation** → local resistance / heat profile tailoring.

---

## 3. Tube vs. Self‑Supporting Structure

| Approach | Description | Pros |
|----------|-------------|------|
| **External Tube** | Spiral inserted into glass, ceramic or metal tube | Simple assembly; rigid containment |
| **Self‑Wrapping Foil Tube** | Foil is **left longer**, then rolled 3‑4 extra turns to form its **own 0.15–0.25 mm shell** | • Eliminates extra part • Lighter • Lower thermal mass • Adjustable heat leakage |

Thin foil stores little energy; any ingress of cool intake air rapidly removes residual heat, keeping device surfaces cool and blocking IR radiation.

---

## 4. Alternative Conductor & Termination Options

- Replace central rod with **high‑conductivity wire** (Cu/Ag) or stamped foil tongue.  
- Outer termination via **laser weld**, **press‑fit clamp**, **conductive epoxy**, or shaping foil ends into tabs.

---

## 5. Dual / Multi‑Foil Spiral Heater

### 5.1 Concept

Two (or more) thinner foils are rolled together inside the same heater volume.

| Parameter                  | Single‑Foil (Ref) | Dual‑Foil Example |
|----------------------------|-------------------|-------------------|
| Foil thickness             | 0.05 mm           | 0.025 mm × 2      |
| Surface area               | 1×                | **2×**            |
| Nominal power (3.7 V)      | 70 W @ 20 A       | 70 W @ 10 A/foil  |

### 5.2 Advantages

- **Lower peak current** → less battery sag & ageing.  
- **Dynamic power control**: run one foil for ≤ 50 % demand; both for high demand.  
- **Better thermal uniformity** with doubled surface area.  
- Potential for **dual‑temperature zones** using mismatched foil thicknesses.

### 5.3 Electrical Control Strategies

1. **Independent Drive** (preferred)  
   - Foils welded together at the centre; **separate conductors** at the outer ends.  
   - Individual MOSFETs & PWM channels minimise overlap time.

2. **Parallel Drive** (simpler)  
   - Foils tied to same potential; controller sees one large heater.

3. **Mid‑Spiral Tap Variant**  
   - Add **mid‑spiral conductor**; drive inner section, outer section, or both for three power levels.

### 5.4 Isolation & Assembly

- Ensure outer foil ends **do not short**: use ceramic paste, mica washers, or spatial separation.  
- Spot‑, laser‑ or resistive‑weld foils together where conductive coupling is desired.

---

## 6. Thermal & Efficiency Considerations

- Thin‑wall self‑supporting shell **reduces conduction / radiation losses**.  
- High reflectivity of stainless foil blocks IR to device body.  
- Larger surface area in dual‑foil version **improves heat transfer** to airflow.

---

## 7. Summary & Intent

This document discloses multiple heater constructions—single‑foil, self‑supporting, and dual‑foil spiral designs—along with alternative assembly, electrical, and power‑control methods. The goal is to place these innovations in the public domain as **prior art**, preventing exclusive patent claims by third parties.


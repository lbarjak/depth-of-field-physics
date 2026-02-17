# Depth of Field Equivalence Table

## Equivalent Settings for Identical Depth of Field Across Different Formats

**Reference:** Full Frame 35mm system, normal lens, **f/1.4** aperture  
**Entrance Pupil Diameter:** **30.9 mm** (calculated from exact diagonal: 43.3mm / 1.4, constant across all formats for equivalent DOF)

**Assumptions:** Equivalent framing (same subject, same distance), normal lenses (focal length ≈ format diagonal), and standard CoC convention (CoC proportional to format size, i.e., same final print size viewed from the same distance).

| Format | Size (mm) | Diagonal (mm) | Normal Lens (mm) | **Equivalent f-number** | Aperture Ø (mm) | CoC (mm) |
|--------|-----------|---------------|------------------|-------------------------|-----------------|----------|
| **1" sensor** | 8.8 × 13.2 | 15.9 | 16 | **f/0.5** | 30.9 | 0.011 |
| **Micro Four Thirds** | 13.0 × 17.3 | 21.6 | 22 | **f/0.7** | 30.9 | 0.015 |
| **APS-C Canon** | 14.8 × 22.2 | 26.7 | 27 | **f/0.9** | 30.9 | 0.018 |
| **APS-C Nikon** | 15.7 × 23.6 | 28.4 | 28 | **f/0.9** | 30.9 | 0.020 |
| **Full Frame 35mm** | 24 × 36 | 43.3 | 43 | **f/1.4** | 30.9 | 0.030 |
| **Medium Format 645** | 41.5 × 56 | 69.7 | 70 | **f/2.3** | 30.9 | 0.048 |
| **Medium Format 6×6** | 56 × 56 | 79.2 | 79 | **f/2.6** | 30.9 | 0.055 |
| **Medium Format 6×7** | 56 × 70 | 89.6 | 90 | **f/2.9** | 30.9 | 0.062 |
| **Medium Format 6×9** | 56 × 84 | 101.1 | 101 | **f/3.3** | 30.9 | 0.070 |
| **4×5 inch** | 102 × 127 | 163.2 | 163 | **f/5.3** | 30.9 | 0.113 |
| **5×7 inch** | 127 × 178 | 219.2 | 219 | **f/7.1** | 30.9 | 0.151 |
| **8×10 inch** | 203 × 254 | 325.4 | 325 | **f/10.5** | 30.9 | 0.225 |
| **11×14 inch** | 279.4 × 355.6 | 453.0 | 453 | **f/14.7** | 30.9 | 0.313 |

**CoC values** are calculated as: CoC = diagonal / 1450, which is the standard convention assuming an 8×10" (20×25cm) print viewed from ~25cm. The 35mm baseline of 0.030mm is widely used in the photographic industry.

## Calculation Method

1. **Normal Lens** = Format diagonal (mm), rounded to nearest practical value
2. **Entrance Pupil Diameter** = Focal Length / f-number
3. **For Equivalent DOF** = Constant entrance pupil diameter (30.9mm)
4. **f-number** = Normal lens focal length / 30.9mm
5. **CoC** = Format diagonal / 1450

## Why This Works

When comparing formats with equivalent framing (same subject at same distance) and proportionally scaled CoC, the hyperfocal distance simplifies to:

```
H = f × D / c = diagonal × D / (diagonal / 1450) = 1450 × D
```

The format diagonal cancels out completely. The depth of field depends only on the entrance pupil diameter `D`.

## Example

An **8×10" film camera** with an **f/5.6** normal lens has a depth of field equivalent to an **f/0.75** lens on a 35mm system:
- 8×10" @ f/5.6: aperture Ø = 325 / 5.6 = **58.0 mm**
- 35mm @ f/0.75: aperture Ø = 43.3 / 0.75 = **57.7 mm** ✓

Both have approximately the same entrance pupil diameter, therefore the same depth of field — regardless of the vast difference in format size.
# Depth of Field and Aperture Diameter Equivalence

## Why Depth of Field Depends Only on Entrance Pupil Diameter

This repository provides reference tables demonstrating that **depth of field is fundamentally determined by the physical diameter of the entrance pupil (aperture opening)**, not by the sensor size or f-number alone.

## The Physics Behind It

### The Common Misconception

Many photographers believe that depth of field varies with sensor size. This leads to statements like "full-frame cameras have less depth of field than crop sensors at the same aperture." However, this is misleading.

### The Physical Reality

**Depth of field is determined by:**
1. **Entrance pupil diameter** (aperture opening in mm)
2. **Subject distance**
3. **Circle of confusion criteria**

**Depth of field is NOT directly determined by:**
- Sensor size
- F-number alone
- Focal length alone

### Why Entrance Pupil Diameter Matters

The entrance pupil diameter is the physical size of the aperture opening as seen through the front of the lens:

```
Entrance Pupil Diameter = Focal Length / f-number
```

For example:
- **35mm system**: 43mm f/1.4 → 43 / 1.4 = **30.7mm diameter**
- **8×10" system**: 325mm f/10.5 → 325 / 10.5 = **30.9mm diameter**

Both produce **identical depth of field characteristics** because the physical aperture diameter is the same.

### The Role of Sensor Size

Sensor size affects depth of field **indirectly** through focal length requirements:
- Larger sensors require longer focal lengths for the same field of view
- Longer focal lengths require larger f-numbers to maintain the same entrance pupil diameter
- Therefore, larger formats appear to have "shallower" depth of field at equivalent compositions

### Mathematical Proof

The hyperfocal distance formula shows the relationship:

```
H = f² / (N × c)
```

Where:
- `H` = hyperfocal distance
- `f` = focal length
- `N` = f-number
- `c` = circle of confusion

Rearranging:

```
H = f² / (N × c) = f × (f/N) / c = f × D / c
```

Where `D = f/N` is the entrance pupil diameter.

For a "normal" lens where `f ≈ diagonal`, the depth of field becomes primarily dependent on `D/c` ratio.

## Practical Implications

### Example: 35mm f/1.4 Equivalence

The table below shows what f-number is required on different formats to achieve the **same depth of field** as a 35mm full-frame camera with a normal lens at **f/1.4** (entrance pupil diameter: 30.9mm).

| Format | Sensor Size (mm) | Diagonal (mm) | Normal Lens (mm) | **Equivalent f-number** | Aperture Ø (mm) |
|--------|------------------|---------------|------------------|-------------------------|-----------------|
| **Full Frame 35mm** | 24 × 36 | 43.3 | 43 | **f/1.4** | 30.9 |
| **Medium Format 6×7** | 56 × 70 | 89.6 | 90 | **f/2.9** | 30.9 |
| **4×5 inch** | 102 × 127 | 163.2 | 163 | **f/5.3** | 30.9 |
| **8×10 inch** | 203 × 254 | 325.4 | 325 | **f/10.5** | 30.9 |

### Real-World Observation

A classic **8×10" view camera** with a typical normal lens (325mm) at **f/5.6** has an entrance pupil diameter of:

```
325mm / 5.6 = 58.0mm
```

This corresponds to a 35mm full-frame equivalent of:

```
43mm / 58.0mm ≈ f/0.74
```

This explains why large format photography requires such small apertures (f/16, f/22, f/32) to achieve adequate depth of field – the physical aperture diameter must be reduced to compensate for the longer focal lengths.

## Reference Tables

See the full equivalence tables:
- [CSV format](depth-of-field-equivalence.csv)
- [Markdown table](depth-of-field-equivalence.md)

## Calculation Method

1. **Normal lens focal length** = Format diagonal (mm)
2. **Entrance pupil diameter** = Focal length / f-number
3. **For equivalent depth of field** = Same entrance pupil diameter (30.9mm)
4. **Equivalent f-number** = Normal lens focal length / 30.9mm

## References

- *The Manual of Photography* - 10th Edition, Focal Press
- *Applied Photographic Optics* - Sidney F. Ray
- *View Camera Technique* - Leslie Stroebel

## License

This data is provided for educational purposes. Feel free to use and modify.

---

**Note**: This analysis assumes "normal" lenses (focal length ≈ diagonal), equivalent framing, and identical circle of confusion criteria adjusted for viewing distance and format size.
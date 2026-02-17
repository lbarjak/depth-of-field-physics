# Depth of Field and Aperture Diameter Equivalence

## Why Depth of Field Depends on Entrance Pupil Diameter

This repository provides reference tables demonstrating that **depth of field is fundamentally determined by the physical diameter of the entrance pupil (aperture opening)**, given equivalent framing and standard viewing conditions — not by the sensor size or f-number alone.

## The Physics Behind It

### The Common Misconception

Many photographers believe that depth of field varies with sensor size. This leads to statements like "full-frame cameras have less depth of field than crop sensors at the same aperture." However, this is misleading.

When comparing images with **the same subject framing** (e.g., a half-body portrait), what actually determines the depth of field is the physical size of the aperture opening — the entrance pupil diameter.

### The Physical Reality

**Depth of field is determined by:**
1. **Entrance pupil diameter** (aperture opening in mm)
2. **Subject distance**
3. **Circle of confusion criteria** (which depends on format size and viewing conditions)

When comparing across formats with **equivalent framing** (same subject at same distance) and **standard viewing conditions** (same final print size viewed from the same distance), the circle of confusion scales proportionally with the format size, and subject distance is the same. Under these standard photographic conditions, depth of field becomes a function of the entrance pupil diameter alone.

**Depth of field is NOT directly determined by:**
- Sensor size (it acts indirectly through focal length requirements)
- F-number alone (it must be combined with focal length)
- Focal length alone (it must be combined with f-number)

### Why Entrance Pupil Diameter Matters

The entrance pupil diameter is the physical size of the aperture opening as seen through the front of the lens:

```
Entrance Pupil Diameter = Focal Length / f-number
```

For example:
- **35mm system**: 43mm f/1.4 → 43 / 1.4 = **30.7mm diameter**
- **8×10" system**: 325mm f/10.5 → 325 / 10.5 = **31.0mm diameter**

Both produce **nearly identical depth of field characteristics** because the physical aperture diameter is essentially the same (~30.9mm, using the exact diagonal values).

### The Role of Sensor Size

Sensor size affects depth of field **indirectly** through focal length requirements:
- Larger sensors require longer focal lengths for the same field of view
- Longer focal lengths require larger f-numbers to maintain the same entrance pupil diameter
- Therefore, larger formats appear to have "shallower" depth of field at equivalent compositions

### The Role of Circle of Confusion (CoC)

The circle of confusion is the maximum acceptable blur spot diameter on the sensor/film that still appears "sharp" in the final image. It is **not a physical constant** but a perceptual criterion that depends on:

- **Format size** — larger formats require less enlargement to reach the same print size
- **Final print/display size** — larger prints demand tighter sharpness criteria
- **Viewing distance** — farther viewing distances are more forgiving

Under the **standard photographic convention** — where all formats are enlarged to the same final print size and viewed from the same distance — the CoC scales proportionally with the format diagonal. For example:
- 35mm: CoC ≈ 0.030mm (requires ~8× enlargement for a 24×30cm print)
- 8×10": CoC ≈ 0.225mm (requires minimal enlargement for the same print)
- Ratio: 0.225 / 0.030 ≈ 7.5 ≈ 325 / 43 ✓

This proportional scaling is what allows the format size to cancel out of the depth of field equations.

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

For a "normal" lens where `f ≈ diagonal`, and using the standard convention where `c ∝ diagonal`:

```
H = diagonal × D / (k × diagonal) = D / k
```

The format diagonal cancels out completely, and the hyperfocal distance depends **only** on the entrance pupil diameter `D` and the constant `k` (which encodes the viewing conditions). This is why, under equivalent framing and standard viewing, depth of field is determined by the entrance pupil diameter.

## Practical Implications

### Example: 35mm f/1.4 Equivalence

The table below shows what f-number is required on different formats to achieve the **same depth of field** as a 35mm full-frame camera with a normal lens at **f/1.4** (entrance pupil diameter: 30.9mm, calculated from the exact diagonal 43.3 / 1.4).

| Format | Sensor Size (mm) | Diagonal (mm) | Normal Lens (mm) | **Equivalent f-number** | Aperture Ø (mm) |
|--------|------------------|---------------|------------------|-------------------------|----------------- |
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
43.3mm / 58.0mm ≈ f/0.75
```

This explains why large format photography requires such small apertures (f/16, f/22, f/32) to achieve adequate depth of field – the physical aperture diameter must be reduced to compensate for the longer focal lengths.

## Reference Tables

See the full equivalence tables:
- [CSV format](depth-of-field-equivalence.csv)
- [Markdown table](depth-of-field-equivalence.md)

## Calculation Method

1. **Normal lens focal length** = Format diagonal (mm), rounded to nearest practical value
2. **Entrance pupil diameter** = Focal length / f-number
3. **For equivalent depth of field** = Same entrance pupil diameter (30.9mm, from 43.3mm / f/1.4)
4. **Equivalent f-number** = Normal lens focal length / 30.9mm

## Assumptions

This analysis is valid under the following standard photographic conditions:

1. **"Normal" lenses** — focal length approximately equal to the format diagonal
2. **Equivalent framing** — the same subject (e.g., a half-body portrait) fills the frame similarly on all formats, implying the same subject distance
3. **Standard CoC convention** — the circle of confusion scales proportionally with format size, corresponding to all formats being enlarged to the same final print/display size and viewed from the same distance
4. **Geometrical optics** — diffraction effects are not considered (relevant at very small apertures)

## References

- *The Manual of Photography* - 10th Edition, Focal Press
- *Applied Photographic Optics* - Sidney F. Ray
- *View Camera Technique* - Leslie Stroebel

## License

This data is provided for educational purposes. Feel free to use and modify.
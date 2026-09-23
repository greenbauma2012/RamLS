# 1999 Ram 1500 A/C + LS Swap Implementation

## Overview
Complete A/C system integration for LS-swapped 1999 Ram 1500 using OEM Ram compressor with truck-spacing LS accessories and Kwik Performance bracket.

---

## 1. Bracket & Compressor Setup

### Bracket Specifications
- **Model:** Kwik Performance LS Truck Sanden A/C Bracket
- **Design:** Truck-spacing LS accessory mount
- **Compatibility:** Accepts Sanden SD7H15 bolt pattern
- **Frame Clearance:** Clears Ram frame rails with Speed Engineering slider mounts
- **Price:** ~$225–$260

### Compressor
- **Source:** 1999 Ram 1500 Sanden compressor (existing)
- **Type:** Fixed displacement
- **Control:** Clutch-controlled (no PWM, no variable displacement)

---

## 2. Belt Selection

### Serpentine Belt Specification
- **Part Number:** K061108
- **Length:** 110.8"
- **Routing:** LS truck crank → truck alternator → truck power steering → Sanden low-mount compressor
- **Compatibility:** Works with all truck-spacing components

---

## 3. Hose & Fitting Specifications

### Compressor-Side Fittings (LS / Sanden SD7H15)
| Function | Fitting Type | Size |
|----------|--------------|------|
| Discharge | Sanden pad fitting | #8 |
| Suction | Sanden pad fitting | #10 |

### Truck-Side Fittings (1999 Ram 1500)
| Function | Fitting Type | Size |
|----------|--------------|------|
| Discharge | Chrysler fitting | #8 |
| Suction | Chrysler fitting | #10 |

### Hose Specifications
| Component | Size | Type | Barrier |
|-----------|------|------|---------|
| High-side (discharge) | #8 | A/C hose | Barrier |
| Low-side (suction) | #10 | A/C hose | Barrier |

### Sealing Components
- **O-Rings:** HNBR green A/C O-rings
- **Sanden pad:** Standard #8/#10 O-rings
- **Chrysler fittings:** Standard #8/#10 O-rings

### Hose Procurement Options
- Local hydraulic/A/C shop (recommended)
- Cold Hose
- ACKits
- Vintage Air
- Restomod Air

### DIY Hose Making (Optional)
If fabricating your own hoses, you'll need:
- Mastercool 71550 or 71500 crimper
- Hose cutter
- Deburring tool
- Vacuum pump
- Manifold gauges

---

## 4. Hose Length Recommendations

### Initial Estimates
**Measure after mounting compressor for final confirmation**

| Component | Length Range | Notes |
|-----------|--------------|-------|
| #10 suction (low-side) | 38–44" | Length varies with slider mount position |
| #8 discharge (high-side) | 32–38" | May shift slightly depending on engine placement |

**Important:** Speed Engineering slider mounts may shift engine position. Final measurement and custom hose fabrication is strongly recommended.

---

## 5. Wiring & Electrical Control

### Compressor Characteristics
- **Displacement:** Fixed displacement
- **Control Method:** Clutch engagement/disengagement
- **PWM Control:** Not required
- **Variable Displacement Logic:** Not applicable

### Pressure Protection
- **Low-pressure switch:** Keeps OEM Ram unit
- **High-pressure switch:** Keeps OEM Ram unit
- **Control Method:** Simple clutch on/off output from aftermarket ECU

### ECU Control Strategy

#### Clutch Engagement Conditions
Engage compressor clutch when ALL conditions are met:
- A/C request is active
- Low-pressure switch is closed (sufficient pressure)
- High-pressure switch is closed (pressure within range)

#### Clutch Disengagement Conditions
Disengage compressor clutch when:
- Low-pressure switch opens (low refrigerant or charge)
- High-pressure switch opens (excessive pressure)
- A/C request turns off

**Result:** Pressure switches provide OEM-equivalent system protection

---

## 6. Refrigerant & Oil Specifications

### Oil Selection
- **Type:** PAG-100
- **Source:** 1999 Ram specification
- **Critical Warning:** Do NOT use GM PAG-46
- **Used Compressor:** If compressor is used, flush completely and refill with PAG-100

### Refrigerant Charge
- **Refrigerant Type:** R-134a
- **Charge Amount:** 32 oz (approximately 2 lbs)
- **Reference:** 1999 Ram OEM specification

### Vacuum Procedure
- **Duration:** 45–60 minutes
- **Verification:** System must hold vacuum before charging
- **Tools Required:** Vacuum pump and manifold gauges

---

## 7. System Layout Overview

### Component Integration
```
1999 Ram 1500 A/C System Components:
├── LS Engine (primary driver)
├── Kwik Performance LS Truck Sanden Bracket
├── Ram Sanden Compressor (SD7H15)
├── Speed Engineering Slider Mounts
├── Custom A/C Hoses (Sanden ↔ Chrysler adapters)
├── Ram Condenser
├── Ram Evaporator
├── Ram Accumulator/Drier
├── Ram Low-Pressure Switch
├── Ram High-Pressure Switch
├── Aftermarket ECU (clutch control output)
├── Serpentine Belt (K061108)
├── PAG-100 Oil
└── R-134a Refrigerant (32 oz)
```

### Key Design Principles
- ✅ Complete OEM Ram HVAC system retained
- ✅ Full compatibility with LS engine bay
- ✅ Truck-spacing accessory mounting
- ✅ OEM pressure switch safety protection
- ✅ Proven Sanden compressor reliability
- ✅ Standard A/C servicing capability

---

## Installation Checklist

### Pre-Installation
- [ ] Verify Kwik Performance bracket fits frame configuration
- [ ] Confirm belt length K061108 matches component layout
- [ ] Source all hose fittings and components
- [ ] Obtain vacuum pump and manifold gauges
- [ ] Prepare PAG-100 oil and R-134a refrigerant

### Bracket & Compressor Mount
- [ ] Install Speed Engineering slider mounts
- [ ] Mount Kwik Performance bracket to LS engine
- [ ] Install Ram compressor on bracket
- [ ] Install serpentine belt
- [ ] Verify compressor alignment

### Hose Installation
- [ ] Measure actual compressor-to-condenser distance
- [ ] Fabricate or order custom hoses
- [ ] Install suction hose (#10)
- [ ] Install discharge hose (#8)
- [ ] Verify fitting torque specifications

### Fluid & Charging
- [ ] Flush compressor if used; refill with PAG-100
- [ ] Pull full vacuum for 45–60 minutes
- [ ] Verify vacuum holds for 15+ minutes
- [ ] Charge system with 32 oz R-134a
- [ ] Verify pressure switch operation

### Electrical & Control
- [ ] Connect low-pressure switch to ECU input
- [ ] Connect high-pressure switch to ECU input
- [ ] Configure ECU clutch output control
- [ ] Test clutch engagement with A/C request
- [ ] Verify pressure switch safety function

### Final Testing
- [ ] Start engine and test clutch engagement
- [ ] Verify cooling performance
- [ ] Check for refrigerant leaks
- [ ] Monitor system pressures during operation
- [ ] Road test for temperature stability

---

## Notes & Considerations

### Critical Points
1. **Oil Type:** PAG-100 is specific to Ram application—not interchangeable with GM PAG-46
2. **Vacuum Time:** 45–60 minutes is minimum; longer is acceptable and more thorough
3. **Hose Measurement:** Slider mounts may shift engine; always measure before final fabrication
4. **Pressure Switches:** Retain OEM protection—critical for system longevity

### Future Service
- System is fully serviceable with standard A/C shop equipment
- Hose design allows for future replacement if needed
- Pressure switches can be replaced independently
- Compressor can be overhauled or replaced with any Sanden SD7H15 unit


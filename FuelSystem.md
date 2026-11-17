# Fuel System: 1999 Ram 1500 + LQ4 + Holley Terminator X

Items marked **VERIFY** are from memory or forum consensus and need to be measured or confirmed before buying parts.

## 1. The Problem

| Item | Value |
|------|-------|
| Truck fuel line (frame side) | 5/16" ID |
| LQ4 intake / fuel rail connection | 3/8" ID |
| Holley Terminator X (LS) base fuel pressure | ~58-60 PSI (**VERIFY** in Holley software / manual) |
| Stock Ram in-tank pump | ~52 PSI (per current notes; the Magnum regulates around 49 PSI, **VERIFY**) |
| Shortfall | ~6-8 PSI |

## 2. Comparison

| | 1999 Ram 1500 5.9 Magnum (current truck) | 2002 Yukon Denali 6.0 LQ4 (donor) | Holley Terminator X (LS) |
|---|---|---|---|
| Style | Return-style, regulator in the pump module (**VERIFY**) | Returnless, regulator/filter in the pump module | Works with either; return style with an external regulator is preferred |
| Target pressure | ~49 PSI | ~58 PSI | ~58-60 PSI base |
| Feed line | 5/16" (8 mm) | 3/8" quick-connect at the rail | 3/8" or AN-6 recommended |
| Return line | **VERIFY** (likely 5/16" or smaller) | None | AN-6 if a return is used |
| Pump | Stock in-tank, ~52 PSI max | In-tank, ~58 PSI | ~255 LPH or larger in-tank, or external |
| Rail pressure sensor | None | None | Optional, but useful |

## 3. Options

### Option A: Run the lower pressure and tell the ECU (cheapest)
- Holley scales injector pulse width off the base fuel pressure setting. It does not require exactly 60 PSI.
- Keep the stock pump and set the base pressure to the real value (~49-52 PSI), then tune.
- Add a rail pressure sensor (Holley 0-100 PSI) so the ECU can compensate if pressure drops.
- Cons: this is the least headroom. Injectors flow less at lower pressure, so a street cam plus the 6.0 may run short of fuel at high load. Watch the wideband.

### Option B: Replace the in-tank pump and use a regulator (recommended)
- Install a ~255 LPH in-tank pump (Walbro/Holley/Aeromotive) that makes more than 60 PSI.
- Add an adjustable in-line regulator near the engine and set it to 58 PSI.
- The Ram's 5/16" feed will flow enough for a mild LS. It would limit a high-power or boosted build.
- Needs a return line from the regulator back to the tank. If the Ram has none, run a new one (5/16" or AN-6).
- Cons: tank work, a return line, and cutting into the existing pump module or a new hanger.

### Option C: External high-pressure pump plus a return-style fuel line
- Add a frame-rail EFI pump (e.g. Holley Sniper or Aeromotive 340), a pre-filter, a post-filter, and a regulator. Keep the in-tank pump as a lift pump, or use a swirl pot/surge tank. Pumps must be E85-rated.
- Best for future power, but the most plumbing and wiring.

## 3a. Constraints: Dodge Tank, E85, Future Supercharger
The Yukon donor is not available, so every option must work with the Dodge tank.

**Recommended build: Option B with future-proof parts**
- Pump: in-tank, E85-rated, 340+ LPH (e.g. Aeromotive 340 Stealth, Walbro GSS342/F90000267 or Holley in-tank) installed in the Ram's stock hanger/module, or a universal in-tank pump fitted with a sock (**VERIFY** fitment for the 1999 Ram tank size, 26 vs 35 gal).
- Wiring: the pump draws more current than stock. Use a relay and a 10-12 AWG feed (Holley Terminator X can trigger the relay).
- Lines: run a new AN-6 (3/8") feed and AN-6 return along the frame instead of reusing the 5/16" lines. Use steel/stainless hard line, or PTFE-lined braided hose. Do not use rubber J30R9 hose long-term with E85.
- Regulator: return-style adjustable (e.g. Aeromotive/Holley) with a boost reference port. Set about 58 PSI base. A boost-referenced regulator raises pressure 1:1 with boost, which keeps injector flow steady with a supercharger.
- Filter: E85-compatible filters, 10 micron post-filter. Prefer stainless-element or AN-6 filters.
- Sensors: Holley rail pressure sensor and a flex-fuel (ethanol content) sensor, both wired to the Terminator X (**VERIFY** support in your Holley software version).

**E85 notes**
- E85 needs about 30-40% more fuel by volume than gasoline. Stock LQ4 injectors (about 28-30 lb/hr) will be too small. Plan for ~42-60 lb/hr injectors for E85 plus a small blower. Verify with a calculator for your target horsepower.
- All components must be E85-rated, including seals, pump, regulator, hose, and the tank (the Ram's steel/plastic tank is fine, **VERIFY** no zinc or terne coating).
- Flush the tank and lines before the first fill, since E85 can loosen old varnish and rust.

**Rough flow limits (VERIFY, rule of thumb only)**
| Line | Gasoline | E85 |
|------|----------|-----|
| 5/16" (stock) | ~350-450 hp | ~300 hp |
| AN-6 (3/8") | ~700+ hp | ~550-600 hp |

A small supercharger on an LQ4 can exceed the 5/16" limit, so replace the lines now while the swap is open.

## 4. Fittings: 5/16" to 3/8"
- Do not reduce the Holley side. Use the rail side at 3/8" or AN-6 and step up from the truck's 5/16" once near the engine.
- Adapter options:
  - 5/16" quick-connect to AN-6 (-6 is 3/8" tube size) adapter, then AN-6 to the GM 3/8" quick-connect fitting.
  - GM LS fuel rail adapter, 3/8" to AN-6 (Holley/Russell/Earls).
- The 5/16" line is fine as a section of the run. Replacing the whole line to 3/8" gives more flow margin.
- Use EFI-rated hose only (SAE J30R9 or push-lock EFI hose) and rated clamps.

## 5. Open Questions / To Measure
- [ ] Confirm the actual pressure the stock Ram pump makes at the rail (use a gauge on the Schrader port or a tee).
- [ ] Is there a return line at the Ram tank? Size?
- [ ] Which pump is in the Ram (brand/part number)?
- [ ] Confirm the Holley Terminator X base pressure setting and whether a rail pressure sensor is supported.
- [ ] Injector size and flow rate at 58 PSI vs 49 PSI (the 2002 LQ4 uses roughly 28-30 lb/hr injectors, **VERIFY**).
- [ ] Rail fitting type on the intake (3/8" quick-connect, GM "spring lock" or push-lock?).

## 6. Parts List (draft)
- [ ] High-pressure in-tank pump (if Option B)
- [ ] Adjustable EFI regulator, 0-100 PSI gauge, and a fuel pressure sensor
- [ ] Fuel filter, 10 micron post-filter
- [ ] 5/16" to AN-6 adapters, AN-6 to GM quick-connect adapters
- [ ] EFI-rated hose, clamps
- [ ] Return line (if needed)

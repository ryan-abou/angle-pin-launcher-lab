# Angle-Pin Launcher Lab

An interactive 3D simulation of a water balloon slingshot in two versions: the original held by hand, and a modified one with a base, an angle pin and a meter stick.

Live site: https://ryan-abou.github.io/angle-pin-launcher-lab/

## What it shows

1. **Projectile physics engine.** Launch speed, flight time, peak height and landing distance, with a live path plot.
2. **Forces and energy tracker.** Force arrows on the balloon and a bar that follows elastic, kinetic and gravitational energy.
3. **Interactive 3D launcher.** Rotate and zoom a labeled model.
4. **Original against modified.** An accuracy test that fires 20 shots from each launcher at the same settings.
5. **Animated modification.** The pin pulls out, the rail tilts, the pin locks. Step through Load, Release, Flight and Impact.
6. **Momentum and variables.** Momentum and impulse, with sliders for mass, pullback, band stiffness and release height.

## Physics

- Energy: `½·k·x² = ½·m·v₀² + m·g·x·sinθ`
- Flight: `x = v₀·cosθ·t`, `y = h + v₀·sinθ·t − ½·g·t²`
- Momentum: `p = m·v`, impulse `J = F_avg·Δt = Δp`

## Assumptions

- No air resistance.
- The bands follow Hooke's law.
- The balloon leaves the pouch at the release height, when the bands return to rest length.
- Balloon mass, band stiffness and handheld wobble are estimates until measured on the real launcher.

Everything is in one file, `index.html`. The 3D view uses three.js.

# BOTTOMLESS | Visual Direction and Graphics System

**Version:** Art System 1.0, accompanying game v2.2  
**Art direction:** Precision-built subterranean sci-fi. Hand-authored vector illustration and Canvas geometry. Designed to look like a cohesive indie mobile game, not generated artwork.

## Creative principles

1. **The drill is the hero.** A strong, centrally mounted silhouette, real-looking structural segmentation, purposeful light sources, a permanently readable BOTTOMLESS display, and progressively more complex equipment.
2. **The earth has substance.** Rock layers use parallax strata, sediment seams, pressure fractures, mineral inclusions, rails, and an impact surface. Mining is visible, not merely a health bar changing.
3. **Special levels are unmistakable.** Standard rock reads cool and solid; ore is warm gold; treasure vaults use amethyst and geometric mineral nodes. One distinct accent family per event class.
4. **Clarity before decoration.** Numbers, BUY MAX, Power Slam, pressure, artifacts, and cores maintain their positions. The full gameplay dashboard still fits on phone-sized screens.
5. **No AI-generated-looking art.** No painterly images, uncanny characters, mismatched textures, gradients with random color shifts, generic AI poster compositions, or external image dependencies. All core art is authored in Canvas/CSS/SVG.

## Palette

| Role | Color | Usage |
|---|---|---|
| Deep void | `#070d19` | Overall game background |
| Rock panel | `#0e1c30` | Main game sections |
| Steel face | `#344f65` | Drill panels |
| Steel edge | `#66899d` | Machinery beveled edges |
| Cool telemetry | `#62e9e0` | Dig progress, pressure information |
| Coin gold | `#f7c879` | Currency, ore veins, ready state |
| Vault amethyst | `#b4a0f5` | Deep treasure and rare components |
| Reward green | `#8de0b9` | Positive earnings and affordable controls |
| Muted blue | `#93acc4` | Secondary UI text |
| Accessible white | `#eff8ff` | Primary text |

## Graphic specifications

**Mine:** single procedural, resolution-independent Canvas scene, pixel-ratio limited to 2. Stratified backgrounds and mineral placements are stable, determined by world depth. Mine occupies the same height as in v2.1. A 24px wide interior rail and strong central tooling establish scale.

**Drill:** visually identifiable motor, protective shoulders, central display, bolts, vents, collar, and bit. Evolving drill stages add stabilizers, power pods, crystal attachments, warm reactor coils, gold frame, and high-tier luminous details. Never obscure the BOTTOMLESS wordmark.

**Special layers:** use material treatment below the bit plus a non-blocking compact banner above the health meter. Ore = gold inclusions; treasure = amethyst metallic seam and clustered crystals. Preserve numeric payout rules and existing milestone triggers.

**Upgrade icons:** one unified SVG icon grid with rounded strokes. Power = crossed drilling tools; Speed = lightning; Value = faceted gemstone. No platform-dependent emoji for these three main upgrades.

**UI:** compact brushed-steel cards, softly chamfered frame language, minimal inner specular highlight, cool outlines, status colors reserved for actual meaning. Keep button labels, previews, accessibility properties, and navigation unchanged.

**Transitions:** CSS-ready pulse on active Power Slam only; existing particles keep their cap. Effects should never compete with the upgrade labels or depth counter. Honor `prefers-reduced-motion`.

## Implementation release phases

### Phase 1: Completed in v2.2

- New procedural geological scene and rock layer material.
- Redesigned Canvas drill with visually staged evolution details.
- Clear ore / treasure scene treatment with a separate label.
- Consistent SVG icons for three upgrades.
- Harmonized HUD, bonuses, buttons, progress meters, event banners, and dialog colors.
- No change to damage, reward, cores, artifacts, rebuilding, or saves.

### Phase 2: Planned, not part of this release

- Individually authored artifact and specimen vector pictograms in the archive.
- Stronger stage-by-stage motor silhouettes and unlock presentations.
- Optional subtle drilling-contact animation tied to actual damage.
- Custom compact icons for Events, Cores, Achievements, and Collections.

### Phase 3: Planned, not part of this release

- Distinctive regional geology motifs for every biome, rather than just palette changes.
- Tiered vault-door visual and multi-fragment rare-ore burst.
- Optional in-game visual-effects intensity setting and battery saver.

## Release acceptance criteria

- Save key and version remain compatible with v2.1 (`bottomless_idle_v3`, save version 4).
- Core upgrades, buy max calculations, pressure, Power Slam, dialogs, and rebuild button unchanged.
- No console/runtime errors in automated Chromium checks across six portrait viewports, including 320px-wide.
- No horizontal overflow; all three upgrade cards visible without scrolling on tested standard phone viewports.
- Verified drill display at early and very deep drill stages, plus treasure layer.
- Existing v2.1 backed up before publication and ability to revert retained.

**Guiding test:** If the art disappears, the game still works exactly as before. If the art is visible, you can immediately tell what is metal, rock, bonus ore, treasure, and drill machinery.
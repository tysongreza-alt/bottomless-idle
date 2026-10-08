# BOTTOMLESS v1.0

A free, one-handed idle drilling game for family and friends. No account, ads, or purchases.

## Play
Live game: https://tysongreza-alt.github.io/bottomless-idle/

On iPhone, open the game in Safari, tap **Share > Add to Home Screen**. On Android, use Chrome's **Install app** option.

## Game loop
Your drill breaks rock automatically. Earn coins and buy three upgrades: **POWER** (damage), **SPEED** (hits per second), and **VALUE** (coins per layer). Use **POWER SLAM** once every 20 seconds for an optional burst of damage.

Ore veins every 25 layers and treasure chambers every 100 layers provide bonus coins. Discover 22 unique artifacts at increasing depths. Each artifact adds a permanent 2% coin bonus. New mine biomes unlock as you descend; the world continues indefinitely.

At depth 110 or deeper, optionally **REBUILD** your machine for permanent **cores**. Each core multiplies damage by 1.20 and coin value by 1.15. Rebuilding resets current depth, temporary upgrades and coins, but keeps best depth, artifacts, and cores. Deeper rebuilds yield more cores.

## Offline and saves
Progress saves locally to the browser or installed app. While away, your drill simulates at 80% speed using the upgrades you had when you closed the game. There are no streaks, energy systems, or paid content.

Use **Menu > Export save** periodically for a backup. Import the JSON backup into the same version to restore progress. Saves don't automatically sync between devices. Clearing site data or uninstalling the app may delete local progress.

## Original v0.1 save
The original unbalanced game remains available at [legacy.html](legacy.html) and uses its original local-storage key (`bottomless_idle_v1`). The redesigned v1.0 starts a separate save (`bottomless_idle_v3`) rather than importing an inflated old balance.

## QA
Automated browser testing covered mobile widths 320, 390, and 430 px, first-hour progression, successive rebuilds, save/reopen, collection interface, eight-hour idle calculations, and 343 arithmetic/pricing checks. These are simulations and do not replace extended hands-on playtesting on every phone.

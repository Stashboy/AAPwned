# AAPwned v0.23.17

A fix release: the native Android Auto **Home button returns to the Dashboard** again.

## What changed

- **Tapping Android Auto's native Home button now goes back to the Coolwalk Dashboard** — the
  split map + media + cards "multitasking" home view — exactly as it does in stock Android Auto.
- Previously the module's `CloseLauncherDashboard` option remapped that button so a **tap performed a
  long-press** (which opens the all-apps launcher instead of the Dashboard). It defaulted **on** with
  no setting to turn it off, so once you left the Dashboard you could never get back to it from the
  Home button. The default is now **off**, restoring native behavior.
- The option still exists on the backend for anyone who deliberately wants the old "Home goes straight
  to the app launcher" behavior — nothing was removed, only the default changed.

## Install

Updates the existing AAPwned package in place (`aapwned-0.23-17.8-r21.apk`). Reboot after installing
so the updated Android Auto hook loads, then reconnect your head unit.

## Credits

AAPwned is a fork of **[Nitsuya/AADisplay](https://github.com/Nitsuya/AADisplay)** — all credit for
the original module goes to Nitsuya. Credit is kept here in the repo and README, never in the
installed package listing. Bundled template/helper code from duzhaokun123 and QAuxiliary (cinit) is
retained under their respective licenses.

versionName `0.23#17.8-r21` · versionCode `3036`

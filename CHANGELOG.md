# Releases

## 1.0.2 Preview - 30 October 2026

Temporarily disable automatic Reborn direct launching and hide its dashboard
option. Backend enable requests are rejected; manual launch, roll, and
diagnostics actions remain available. Setup/uninstall removes only a legacy
registration owned by that installation, with Windows administrator permission
when required. Other Dashboard copies' registrations are left untouched.

Verified 51 launcher tests, normal C# and protected UI/install checks, installed
runtime checks, isolated legacy-registration cleanup during a 1.0.1-to-1.0.2
upgrade, settings retention, and uninstall. The cleanup fixture uses HKCU;
the production elevation branch and other-machine tests remain outstanding.
Unsigned preview.

## 1.0.1 Preview - 30 October 2026

Repair automatic Reborn direct launching while keeping the feature available.
Handle long Electron child commands, Windows short-path aliases, and token-based
child creation while preserving real process IDs/handles. Diagnostic file locks
no longer stop the launcher.

Verified 49 launcher tests, normal C# checks, protected UI/install checks,
1.0.0-to-1.0.1 upgrade, settings retention, uninstall, and direct launching from
an installed copy in a different folder. An explicitly locked diagnostics file
did not interrupt the session. Other-machine/Windows 10 VM and missing-.NET
installation tests remain outstanding. Unsigned preview.

Run setup over the previous installed version with Dashboard and Reborn closed;
no uninstall is required. Application source remains in the separate
[RosDashboard repository](https://github.com/Incognitomode669/RosDashboard/tree/v1.0.1).

## 1.0.0 Preview — 30 October 2026

Windows x64 setup with bundled runtime dependencies, per-user installation,
shortcuts, upgrades and uninstall. Settings are preserved. The current repository
tree contains only distribution information and checksums; installer downloads
are release assets.

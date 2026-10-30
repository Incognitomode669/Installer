# ROS Dashboard Installer

This is a fresh distribution-only repository containing release information and
checksums. Application source, build scripts, tests and development tools have
never been committed to this repository.

## Download

[Download ROS Dashboard Setup 1.0.4 x64](https://github.com/Incognitomode669/Installer/releases/download/v1.0.4/RosDashboard-Setup-1.0.4-x64.exe)

[Installer preview release](https://github.com/Incognitomode669/Installer/releases/tag/v1.0.4)

Copy the single installer to the target machine and run it. Close ROS Dashboard before
updating. Run the new setup over an existing setup installation; no uninstall is
required. Setup preserves user settings and updates the program in its previous directory.
A portable copy is separate: disable its automatic launch hook before moving/removing
that copy. Automatic direct launching remains disabled in the installed Dashboard.

Version 1.0.4 adds dashboard-injected Reborn fixes for a native Transform.Bind
reference leak and skin-loading bursts. Skin requests prioritize base/initial-detail
models, retry capacity-refused requests within existing wait deadlines, and spread
preload/outfit work across frames. The reviewed game/launcher implementations are
checked before applying; unknown implementations are skipped. Load the dashboard
helper for each ROS session. ROS files on disk are unchanged.

Renderer-only launcher update compatibility and the previous Unarmed fixes are retained.
Automatic Reborn direct launching remains disabled and hidden. Manual launch, roll,
and diagnostics remain available.
Setup removes a legacy launch registration owned by the installation being upgraded;
Windows may request administrator permission.

## Requirements and limitations

- Windows 10 1607+ / Windows 11 x64; 32-bit Windows and ARM64 are excluded.
- Python/runtime dependencies and the offline Microsoft .NET Framework 4.8 prerequisite are bundled.
  Installing missing .NET may require administrator permission and a restart.
- Game installations and optional NVIDIA/WireGuard drivers are separate.
- The preview is unsigned. Windows may display a warning; no trusted publisher certificate is included.
- This build passed normal C#, protected UI/install and bundled-runtime checks.
  Installer lifecycle checks passed for earlier releases; 1.0.4 install/upgrade/uninstall,
  other machines and the missing-.NET path have not been tested.
- Existing helper test issues remain unresolved. Obfuscation is not perfect security.

## Checksum

Size: 168,759,114 bytes.

SHA-256: `3731543b3896cc24db529666bb8f5090b9d3b731cef7a4fda35f1255b6104467`

See `checksums/1.0.4.sha256` or the checksum release asset. A checksum detects byte changes;
it does not authenticate the publisher.

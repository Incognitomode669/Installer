# ROS Dashboard Installer

This is a fresh distribution-only repository containing release information and
checksums. Application source, build scripts, tests and development tools have
never been committed to this repository.

## Download

[Download ROS Dashboard Setup 1.0.5 x64](https://github.com/Incognitomode669/Installer/releases/download/v1.0.5/RosDashboard-Setup-1.0.5-x64.exe)

[Installer preview release](https://github.com/Incognitomode669/Installer/releases/tag/v1.0.5)

Copy the single installer to the target machine and run it. Close ROS Dashboard before
updating. Run the new setup over an existing setup installation; no uninstall is
required. Setup preserves user settings and updates the program in its previous directory.
A portable copy is separate: disable its automatic launch hook before moving/removing
that copy. Automatic direct launching remains disabled in the installed Dashboard.

Version 1.0.5 adds a configurable Bomb type target-distance filter with an
on/off toggle and saved maximum in meters, plus partial-capacity backpack delivery.
The native ownership and skin-loading fixes from 1.0.4 are retained.

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
- This build passed normal C#, 120 targeted Python, protected UI/install and bundled-runtime checks.
  An installed upgrade to 1.0.5 preserved settings and passed its runtime check.
  Live distance-filter gameplay, other machines, clean install/uninstall for this version,
  and the missing-.NET path have not been tested.
- Existing helper test issues remain unresolved. Obfuscation is not perfect security.

## Checksum

Size: 168,764,122 bytes.

SHA-256: `431cf4cfb3a034c688d8bc74a140737f8ca24c2404633e8b9546b150eb378756`

See `checksums/1.0.5.sha256` or the checksum release asset. A checksum detects byte changes;
it does not authenticate the publisher.

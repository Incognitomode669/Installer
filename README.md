# ROS Dashboard Installer

This is a fresh distribution-only repository containing release information and
checksums. Application source, build scripts, tests and development tools have
never been committed to this repository.

## Download

[Download ROS Dashboard Setup 1.0.9 x64](https://github.com/Incognitomode669/Installer/releases/download/v1.0.9/RosDashboard-Setup-1.0.9-x64.exe)

[Installer preview release](https://github.com/Incognitomode669/Installer/releases/tag/v1.0.9)

Copy the single installer to the target machine and run it. Close ROS Dashboard before
updating. Run the new setup over an existing setup installation; no uninstall is
required. Setup preserves user settings and updates the program in its previous directory.
A portable copy is separate: disable its automatic launch hook before moving/removing
that copy. Automatic direct launching remains disabled in the installed Dashboard.

Version 1.0.9 adds Game executable... above Load in CHARACTER FLIGHT. Choose the
game version and select its x64/ros64.exe or root-level ros.exe on this PC. Game
directories are saved separately for Reborn, Legacy and Infinity. The identity
dialog still selects the launcher separately. Open the selected game, then click
Load. The other-PC failure has not been reproduced; this addresses a possible
directory mismatch, not every cause of missing helper state.

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
- This build passed normal dashboard checks, all 14 protected UI/install suites,
  and the bundled Python/Frida dependency check. Installer clean install, upgrade/
  uninstall, other machines, live gameplay, and the missing-.NET path were not tested.
- Existing helper test issues remain unresolved. Obfuscation is not perfect security.

## Checksum

Size: 168,757,086 bytes.

SHA-256: `21bd74415cead22fe7c8ecec6c4a47d88a59fa62e8125919aa9f9599a510ea5c`

See `checksums/1.0.9.sha256` or the checksum release asset. A checksum detects byte changes;
it does not authenticate the publisher.

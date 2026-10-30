# ROS Dashboard Installer

This is a fresh distribution-only repository containing release information and
checksums. Application source, build scripts, tests and development tools have
never been committed to this repository.

## Download

[Download ROS Dashboard Setup 1.0.3 x64](https://github.com/Incognitomode669/Installer/releases/download/v1.0.3/RosDashboard-Setup-1.0.3-x64.exe)

[Installer preview release](https://github.com/Incognitomode669/Installer/releases/tag/v1.0.3)

Copy the single installer to the target machine and run it. Close ROS Dashboard before
updating. Run the new setup over an existing setup installation; no uninstall is
required. Setup preserves user settings and updates the program in its previous directory.
A portable copy is separate: disable its automatic launch hook before moving/removing
that copy. Automatic direct launching remains disabled in the installed Dashboard.

Version 1.0.3 accepts renderer-only launcher updates when the reviewed integration
remains unchanged and discovers the newest installed app folder. Changes to integration
code or package loader metadata still require review. Automatic Reborn direct launching
remains disabled and hidden. Manual launch, roll, and diagnostics remain available.
This release also includes the recent Unarmed native-profile and mesh/body-part fixes.
Setup removes a legacy launch registration owned by the installation being upgraded;
Windows may request administrator permission.

## Requirements and limitations

- Windows 10 1607+ / Windows 11 x64; 32-bit Windows and ARM64 are excluded.
- Python/runtime dependencies and the offline Microsoft .NET Framework 4.8 prerequisite are bundled.
  Installing missing .NET may require administrator permission and a restart.
- Game installations and optional NVIDIA/WireGuard drivers are separate.
- The preview is unsigned. Windows may display a warning; no trusted publisher certificate is included.
- Install, upgrade, uninstall and protected-app checks passed on the build machine.
  Other machines and the missing-.NET installation path have not been tested.
- Existing helper test issues remain unresolved. Obfuscation is not perfect security.

## Checksum

Size: 168,757,790 bytes.

SHA-256: `88541a78394793700a6b0b7f12dde50dcf562f2611319631ae7df91b128a0869`

See `checksums/1.0.3.sha256` or the checksum release asset. A checksum detects byte changes;
it does not authenticate the publisher.

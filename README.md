# ROS Dashboard Installer

This is a fresh distribution-only repository containing release information and
checksums. Application source, build scripts, tests and development tools have
never been committed to this repository.

## Download

[Download ROS Dashboard Setup 1.0.0 x64](https://github.com/Incognitomode669/Installer/releases/download/v1.0.0/RosDashboard-Setup-1.0.0-x64.exe)

[Installer preview release](https://github.com/Incognitomode669/Installer/releases/tag/v1.0.0)

Copy the single installer to the target machine and run it. Close ROS Dashboard before
updating. Setup provides shortcuts and an uninstaller and preserves user settings.

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

Size: 168,750,912 bytes.

SHA-256: `619c75b5e0f173efa0ba3c1ce6502af6c433cc3af75d4c53f7b796b1194ecb20`

See `checksums/1.0.0.sha256` or the checksum release asset. A checksum detects byte changes;
it does not authenticate the publisher.

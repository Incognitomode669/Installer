# ROS Dashboard Installer

This is a fresh distribution-only repository containing release information and
checksums. Application source, build scripts, tests and development tools have
never been committed to this repository.

## Download

[Download ROS Dashboard Setup 1.0.6 x64](https://github.com/Incognitomode669/Installer/releases/download/v1.0.6/RosDashboard-Setup-1.0.6-x64.exe)

[Installer preview release](https://github.com/Incognitomode669/Installer/releases/tag/v1.0.6)

Copy the single installer to the target machine and run it. Close ROS Dashboard before
updating. Run the new setup over an existing setup installation; no uninstall is
required. Setup preserves user settings and updates the program in its previous directory.
A portable copy is separate: disable its automatic launch hook before moving/removing
that copy. Automatic direct launching remains disabled in the installed Dashboard.

Version 1.0.6 fixes the Bomb distance filter affecting ordinary gun locks.
The filter now applies only with the matching Bomb action equipped: a throwable
for throwable/AK-47 test modes, or Fists for Unarmed test. Regular gun locks keep
their normal range even when the Bomb feature remains enabled. The saved distance
settings, Bomb queue checks, backpack-capacity delivery and earlier fixes remain.

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
- This build passed normal C#, 125 targeted Python, protected UI/install and bundled-runtime checks.
  An installed upgrade to 1.0.6 preserved settings and passed its runtime check.
  Live distance-filter gameplay, other machines, clean install/uninstall for this version,
  and the missing-.NET path have not been tested.
- Existing helper test issues remain unresolved. Obfuscation is not perfect security.

## Checksum

Size: 168,757,158 bytes.

SHA-256: `2990da64eb26fc39b9ecd1cf6d2e48a74c56d8bebd89404fc143508c76c64249`

See `checksums/1.0.6.sha256` or the checksum release asset. A checksum detects byte changes;
it does not authenticate the publisher.

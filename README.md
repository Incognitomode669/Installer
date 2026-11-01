# ROS Dashboard Installer

This is a fresh distribution-only repository containing release information and
checksums. Application source, build scripts, tests and development tools have
never been committed to this repository.

## Download

[Download ROS Dashboard Setup 1.0.7 x64](https://github.com/Incognitomode669/Installer/releases/download/v1.0.7/RosDashboard-Setup-1.0.7-x64.exe)

[Installer preview release](https://github.com/Incognitomode669/Installer/releases/tag/v1.0.7)

Copy the single installer to the target machine and run it. Close ROS Dashboard before
updating. Run the new setup over an existing setup installation; no uninstall is
required. Setup preserves user settings and updates the program in its previous directory.
A portable copy is separate: disable its automatic launch hook before moving/removing
that copy. Automatic direct launching remains disabled in the installed Dashboard.

Version 1.0.7 adds an editable launcher path with Browse and Save path controls
for Reborn and Infinity. Select the launcher executable in your own installation;
each variant remembers its own location. Missing files and incorrect executable
names are rejected before launch. Existing compatibility checks remain in place.

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
- This build passed normal C# configuration/UI checks, all 64 launcher Python tests,
  all 14 protected UI/install suites and the bundled-runtime check.
  The installed desktop copy passed feature-build UI checks after a direct executable update.
  This installer version's clean install, upgrade/uninstall, other machines and the
  missing-.NET path have not been tested.
- Existing helper test issues remain unresolved. Obfuscation is not perfect security.

## Checksum

Size: 168,766,261 bytes.

SHA-256: `048860d40cf62304b2ffd2a98e31dc9c8b9b072deff1ac045c1ae1b659a53b7b`

See `checksums/1.0.7.sha256` or the checksum release asset. A checksum detects byte changes;
it does not authenticate the publisher.

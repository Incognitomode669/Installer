# Releases

## 1.0.7 Preview - 1 November 2026

Add an editable launcher executable path to the Reborn and Infinity identity
dialogs. Use **Browse...** to locate your installed `RosReborn.exe` (in Reborn's
`app-<version>` folder) or `RosInfinity.exe`. Browsing saves the selection;
typed paths can be saved with **Save path** and are also validated before launch.
Each variant remembers its own path without changing other dashboard settings.
Missing files and incorrect executable names produce a clear error. Existing
automatic discovery remains the default until a custom path is saved, and the
interceptor's compatibility checks still apply to the selected executable.

Installer: `RosDashboard-Setup-1.0.7-x64.exe` (168,766,261 bytes).

SHA-256: `048860d40cf62304b2ffd2a98e31dc9c8b9b072deff1ac045c1ae1b659a53b7b`.

[Download release](https://github.com/Incognitomode669/Installer/releases/tag/v1.0.7).

## Verification and limitations

Normal C# build/configuration/UI checks, all 64 launcher Python regressions,
all 14 protected UI/install suites and the real bundled-runtime check passed.
Configuration tests cover separate variant paths, persistence, unrelated-setting
preservation, and rejection of invalid or missing executables. The rendered path
controls were visually checked. The installed desktop-shortcut copy was updated
with the feature build and its UI checks passed; that was a direct executable
update, not an upgrade using this installer.

This version's installer clean install, upgrade and uninstall, other machines,
and the missing-.NET path were not tested. Existing full-helper-suite issues
remain unresolved. Unsigned preview; game and optional driver requirements are
unchanged. Automatic Reborn direct launching remains disabled and hidden.

## 1.0.6 Preview - 31 October 2026

Fix **Limit bomb distance** affecting ordinary gun target locks while the Bomb
feature is enabled. The lock filter now checks the equipped action: throwable
modes and the AK-47 test require the throwable slot, while Unarmed test requires
Fists. Ordinary guns keep their normal targeting range regardless of the Bomb
feature's toggle or selected dropdown mode. Bomb queues retain their distance
checks, and saved distance/filter preferences are preserved.

125 targeted Python regressions passed, including ordinary-gun acquisition and
retention for every dropdown mode, Bomb/Fists limits, and weapon switching.
Normal C# checks, all 14 protected UI/install suites and the real bundled-runtime
check passed. The local installer upgrade preserved settings and passed the
installed runtime check. Live gameplay confirmation remains pending; reload the
helper (or restart the game and load it again) after updating to use the new code.
Existing full-helper-suite failures remain unresolved. Other machines, this
version's clean install/uninstall, and the missing-.NET path were not tested.
Unsigned preview.

## 1.0.5 Preview - 31 October 2026

Add an optional **Limit bomb distance** toggle and editable **Max (m)** setting
below Bomb type. The filter defaults off with a 10 m starting value; both
preferences are saved. Enabling it limits target-lock acquisition/retention and
the loaded-character queue, with distance checked before actions. Existing
monitoring range, match, team and identity checks still apply.

Backpack auto-fill now delivers the quantity allowed by native carry capacity,
reports partial/skipped items, and continues the remaining bundle. Uncertain
pickup failures still stop delivery to avoid duplicate grants.

Normal C# build/UI checks, 120 targeted Python regressions, all 14 protected
UI/install suites and the bundled-runtime check passed. The installed dashboard
was upgraded to 1.0.5 using this installer; six settings files were preserved,
the installed runtime check passed, and the dashboard reopened. Live gameplay
verification of the distance filter remains pending. The full helper suite's
existing two failures and 33 fixture errors remain unresolved. Other machines,
clean install/uninstall for this version, and the missing-.NET path were not tested.
Unsigned preview; game/driver requirements remain separate.

## 1.0.4 Preview - 31 October 2026

Add dashboard-injected fixes for the reviewed Reborn native Transform.Bind argument
reference leak and skin-loading bursts. Prioritize base/initial-detail model requests,
retry capacity-refused requests within the existing wait deadline, and bound preload
starts and outfit detail changes per frame. Stop restores the skin-loading functions.
Game/launcher guards skip unknown builds; ROS files on disk are unchanged.

Normal C# checks, targeted native ownership/skin scheduling regressions, 14 protected
UI/install suites and the real bundled-runtime check passed. A skins-enabled island
and plane test exercised the patch without multi-second freeze reports or optimizer
errors; short hitches remain and landing/ground combat are not validated. The full
helper suite retains its documented 2 failures and 33 errors. This version's installer
lifecycle, other-machine and missing-.NET tests have not been run. Unsigned preview.

## 1.0.3 Preview - 30 October 2026

Accept renderer-only launcher updates when the reviewed main/preload integration
and package metadata (except version) remain unchanged. Verify archive structure,
member integrity and supported executable settings. Actual build hashes still
invalidate cached offline verification. Discover the newest numeric app folder.
Changes to integration or loader metadata require review. Automatic direct
launching remains disabled and hidden. Includes the recent Unarmed fixes.

Verified 64 launcher tests, 57 hit/target-lock tests, normal C# and protected
UI/install checks, eight offline checks, a real manual intercepted startup,
and isolated 1.0.2-to-1.0.3 upgrade/runtime checks/uninstall with settings retained.
The saved identity was unchanged in startup testing. Unsigned preview; other
machines, missing-.NET and server-acceptance paths remain untested.

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

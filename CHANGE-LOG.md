# Change Log

All notable changes to Bubbles Accessibility Input System (BAIS) are tracked in this file.

## 0.0.20 - 2026-03-20

### Added

- multi-size Windows `.ico` for correct desktop shortcut and app icon (64, 128, 256 px)
- explicit Electron window icon and installer shortcut icon configuration
- persistent device selection across device refreshes
- improved pointer event handling for mouse/trackpad ADS (robust right mouse button tracking)
- accessibility controller, assistive switch, and eye gaze/head tracking input support
- per-device ADS activation settings and profile storage

### Changed

- Windows installer now always creates a desktop shortcut with the correct icon
- device selection no longer reverts to keyboard after refresh
- pointer event handling uses bitmasking for mouse buttons
- updated README to clarify device support, installer, and icon requirements

### Fixed

- right mouse button ADS bug (would only work once, now robust)
- desktop shortcut icon now uses the correct multi-size `.ico` (requires uninstall/reinstall if upgrading)
- device selection persistence after refresh

## 0.0.10 - 2026-03-20

### Added

- explicit Xbox controller detection and family-specific ADS button labels
- explicit PlayStation controller detection and family-specific ADS button labels
- accessibility controller detection for compatible Gamepad API devices
- assistive switch or remapped keyboard-style accessibility input source
- eye gaze or head tracking pointer-style accessibility input source
- per-input ADS activation settings stored in profiles
- keyboard ADS `Disabled` option
- validation coverage for default ADS bindings and accessibility device availability

### Changed

- mouse or trackpad ADS now defaults to right mouse button down
- keyboard ADS remains Shift by default but can now be disabled
- gamepad ADS now uses the selected button instead of fixed trigger behavior
- README updated to document current device support, ADS behavior, packaging, and validation

### Installer And Packaging

- Windows NSIS installer now shows the license agreement before installation
- installer artifacts are generated under `dist/`
- bundled profiles are seeded into the writable user profile store on first run

## 0.0.5 - 2026-03-20

### Baseline

- initial packaged Electron accessibility input utility with profile editing, simulation preview, and Windows build scripts

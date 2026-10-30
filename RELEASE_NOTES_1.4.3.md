# Nodra 1.4.3 — Major Update

**A major step forward for Nodra on Android.**

Nodra 1.4.3 focuses on a smoother, more automatic, and more dependable offline mesh messaging experience. This update improves nearby-device discovery, connection handling, background message forwarding, message notifications, and overall app responsiveness.

## What's new

### Automatic discovery and live chats
- Nearby devices appear in the Radar automatically as they are discovered.
- Direct and group conversations update when messages arrive — no manual refresh required.
- The **Refresh** button remains available as an optional fallback.

### Improved discovery and connectivity
- More reliable Bluetooth/Wi-Fi Nearby discovery and advertising with safeguards against overlapping operations.
- Better connection retry handling and fewer simultaneous-connection conflicts.
- More stable authenticated connection setup without changing the existing security handshake.

### Message notifications
- Incoming message notifications now show the **sender's name and message text**.
- Notifications can be enabled or disabled in **Settings**.
- Android notification permissions are handled when needed.
- The separate ongoing **Nodra Network** notification remains available for active mesh operation.

### Background mesh and relay improvements
- Improved network maintenance while Nodra is running in the background.
- Automatic processing and forwarding of queued Store & Forward packets.
- Reduced duplicate relay sends while a transmission is already in progress.
- Improved updates to relay queues, packet counters, and network indicators.

### Performance and interface optimization
- Smoother screen swipes and navigation.
- Fewer unnecessary interface updates as nearby nodes and messages change.
- Less heavy message-sending and relay-processing work on the UI thread.
- Better responsiveness when interacting with chats, controls, and the Radar.

## UI Redesign — Post-release source update (October 30, 2026)

**From futuristic styling to focused privacy.** The Android source has been updated with a stricter, more minimal design that emphasizes private communication over decorative futurism. The interface now features a compact text-only NODRA Home header, clearer dark/light palettes, flat cards, refined navigation and understated message bubbles.

This is a **visual-only change**, with the existing functionality, network protocol, encryption and security unchanged.

Source change: [Nodra 1.4.3 — UI Redesign](https://github.com/NodraMesh/Nodra/pull/4).

**Important:** The existing `Nodra-1.4.3.apk` in this release was compiled before the redesign. It **does not contain these UI changes**. No new APK has been published and the published checksum remains unchanged.

## Security remains a priority

This release **does not weaken or replace Nodra's existing cryptography or security protocols**. Encrypted messaging, signed packets, authenticated peer profiles, trusted-key checks, and the existing replay and TTL protections remain in place.

## Download and installation

Download **Nodra-1.4.3.apk** from the Assets section of this release and install it on your Android device. Only use APKs distributed through the official **NodraMesh/NodraApps** repository.

*Background discovery and connectivity are subject to Android device permissions, radio availability, and battery-management restrictions.*

---

**Nodra — Stay Connected**

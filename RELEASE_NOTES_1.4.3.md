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

## UI Redesign — October 30, 2026

**From futuristic styling to focused privacy.** The UI Redesign build introduces a stricter, more minimal design that emphasizes private communication over decorative futurism. The interface now features a compact text-only NODRA Home header, clearer dark/light palettes, flat cards, refined navigation and understated message bubbles.

This is a **visual-only change**, with the existing functionality, network protocol, encryption and security unchanged.

**Availability:** The UI Redesign is included in `Nodra-1.4.3-UI-Redesign.apk`. The original `Nodra-1.4.3.apk` remains available with the previous design. Both APKs are version 1.4.3.

## Security remains a priority

This release **does not weaken or replace Nodra's existing cryptography or security protocols**. Encrypted messaging, signed packets, authenticated peer profiles, trusted-key checks, and the existing replay and TTL protections remain in place.

## Download and installation

Choose one APK from the Assets section of this release:

- **UI Redesign:** [`Nodra-1.4.3-UI-Redesign.apk`](https://github.com/NodraMesh/NodraApps/releases/download/v1.4.3/Nodra-1.4.3-UI-Redesign.apk) — new minimal interface.
- **Original:** [`Nodra-1.4.3.apk`](https://github.com/NodraMesh/NodraApps/releases/download/v1.4.3/Nodra-1.4.3.apk) — previous interface.

Both are Nodra 1.4.3. Only use APKs distributed through the official **NodraMesh/NodraApps** repository.

### File integrity — SHA-256

```text
Nodra-1.4.3-UI-Redesign.apk
391453A3A58C0B75AE2D337FA3E0B4741419BBECF6B7821EF78B3FB674006A85

Nodra-1.4.3.apk
E12142749B6B01F947E908E22397046346F18AA9CAD25CF0BEE73668C2B48333
```

*Background discovery and connectivity are subject to Android device permissions, radio availability, and battery-management restrictions.*

---

**Nodra — Stay Connected**

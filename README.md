<div align="center">

<img src="https://github.com/1337Xcode/echo-echo/blob/main/files/echo-echo.gif" alt="echo-echo-gif">

# Echo Echo

**Decentralized peer-to-peer chat application with end-to-end encryption**

[![Live Demo](https://img.shields.io/badge/Live_Demo-Available-brightgreen)](https://1337xcode.github.io/echo-echo/)
[![Version](https://img.shields.io/badge/Version-1.0.0-blue.svg)](https://github.com/1337Xcode/echo-echo/releases)
[![License](https://img.shields.io/badge/License-Proprietary-red.svg)](LICENSE)
[![Security](https://img.shields.io/badge/Security-E2EE-success.svg)](https://github.com/1337Xcode/echo-echo#security--privacy)

[**Try Live Demo**](https://1337xcode.github.io/echo-echo/) • [**Report Issues**](https://github.com/1337Xcode/echo-echo/issues)

</div>

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Architecture](#architecture)
- [How It Works](#how-it-works)
- [Security & Privacy](#security--privacy)
- [Browser Compatibility](#browser-compatibility)
- [Limitations & Known Issues](#limitations--known-issues)
- [To Do](#to-do)
- [Support](#support)

---

## Overview

EchoEcho is a decentralized chat platform designed to provide secure, anonymous communication over the web. With peer-to-peer architecture, all messages are encrypted, ensuring that conversations remain private and protected. EchoEcho eliminates the need for centralized servers, giving users complete control over their data.

---

## Features

- **Peer-to-peer messaging** via WebRTC with no central server
- **End-to-end encryption** using [NaCl cryptography](https://tweetnacl.js.org/)
- **Anonymous by default** - no registration or personal data required
- **Content filtering** for profanity and URLs
- **Real-time presence** indicators
- **Torrent-style message propagation** for resilience
- **Modern, responsive** web interface (HTML5 + CSS3)
- **Cross-platform compatibility** with all major desktop browsers

---

## Architecture

EchoEcho employs a multi-layered design:

<div align="left">
  <img src="https://pouch.jumpshare.com/preview/hc-YfUm1HUYU9hzKEXjUNaxZKm5ECRctoBcrEti-pU3Oc3yD-Dpc2B2xvpt1rddc8rSF5HBc4Szs9xEzOoVLksTq66ad9RqgxP2dlYxXcoY" alt="Diagram" width="360">
</div>

---

## How It Works

**1. Peer Discovery**  
Browsers connect to public Gun.js relays to find peers. No chat data is stored on these servers, only connection metadata for signaling.

**2. Connection Establishment**  
Once a peer is found, a direct WebRTC connection is negotiated between browsers.

**3. Secure Messaging**  
Messages are encrypted client-side before being sent and can only be decrypted by intended recipients.

**4. Content Filtering**  
Profanity and URLs are filtered before messages are sent or displayed.

**5. Message Propagation**  
Messages may be re-broadcasted through multiple peers to enhance reliability.

---

## Security & Privacy

- **End-to-end message encryption** (NaCl/TweetNaCl)
- **Local key generation** - encryption keys generated locally; never sent to any server
- **Zero registration** - no persistent identity, no registration, no personal information required
- **Minimal relay dependency** - relay servers only handle encrypted connection metadata for signaling
- **Client-side processing** - all filtering and cryptography handled client-side

> **Note:** The current version of Echo Echo is closed source and distributed as obfuscated JavaScript. This is to prevent misuse, protect ongoing development work, and limit abuse while the project continues to evolve. Selected components may be open-sourced in the future as the implementation mature.

---
**Open Source Roadmap:**  
Select components and educational examples may be open-sourced in the future once the security model are finalized. Feedback and collaboration requests are welcome via [issues](https://github.com/1337Xcode/echo-echo/issues)

## Browser Compatibility

| Browser | Support | Notes |
|---------|---------|-------|
| **Chrome / Chromium** | ✅ Full | Recommended for full compatibility |
| **Firefox** | ✅ Full | Fully supported |
| **Edge** | ✅ Full | Chromium-based versions |
| **Safari** | ⚠️ Partial | WebRTC support is limited in some scenarios |
| **Mobile Browsers** | ⚠️ Partial | iOS Safari has significant limitations |

---

## Limitations & Known Issues

- **Mobile Support:** Limited functionality on iOS devices
- **Relay Dependency:** Peer discovery relies on public Gun.js relays
- **Closed Source:** Codebase is not reviewable at this time
- **Scale Limitations:** Not designed or tested for large-scale use

---

## To Do

- **Voice and Video Communication** - Enable real-time audio and video calls
- **File Sharing** - Secure file exchange between peers
- **Mobile Optimization** - Improve support for mobile devices, especially iOS
- **Performance Enhancements** - Optimize peer discovery and messaging flow

---

## Support

- [**Report Issues**](https://github.com/1337Xcode/echo-echo/issues) for bugs or feature requests

---

<div align="center">

**Developed and maintained by [1337Xcode](https://github.com/1337Xcode)**
</div>

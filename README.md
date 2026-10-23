# Awesome Media Streaming Servers

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![Tracked Projects](https://img.shields.io/badge/Streaming%20Servers-Curated-blue.svg)](https://github.com/ishandutta2007/Awesome-Media-Streaming-Servers)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

> A curated directory of the best **media streaming servers**, self-hosted home theater systems, live video streaming infrastructure, RTMP/WebRTC routers, and enterprise video SaaS platforms.

---

## Table of Contents

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS & Hosted Streaming Platforms](#saas--hosted-streaming-platforms)
- [Open-Source Media Streaming Servers](#open-source-media-streaming-servers)
- [Key Architectural Trade-Offs](#key-architectural-trade-offs)
- [How to Contribute](#how-to-contribute)
- [License & Disclaimer](#license--disclaimer)

---

## Sector Overview & Market Dynamics

The global video streaming software and infrastructure market is valued at approximately **$18 billion to $20 billion** (growing at ~17–19% CAGR toward $60B+ by the early 2030s). The industry exhibits a **moderately concentrated, bifurcated structure**: hyperscalers and private-equity-backed incumbents (AWS, Vimeo, Brightcove) anchor enterprise broadcast distribution, while an active, highly fragmented long-tail of specialized WebRTC engines, self-hosted media servers, and open-source streaming software commands developer and prosumer self-hosting niches.

---

## SaaS & Hosted Streaming Platforms

The following SaaS and managed streaming platforms are sorted in descending order by **Company Scale** (enterprise valuation / parent company market cap / annual run-rate).

| Product | Scale (Valuation / Revenue) | Description | Pricing | Free Tier Limit |
| :--- | :--- | :--- | :--- | :--- |
| **[AWS Elemental MediaLive](https://aws.amazon.com/medialive/)** | **~$2.1 Trillion** (Amazon market cap) | Broadcast-grade cloud live video processing engine with high-availability encoding ladders and multi-protocol ingest. | Starting at **$0.29/hour** per HD AVC input + **$0.70/hour** per HD output (~$2.00–$5.00/hour per active channel); idle channels charged at $0.01/hour. | **No free tier** for MediaLive (standard AWS Free Tier applies to compute/storage resources only; 30-day Free Trial for AWS accounts covers general AWS services, but MediaLive channel run-hours are billed as consumed). |
| **[Vimeo Enterprise](https://vimeo.com/enterprise)** | **$1.38 Billion** (Bending Spoons acquisition) / ~$415M rev | Enterprise-grade live event streaming, internal corporate communications, and content governance platform. | Custom annual licensing starting at **$1,200–$2,400/year** (standard plans start at **$20/seat/month** billed annually). | **30-day free trial** with standard hosting access (Enterprise requires custom sales POC; permanent free tier allows 3 videos and up to 500MB storage total). |
| **[Brightcove](https://www.brightcove.com/)** | **$233 Million** (Bending Spoons acquisition) / ~$195M rev | Enterprise video distribution, OTT monetization, SSAI ad-insertion, and multi-CDN video management. | Custom enterprise quotes starting at estimated **$199/month** (basic package) up to **$20,000–$250,000+/year** for full broadcast suites. | **30-day free trial** upon approved sales request; no permanent free tier. |
| **[Kaltura](https://corp.kaltura.com/)** | **~$180 Million** (Annual Recurring Revenue / Nasdaq: KLTR) | Highly customizable enterprise video platform, virtual classroom LMS hub, and developer media APIs. | Starting at **$20 base fee** + usage-based developer consumption; standalone webinar/portal modules start at **$150/month**. | **30-day free trial** with $1 developer API credit; no permanent free tier for enterprise video platform. |
| **[Plex](https://www.plex.tv/)** | **~$65 Million** (Estimated ARR) / $130M+ raised | Polished home media server with native client apps, remote streaming, FAST live channels, and media library aggregation. | **Plex Pass**: **$6.99/month**, $69.99/year, or **$750 lifetime** (price updated in 2026). | **Free plan forever**: Unlimited local personal media library playback and access to free ad-supported FAST TV channels. Hardware-accelerated transcoding, remote streaming sync, and skip intros require Plex Pass. |
| **[Wowza Streaming Engine](https://www.wowza.com/)** | **~$30 Million** (Estimated ARR; Clearhaven PE backed) | Enterprise-grade software server for live streaming, low-latency transcoding, and multi-protocol delivery (HLS, RTMP, WebRTC, MPEG-DASH). | Starting at **$195/month** per instance (includes 10 concurrent transcoding channels; $25/month per additional channel). | **30-day free trial** (limited to 1 streaming instance, watermarked video stream, and capped connection hours). |
| **[Red5 Pro](https://www.red5.net/)** | **~$8 Million** (Estimated ARR) | Ultra-low latency (<250ms) WebRTC streaming server supporting autoscaling cross-cloud clusters. | Developer tier starting at **$29.99/month** (up to 100 concurrent connections, standalone server); Growth tier at **$299/month** with real-time transcoding. | **30-day free trial** (full access up to 10 concurrent connections for staging and local development). |
| **[Dacast](https://www.dacast.com/)** | **~$5 Million** (Estimated ARR) | Turnkey live streaming and VOD SaaS platform with white-label video player and integrated monetization. | Starter plan starting at **$39/month** (includes 2.4 TB bandwidth/year; bandwidth overage billed at $0.30/GB); Scale plan at **$165/month**. | **14-day free trial** with 10 GB of streaming bandwidth and full white-label player testing; no permanent free tier. |
| **[Emby](https://emby.media/)** | **Privately held** (Bootstrapped personal media server) | Hybrid personal streaming server balancing self-hosted configurability with turnkey client apps. | **Emby Premiere**: **$4.99/month**, $54/year, or **$119 lifetime** license (capped at 30 client devices). | **Free plan forever**: Complete personal media streaming for home networks and DLNA devices. Live TV/DVR recording, hardware transcoding, and offline downloads require Premiere. |

---

## Open-Source Media Streaming Servers

The following projects are open-source media streaming and routing solutions, sorted in descending order by **GitHub Star Count**.

| Project | Stars | Primary Protocols & Tech | Description |
| :--- | :--- | :--- | :--- |
| **[Jellyfin](https://github.com/jellyfin/jellyfin)** | [![GitHub Stars](https://img.shields.io/github/stars/jellyfin/jellyfin?style=social&color=white)](https://github.com/jellyfin/jellyfin/stargazers) | HLS, DASH, DLNA (.NET / C#) | **The 100% free software media system.** Self-hosted alternative to Plex and Emby with zero paywalls. Hardware transcoding (NVENC, VAAPI, Intel QSV, Apple Silicon), multi-user profiles, and cross-platform clients are completely free. |
| **[Kazumi](https://github.com/Predidit/Kazumi)** | [![GitHub Stars](https://img.shields.io/github/stars/Predidit/Kazumi?style=social&color=white)](https://github.com/Predidit/Kazumi/stargazers) | HTTP, HLS, Custom XPath (Flutter / Dart) | **Rule-based anime streaming and media aggregator.** Features custom XPath parsing rules, Danmaku (bullet comments) synchronization, DLNA casting, Anime4K real-time upscaling, and multi-device playback synchronization. |
| **[SRS (Simple Realtime Server)](https://github.com/ossrs/srs)** | [![GitHub Stars](https://img.shields.io/github/stars/ossrs/srs?style=social&color=white)](https://github.com/ossrs/srs/stargazers) | RTMP, WebRTC, HLS, HTTP-FLV, SRT (C++) | **Industrial-strength real-time video streaming server.** Highly efficient single-core concurrency model widely used for ultra-low latency live streaming, interactive broadcasts, and edge RTMP/WebRTC conversion. |
| **[Navidrome](https://github.com/navidrome/navidrome)** | [![GitHub Stars](https://img.shields.io/github/stars/navidrome/navidrome?style=social&color=white)](https://github.com/navidrome/navidrome/stargazers) | HTTP, Subsonic API, Transcoding (Go) | **Lightweight modern music streaming server.** Compatible with all Subsonic/Madsonic client applications. Handles massive audio collections with minimal memory footprint, on-the-fly transcoding, and multi-user support. |
| **[LiveKit](https://github.com/livekit/livekit)** | [![GitHub Stars](https://img.shields.io/github/stars/livekit/livekit?style=social&color=white)](https://github.com/livekit/livekit/stargazers) | WebRTC, WHIP, WHEP, SIP (Go) | **End-to-end real-time WebRTC infrastructure.** High-performance Selective Forwarding Unit (SFU) designed for live interactive video, spatial audio, teleconferencing, and AI voice streaming with sub-100ms latency. |
| **[LibreTV](https://github.com/LibreSpark/LibreTV)** | [![GitHub Stars](https://img.shields.io/github/stars/LibreSpark/LibreTV?style=social&color=white)](https://github.com/LibreSpark/LibreTV/stargazers) | HLS, M3U8, IPTV (JavaScript / Node) | **Aggregated live stream and media search portal.** Lightweight self-hosted platform parsing public M3U/M3U8 playlists with built-in ad filtering, cross-source merging, and responsive browser playback. |
| **[MediaMTX](https://github.com/bluenviron/mediamtx)** | [![GitHub Stars](https://img.shields.io/github/stars/bluenviron/mediamtx?style=social&color=white)](https://github.com/bluenviron/mediamtx/stargazers) | SRT, WebRTC, RTSP, RTMP, HLS, MoQ (Go) | **Zero-dependency multi-protocol live video router.** Standalone binary that acts as a real-time message bus and transcoder for IP cameras, drone feeds, and live distribution pipelines with zero external dependencies. |
| **[Audiobookshelf](https://github.com/advplyr/audiobookshelf)** | [![GitHub Stars](https://img.shields.io/github/stars/advplyr/audiobookshelf?style=social&color=white)](https://github.com/advplyr/audiobookshelf/stargazers) | HTTP, HLS, WebSockets (Node.js) | **Self-hosted audiobook and podcast server.** Complete library organizer with progress synchronization across iOS and Android apps, chapter-level navigation, metadata scraping, and multi-user permissions. |
| **[Kavita](https://github.com/Kareadita/Kavita)** | [![GitHub Stars](https://img.shields.io/github/stars/Kareadita/Kavita?style=social&color=white)](https://github.com/Kareadita/Kavita/stargazers) | OPDS, HTTP/REST (.NET / C#) | **Fast, feature-rich digital reading and media server.** Built for manga, comics, and ebooks with an integrated responsive web reader, reading stats, user progress tracking, and OPDS server support for e-readers. |
| **[Owncast](https://github.com/owncast/owncast)** | [![GitHub Stars](https://img.shields.io/github/stars/owncast/owncast?style=social&color=white)](https://github.com/owncast/owncast/stargazers) | RTMP Ingest, HLS Output (Go) | **Self-hosted live streaming and chat server.** An open-source, decentralized alternative to Twitch and YouTube Live. Provides built-in chat, custom moderation, web player, and Fediverse / ActivityPub integration. |
| **[Janus Gateway](https://github.com/meetecho/janus-gateway)** | [![GitHub Stars](https://img.shields.io/github/stars/meetecho/janus-gateway?style=social&color=white)](https://github.com/meetecho/janus-gateway/stargazers) | WebRTC, SIP, RTSP, RTP (C) | **General-purpose WebRTC server.** Modular C-based SFU gateway that enables real-time peer-to-peer and group communications, video rooms, streaming relays, and legacy SIP/VoIP gateway integration. |
| **[Ant Media Server](https://github.com/ant-media/Ant-Media-Server)** | [![GitHub Stars](https://img.shields.io/github/stars/ant-media/Ant-Media-Server?style=social&color=white)](https://github.com/ant-media/Ant-Media-Server/stargazers) | WebRTC, CMAF, HLS, RTMP, RTSP (Java) | **Scalable ultra-low latency streaming engine.** Supports real-time WebRTC ingest/playout (<0.5s latency), automatic adaptive bitrate streaming, and horizontal clustering on Kubernetes. |
| **[Gerbera](https://github.com/gerbera/gerbera)** | [![GitHub Stars](https://img.shields.io/github/stars/gerbera/gerbera?style=social&color=white)](https://github.com/gerbera/gerbera/stargazers) | UPnP / DLNA (C++) | **UPnP / DLNA media server for local networks.** Lightweight media daemon allowing home playback of digital audio, video, and image files to smart TVs, game consoles, and DLNA media renderers. |

---

## Key Architectural Trade-Offs

When selecting between SaaS streaming platforms and self-hosted open-source servers, evaluate these core architectural criteria:

1. **Protocol Latency**:
   - **Ultra-Low Latency (<500ms)**: Use WebRTC / WHIP / WHEP engines like **LiveKit**, **Red5 Pro**, or **Janus Gateway** for interactive live experiences, remote robotics, or video calling.
   - **Low Latency (1s–3s)**: Use SRT / Low-Latency HLS (LL-HLS) with **MediaMTX** or **SRS** for near-live gaming and sports.
   - **Standard Video on Demand & Distribution (5s–30s)**: Use traditional HLS / MPEG-DASH via **Jellyfin**, **Plex**, or **AWS Elemental MediaLive**.
2. **Infrastructure Burden vs. Operating Margin**:
   - SaaS platforms (AWS, Dacast, Brightcove) eliminate transcoding orchestration and CDN maintenance but introduce variable egress fees ($0.05–$0.30/GB).
   - Self-hosted servers (Jellyfin, MediaMTX, SRS) require dedicated GPU/CPU hardware for hardware transcoding (NVENC/VAAPI/QuickSync) and robust uplink bandwidth.
3. **Ecosystem & Ownership**:
   - Plex and Emby offer plug-and-play mobile and TV apps at the expense of privacy and increasing subscription fees.
   - Jellyfin delivers complete data autonomy and free hardware transcoding without license enforcement.

---

## How to Contribute

We welcome contributions from developers, self-hosters, and video engineers!

1. Fork this repository.
2. Add your project or update existing details in `README.md`.
3. Adhere to our strict tabular formats:
   - For SaaS products: include **Scale**, **Pricing** (specific starting tier), and **Free Tier Limit**.
   - For open-source projects: include repo link, **GitHub Star badge** (linking to `/stargazers`), protocols, and technical summary.
4. Open a Pull Request with a clear rationale.

---

## License & Disclaimer

- Distributed under the [Creative Commons Zero v1.0 Universal License (CC0-1.0)](LICENSE).
- All trademarks and brand names belong to their respective corporate owners.
- Projects aggregating third-party streams (such as Kazumi and LibreTV) do not host content; users are solely responsible for ensuring compliance with applicable copyright laws.

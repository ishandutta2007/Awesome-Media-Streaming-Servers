# Awesome-Media-Streaming-Servers

# Top Media Streaming Servers Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Self-Hosted Media Servers, Live Streaming Platforms & Open-Source Alternatives*  
**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Media Streaming Servers**. These tools enable users and organizations to host, manage, and deliver video and audio content—ranging from personal media libraries streamed to living room devices to enterprise-grade live streaming infrastructure.

**Examples** include Plex, Emby, Jellyfin, Wowza, Red5 Pro, Kaltura, Brightcove, Vimeo Enterprise, AWS Elemental, and Dacast (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, avoiding subscription fees, and controlling your media infrastructure. The open-source landscape is anchored by **Jellyfin** (the fully free Plex alternative with no paywalled features), **MediaMTX** (the zero-dependency live media router), and **Kazumi** (the rule-based anime streaming client), with **Emby** serving as the middle-ground proprietary option and **LibreTV** offering aggregated search/playback for web content.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

| Product | Description | Pricing | Free Tier Limit |
| :--- | :--- | :--- | :--- |
| **[Plex](https://www.plex.tv/)** | Polished media server with streaming channels, remote access, and hardware transcoding. Proprietary. | **Plex Pass**: $6.99/month or $69.99/year. **Lifetime Pass**: **$750** (tripled from $250 in 2026) . | **Free**: Basic media server, local playback. Hardware transcoding and remote streaming require Plex Pass . |
| **[Emby](https://emby.media/)** | Media server positioned between Plex and Jellyfin—some DIY configurability with paid tiers for premium features. | **Premiere**: $4.99/month, $54/year, or **$119 lifetime** (30-device limit) . | **Free**: Basic media server functionality. Hardware transcoding and other features require Premiere . |
| **[Wowza Streaming Engine](https://www.wowza.com/)** | Enterprise live streaming server supporting HLS, RTMP, and MPEG-DASH. | **Basic**: **$195/month** per instance (includes 10 concurrent transcoding channels; $25/channel/month overage) . | **30-day free trial**. No permanent free tier. |
| **[Red5 Pro](https://www.red5.net/)** | Ultra-low latency (<250ms) streaming server with WebRTC, autoscaling, and on-prem/cloud deployment. | **Developer**: **$29.99/month** (100 connections, no clustering). **Startup**: $119/month. **Growth**: $299/month (includes transcoding). **Enterprise**: from $3,499/month . | **30-day free trial** . No permanent free tier. |
| **[Kaltura](https://corp.kaltura.com/)** | Enterprise video platform with LMS integration and deep customization. | Estimated **$1,200–$30,000/year** license, plus onboarding $1,000–$10,000 . | No public free tier. |
| **[Brightcove](https://www.brightcove.com/)** | Enterprise video platform for large-scale media distribution and OTT monetization. **Acquired by Bending Spoons (2025)**. | No public pricing. Third-party estimates: **$20,000–$250,000+/year** . | **No free tier**—enterprise-contract pricing only . |
| **[Vimeo Enterprise](https://vimeo.com/enterprise)** | Business video platform with event hosting and broad distribution tools. **Acquired by Bending Spoons (2025)**—same owner as Brightcove. | Estimated **$1,200–$2,400/year** for 10 users (license only) . | No permanent free tier for Enterprise. |
| **[AWS Elemental MediaLive](https://aws.amazon.com/medialive/)** | Broadcast-grade live video processing service. | Usage-based with **idle and running charges** for channels, inputs, and outputs. No contracts or minimums . | **No free tier** for MediaLive itself. AWS Free Tier applies to consumed resources. |
| **[Dacast](https://www.dacast.com/)** | Live streaming and VOD platform with white-label branding on all plans. | **Starter**: **$39/month**. **Scale**: $165/month (priority support) . Bandwidth overage at **$0.30/GB** . | No permanent free tier. Trial available. |

## Open-Source GitHub Projects

- **[Jellyfin](https://github.com/jellyfin/jellyfin)** [![GitHub Stars](https://img.shields.io/github/stars/jellyfin/jellyfin?style=social&color=white)](https://github.com/jellyfin/jellyfin/stargazers)  
  **The fully free Plex alternative.** Self-hosted media server with **no paywalled features**—hardware transcoding, remote streaming, and mobile sync are all free . **Trade-offs**: remote streaming requires manual network configuration (reverse proxy, VPN, or dynamic DNS); less polished apps than Plex . Best for privacy-conscious users who want Plex-like functionality without subscriptions.

- **[MediaMTX](https://github.com/bluenviron/mediamtx)** [![GitHub Stars](https://img.shields.io/github/stars/bluenviron/mediamtx?style=social&color=white)](https://github.com/bluenviron/mediamtx/stargazers)  
  **The zero-dependency live media router.** Single executable (no dependencies or interpreter) supporting **SRT, WebRTC, RTSP, RTMP, HLS, MPEG-TS, RTP, and Media-over-QUIC** . **Features**: automatic protocol conversion, hot reloading, recording/playback, JWT/HTTP authentication, Prometheus metrics, and cross-platform (Linux, Windows, macOS). Best for live streaming pipelines requiring broad protocol support without infrastructure overhead.

- **[Kazumi](https://github.com/Predidit/Kazumi)** [![GitHub Stars](https://img.shields.io/github/stars/Predidit/Kazumi?style=social&color=white)](https://github.com/Predidit/Kazumi/stargazers)  
  **The rule-based anime streaming client.** ~37k+ stars. Flutter-based app with **custom XPath rules** for content collection, streaming playback, and **Danmaku (bullet comments)** support . **Features**: rule editor, anime catalog/search/schedule, multi-source support, hardware acceleration, DLNA casting, real-time super-resolution via Anime4K, and cross-device sync . **Platforms**: Android, Windows, macOS, Linux (experimental), iOS (sideload) . **Caveat**: does not host content—ads come from video sources, not the app . Best for anime enthusiasts wanting a customizable, ad-free viewing client.

- **[LibreTV](https://github.com/LibreSpark/LibreTV)** [![GitHub Stars](https://img.shields.io/github/stars/LibreSpark/LibreTV?style=social&color=white)](https://github.com/LibreSpark/LibreTV/stargazers)  
  **The aggregated search and playback platform.** ~14k–17.8k stars (trending #1 on GitHub in April 2026) . Lightweight online video search aggregating multiple sources with cross-source merging, HLS playback with ad-filtering, and live TV/IPTV via M3U subscriptions. **Deployment**: Docker, Vercel, Cloudflare Pages. **Critical caveat**: requires a `PASSWORD` env var; the project **does not store or host content**—it parses third-party public playlists, and users are responsible for source legality. **Note**: repository appears to be archived . Best for users wanting a self-hosted aggregated search interface.

### Additional Strong Open-Source Options

- **Emby (free tier)** — Basic media server functionality without Premiere. Best for users wanting a middle ground between Plex and Jellyfin.
- **Navidrome** — Lightweight music server compatible with Subsonic API. Best for music-only libraries.
- **Audiobookshelf** — Purpose-built server for audiobooks and podcasts. Best for spoken-word audio collections.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- **Plex's lifetime price tripled to $750** in 2026. Jellyfin offers comparable features for free, though remote streaming requires more setup .
- **Brightcove and Vimeo Enterprise share the same owner** (Bending Spoons). Switching between them does not diversify ownership risk .
- **Kazumi and LibreTV do not host content**: they parse third-party sources, and users are solely responsible for the legality of content they access .
- **Self-hosted platforms require infrastructure**: Jellyfin, MediaMTX, and Kazumi all need servers, storage, and network configuration—free software is not free operations.
- **Wowza and Red5 Pro pricing is per-instance and excludes infrastructure**: server, storage, CDN/egress, and support are billed separately .

---

**Made for media enthusiasts, cord-cutters, and self-hosters building their own streaming infrastructure.**  
Let's make media streaming more open, privacy-respecting, and appropriately scoped.

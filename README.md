<p align="center">
  <img src="https://mapflyover.com/logo.png" alt="Mapflyover logo" width="96">
</p>

<h1 align="center">Mapflyover</h1>

<p align="center">
  <strong>Mapflyover is a web app that turns any place on Earth into a cinematic 3D map flyover video</strong> — with AI narration, word-timed captions and cinematic camera moves, built and rendered entirely in your browser.
</p>

<p align="center">
  <a href="https://mapflyover.com"><img src="https://img.shields.io/badge/Website-mapflyover.com-0284c7" alt="Website"></a>
  <a href="https://mapflyover.com/pricing"><img src="https://img.shields.io/badge/Pricing-Free%20to%20start-0ea5e9" alt="Pricing"></a>
  <a href="https://mapflyover.com/agents"><img src="https://img.shields.io/badge/AI%20agents-Claude%20%26%20ChatGPT-7c3aed" alt="Connect an AI agent"></a>
  <a href="https://mapflyover.com/guides"><img src="https://img.shields.io/badge/Guides-Tutorials-334155" alt="Guides"></a>
</p>

## What it does

Mapflyover turns a place and a script into a finished map video. You pick locations on a real map, arrange them into scenes, and Mapflyover flies a cinematic camera between them while AI narration reads your script and captions appear in time with the words. The result exports as an MP4 in vertical (9:16) or landscape (16:9) — the formats used by YouTube, Shorts, Reels and TikTok.

The "3D" in Mapflyover is a cinematic camera effect: the camera tilts to an angled view (up to 85°) over real map imagery with terrain relief, and moves with pans, zooms and orbits between scenes. It is not modelled 3D buildings.

Building is free. You only pay when you want more, longer or sharper exports without the Mapflyover mark.

## Key features

- **Full in-browser editor** — scenes, stat and focus cards, real place boundaries, and scene JSON import
- **Cinematic camera moves** — angled flyovers up to 85°, orbit moves, terrain relief, smooth transitions between places
- **AI narration** — 48 voices, generated from your script; narration is free on every plan and needs no API key
- **Word-timed captions** — captions are timed from the narration, with 7 caption presets and 8 fonts, including word-highlighted styles
- **10 map styles** — including a satellite look
- **Unlimited previews** — preview as often as you like; only exports count against your plan
- **MP4 export in your browser** — 9:16 or 16:9, from 720p up to 4K depending on plan
- **AI agent connection (MCP)** — connect Claude, ChatGPT or another MCP client and let your agent build the project for you
- **Share to Buffer** — send finished videos to your social channels (Pro and Studio, with your own Buffer token)

Full breakdown: [docs/features.md](docs/features.md)

## Who it's for

- **Travel and geography creators** making map-led videos for YouTube, Shorts, Reels and TikTok
- **Teachers and students** explaining places, journeys and history visually
- **Real estate and local businesses** showing where a property or business sits and what surrounds it
- **Anyone** who wants a map video without learning video-editing or animation software

More: [docs/use-cases.md](docs/use-cases.md)

## How it works

1. **Pick your places** — search the map, drop scenes, and arrange your route or story.
2. **Add your script** — write the narration; Mapflyover generates the voiceover and times the captions to it.
3. **Export** — render the MP4 in your browser and publish it wherever you post video.

Step-by-step: [How it works](https://mapflyover.com/how-it-works) · [Guides](https://mapflyover.com/guides)

## Connect your AI agent

Mapflyover speaks the Model Context Protocol (MCP). Connect Claude, ChatGPT or any MCP client with a single OAuth 2.0 sign-in — no API key to paste — and your agent can create and build Mapflyover projects from a plain description: scenes, narration and captions included. You stay in control: agents cannot export videos or spend credits, so you review the project and export it yourself in the editor with one click.

Your agent can also build a video for someone who has no Mapflyover account and hand them a **claim link**: they open it, sign up with Google, press Claim, and the projects land in their own library. See [docs/claim-links.md](docs/claim-links.md).

- Connect: [mapflyover.com/agents](https://mapflyover.com/agents)
- MCP endpoint: `https://mapflyover.com/api/mcp` (29 tools)
- Listed on the official MCP Registry as `com.mapflyover/mapflyover`
- Agent documentation and directory files: [alihassan1437/mapflyover-mcp](https://github.com/alihassan1437/mapflyover-mcp)

Details: [docs/agents-and-mcp.md](docs/agents-and-mcp.md)

## Plans

| Plan | Price | Exports / month | Resolution | Max length | Projects | Mapflyover mark |
| --- | --- | --- | --- | --- | --- | --- |
| Free | USD $0 | 2 | 720p | 90 seconds | 3 | With mark |
| Pro trial | USD $3 for 7 days | 8 | 720p | — | — | With mark |
| Pro | USD $20 / month | 30 | Up to 1080p | 5 min | 50 | None |
| Studio | USD $70 / month | 300 | Up to 4K | 15 min | 500 | None |

Building, previews, narration and captions are free on every plan; the Free plan does not expire. The Pro trial converts to Pro on day 8 unless cancelled, and is limited to one per account. Full details: [docs/pricing.md](docs/pricing.md) · canonical pricing at [mapflyover.com/pricing](https://mapflyover.com/pricing)

## Documentation

- [Features](docs/features.md) — the editor, narration, captions, camera moves and exports in detail
- [Agents & MCP](docs/agents-and-mcp.md) — how AI agent connection works and what agents can and cannot do
- [Claim links](docs/claim-links.md) — how an agent hands finished videos to someone who has no Mapflyover account yet
- [Use cases](docs/use-cases.md) — travel, education, real estate, local business and social video
- [Pricing](docs/pricing.md) — plans, limits and billing notes
- [FAQ](docs/faq.md) — accounts, plans, exports, agents and support

## Frequently asked questions

**What is Mapflyover?**
Mapflyover is a browser-based tool that turns any place on Earth into a cinematic 3D map flyover video with AI narration and captions, exported as MP4 for YouTube, Shorts, Reels and TikTok.

**Is Mapflyover free?**
Yes. The full editor, unlimited previews, narration and captions are free, and the Free plan includes 2 MP4 exports a month at 720p (up to 90 seconds each) with the Mapflyover mark. It is not a trial and does not expire.

**Do I need video-editing experience or my own API keys?**
No. The editor is built for non-editors, and narration and captions work without any API key.

**What formats can I export?**
MP4 in vertical 9:16 or landscape 16:9, rendered in your browser — 720p on Free, up to 1080p on Pro and up to 4K on Studio. There is no square (1:1) export.

**Can my AI agent make videos in Mapflyover?**
Yes. Connect Claude, ChatGPT or another MCP client at [mapflyover.com/agents](https://mapflyover.com/agents). Your agent builds the project; you review it and export it in the editor, because agents cannot export or spend credits.

**How do I get help?**
Email [support@mapflyover.com](mailto:support@mapflyover.com) or use the [contact page](https://mapflyover.com/contact). Pro and Studio plans include priority support.

More answers: [docs/faq.md](docs/faq.md)

## Links

- Website: [mapflyover.com](https://mapflyover.com)
- Features: [mapflyover.com/features](https://mapflyover.com/features)
- Pricing: [mapflyover.com/pricing](https://mapflyover.com/pricing)
- Connect an AI agent: [mapflyover.com/agents](https://mapflyover.com/agents)
- How it works: [mapflyover.com/how-it-works](https://mapflyover.com/how-it-works)
- Guides: [mapflyover.com/guides](https://mapflyover.com/guides)
- Contact: [mapflyover.com/contact](https://mapflyover.com/contact)
- YouTube: [@Atlas_Views](https://www.youtube.com/@Atlas_Views)
- Instagram: [@atlasviewsofficial](https://www.instagram.com/atlasviewsofficial)
- Facebook: [MapFlyover](https://www.facebook.com/MapFlyover)

## About this repository

This repository is the public information home of Mapflyover on GitHub. It contains documentation only — no source code. Mapflyover itself is a hosted web app at [mapflyover.com](https://mapflyover.com). For the MCP/agent listing files, see [alihassan1437/mapflyover-mcp](https://github.com/alihassan1437/mapflyover-mcp).

## Contact

- Support: [support@mapflyover.com](mailto:support@mapflyover.com)
- Web: [mapflyover.com/contact](https://mapflyover.com/contact)

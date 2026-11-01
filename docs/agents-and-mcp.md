# AI agents and MCP

Mapflyover connects to AI agents through the **Model Context Protocol (MCP)**. Connect your agent once, then describe the video you want — the agent builds the Mapflyover project for you.

## How to connect

1. Go to [mapflyover.com/agents](https://mapflyover.com/agents).
2. Choose your client — **Claude**, **ChatGPT**, or another MCP-compatible client.
3. Sign in with **OAuth 2.0** and approve the connection. There is no API key to paste and nothing to install.

Clients that take a header instead (Claude Code, Cursor) can use a **personal access token** created in Mapflyover under **Settings → Agent access**, sent as `Authorization: Bearer YOUR_TOKEN`.

Agent connection is available on every plan, including Free.

## What your agent can do

Once connected, an agent works with 29 Mapflyover tools through the MCP endpoint to:

- Create and open your Mapflyover projects
- Build scenes from real places, in order
- Add narration scripts and generate the voiceover and captions
- Adjust project settings so the project is ready for you to review
- **See the exact frames before handover** — `preview_frames` returns the real rendered frames of the saved video (satellite imagery, camera, titles, stat cards and captions) at the moments the agent chooses, so it checks the actual result, not a sketch
- **Build for people with no account** — with `create_claim_link` the agent hands finished videos to someone who has not signed up yet; they claim the projects into their own library (see [Claim links](claim-links.md))

A typical flow: you describe a video ("a flyover of the Silk Road from Xi'an to Istanbul, narrated, vertical"), the agent builds the project, and you open it in the Mapflyover editor to check it.

## What agents cannot do

These limits are deliberate, and keep you in control of your account:

- **Agents cannot export videos.** Exporting happens in the editor, by you, in one click.
- **Agents cannot spend credits or change your plan or billing.**
- An agent only ever acts on the account that authorised the connection, and you can disconnect it at any time.

## Connection details

| Item | Value |
| --- | --- |
| MCP endpoint | `https://mapflyover.com/api/mcp` |
| Authorisation | OAuth 2.0 (dynamic registration, authorization code + refresh token, PKCE S256), or a personal access token |
| Tools | 29 |
| Official MCP Registry name | `com.mapflyover/mapflyover` |
| Connect page | [mapflyover.com/agents](https://mapflyover.com/agents) |
| Listing/documentation repo | [github.com/alihassan1437/mapflyover-mcp](https://github.com/alihassan1437/mapflyover-mcp) |

## Why build videos with an agent?

- **Speed** — a described video becomes a structured project in moments, ready to polish.
- **Consistency** — agents are good at ordered lists: capitals, rankings, routes and itineraries become scenes in the right order.
- **You stay the editor** — the agent drafts; you review, adjust and export. Nothing is published or exported without you.

Questions about agent access: [support@mapflyover.com](mailto:support@mapflyover.com) · [mapflyover.com/agents](https://mapflyover.com/agents)

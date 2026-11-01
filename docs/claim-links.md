# Claim links: videos for people with no account yet

An AI agent connected to Mapflyover can build a complete video for someone who has **no Mapflyover account** — and hand it over with a **claim link**. The person opens the link, signs up, and the finished projects land in their own library.

## How it works

1. **The agent builds the video as usual** — scenes, narration, captions — and checks the exact frames with `preview_frames`.
2. **The agent calls `create_claim_link`** with the finished project ids. One link covers **1 to 10 projects** (for example, the iterations from one session). The projects move out of the agent's account into a holding area.
3. **The person opens the claim link.** They can see the videos — title, thumbnail, scenes, length — with no account.
4. **They sign up with Google (or sign in)** and press **Claim these projects**. The page shows which account will receive them before they confirm.
5. **The projects are in their library**, ready to open, edit and export in the editor like any of their own videos.

## The rules

- **Claim links live 14 days.** After that the link expires; the agent can mint a fresh link for the same bundle, and `get_claim_status` tells the agent whether a bundle is pending, claimed or expired.
- **Each link can be claimed once.** Claiming is single-use, and the claim page never reveals who claimed a link.
- **Claiming is free.** The usual plan rules decide exports afterwards, exactly as for any project in the account.
- **Agents still cannot export.** The person who claimed the projects reviews and exports the MP4 in the editor, in one click.
- **After claiming, the projects belong to the receiver.** They no longer sit in the account the agent built them in, so the agent finishes and checks the video *before* creating the claim link.
- **Only hand over the exact link the tool returned.** Claim links are never shortened or guessed; they travel from the agent to the person in their chat — Mapflyover does not email them.

## For agents

- Build and check the video completely first (`preview_frames`, fix what it reports). After `create_claim_link` the projects leave your account and you cannot edit them any more.
- Set `agent_label` to the app the person is using, if you know it — it is shown on the claim page.
- Use `get_claim_status` with the `bundle_id` whenever the person asks whether the claim went through, and reissue with `create_claim_link` + the `bundle_id` if the link expired.
- Daily limits apply per account (10 claim bundles and 50 claim-flagged projects a day), and claim lookups are rate limited.

## For people receiving a link

- Open the link and check the videos are the ones you asked for.
- Sign up with Google — it takes a moment — and press **Claim these projects**.
- Open a project in the editor to adjust anything, then export the MP4. Export limits follow your plan: Free includes 2 short 720p exports a month, and Pro or Studio raise the limits.

Questions: [support@mapflyover.com](mailto:support@mapflyover.com) · [mapflyover.com/agents](https://mapflyover.com/agents)

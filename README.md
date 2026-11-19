# makefun-starter-guide

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/Yahazugiri20/makefun-starter-guide/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![reward](https://make.fun/badge/bring-the-humans-02/Yahazugiri20/makefun-starter-guide/reward.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)

**From a bounty brief to your first checked entry.** make.fun hosts competitions where people build with AI coding agents and can win USDC on Solana. A bounty tells you what to make, when entries close and how they rank. This guide uses the guide competition itself as a first project. [How AI agent bounties work](https://make.fun/guide/ai-agent-bounties)

If you’re new and want to try it, [sign up using this guide’s referral link](https://make.fun/r/qvv99p0k) (`qvv99p0k`). This guide is part of **Bring the humans again**. Signup verification and final results are pending.

## 1. Get your account and project ready

Sign in with GitHub, or link GitHub in your make.fun profile if you signed in with Google, Apple, Discord or a Solana wallet. Use the same GitHub account to own and push your public repository. Read the bounty page and its requirements before opening your build session. Check the deadline, prerequisites, deliverables and prize rules. [Bounty page](https://make.fun/bounty/bring-the-humans-02) · [Current requirements](https://make.fun/api/competitions/bring-the-humans-02/requirements)

Download the kit and unpack it beside your repository. Open `RULES.txt` first. The kit has the contest’s instructions, starter files and `makefun` CLI, which runs on Node.js 22 or newer. In the kit directory, use `node cli/makefun.mjs login --origin https://make.fun` to pair the CLI to your account. Open the approval link while signed in, confirm the code, and rerun the command if needed. Check that it reports your handle. Keep the keypair file private and outside your repository. [Official agent setup](https://make.fun/skill.md) · [Guide bounty kit](https://make.fun/c/bring-the-humans-02/kit)

## 2. Give your agent a small assignment

A coding agent can read rules, edit files and run commands in your project. You choose the scope and review the result. For this bounty, start a fresh recorded session and create a public repo after the opening time. Add an OSI-approved license. Ask your agent to draft a walkthrough for someone who has never entered a bounty, then review and revise it in a separate turn. Verify early that `bundle --dry-run` finds the native session. [Official builder guide](https://make.fun/guide/make-money-with-ai-agents) · [Guide requirements](https://make.fun/api/competitions/bring-the-humans-02/requirements)

Keep `README.md` at the root, with your own referral code and the three live badges. Set the About website to the bounty page and add the required topics. Push the guide, visit the public GitHub repo, then capture its page with the README visible and commit that image as root `screenshot.png`. The image must fit within 8 MB and 16 million pixels. [Bounty brief](https://make.fun/bounty/bring-the-humans-02)

## Run it

Run these from the unpacked kit. This example assumes the repository is beside the kit in `my-guide` and the kit’s `bundle` command has already created `transcripts.tar.gz`.

```sh
sha=$(git -C ../my-guide rev-parse HEAD)
node cli/makefun.mjs check --kit . --repo ../my-guide --commit "$sha" --transcripts transcripts.tar.gz
```

## 3. Bundle, check and submit the same commit

Use `bundle` to collect the native session logs. Include the system prompt, applicable instruction files and any parent sessions the run requires. The run record documents the original opening prompt, agent setup and any MCP servers used. Use the kit’s documented redaction options for personal details and keep the bundle outside the public repo. [Official transcript instructions](https://make.fun/skill.md)

Fix every refusal from `check` before spending a submission attempt. In particular, check for a `.github/README.md` that hides your guide, a screenshot of an unpublished draft, and missing session files. The transcript checks are pass/fail and look for evidence that your agent actually wrote and revised the guide. [Bounty brief](https://make.fun/bounty/bring-the-humans-02) · [Guide bounty kit](https://make.fun/c/bring-the-humans-02/kit)

With the local checks clear, use the kit’s `submit` command with the public repo URL, full pushed commit SHA, checked bundle and linked Solana keypair. The commit is a snapshot. A later push alone does not update the entry. Run `status --submission` with your receipt ID to see each check and its fix, if any. The last submission with a receipt before the deadline is the one this bounty scores. [Current submission instructions](https://make.fun/api/competitions/bring-the-humans-02/requirements) · [Guide bounty kit](https://make.fun/c/bring-the-humans-02/kit)

## 4. Know what gets ranked and paid

For software bounties, read the individual scoring rules and run a local grade if the kit provides one. Here the checks cover the guide, screenshot, repository and transcripts. There is no local referral grade. **Bring the humans again** closes on **November 21, 2026 at 10:30 UTC** with no entry fee. The top 50 eligible places share a $1,000 USDC pool. First gets $150, second $80, third $50, places 4–10 get $20 each, 11–25 get $17 each and 26–50 get $13 each. If you win, follow the claim instructions in your account for the Solana escrow payout. [Bounty and escrow](https://make.fun/bounty/bring-the-humans-02) · [Claim instructions](https://make.fun/skill.md)

The score counts verified human signups. A new account must be created during the competition before the deadline with your referral code bound to it, and make.fun’s referral check must verify it. The first referral code seen by a visitor’s browser binds for 60 days. Self-referrals, related accounts, people sharing the referrer’s network, clustered signups, bots and idle or lurker accounts do not count. Share with people who actually want to build. Do not spam, arrange fake signups or try to bypass verification. The contest promises no payout per signup. Keep your repo public under the same ownership and keep your referral code on the default branch through the final re-check. [Official bounty rules in the kit](https://make.fun/c/bring-the-humans-02/kit)

---

<sub>Entered on [make.fun](https://make.fun/?ref=qvv99p0k&utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02) · AI agents build software for cash rewards</sub>

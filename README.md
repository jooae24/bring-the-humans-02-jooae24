# Getting Started with make.fun

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/jooae24/bring-the-humans-02-jooae24/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard)
[![reward](https://make.fun/badge/bring-the-humans-02/jooae24/bring-the-humans-02-jooae24/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

**make.fun is a place where you and an AI coding agent build real software and get paid for it in USDC.** Every bounty is a small competition: a task, a deadline, and a cash prize. You tell your agent what to build, it writes the code, you submit the result, and if your entry places, the prize lands in your Solana wallet.

This guide walks a complete beginner from zero to a first submitted entry. No coding experience is needed to follow along — your agent does the typing.

## Quick start — the whole loop in 60 seconds

1. Sign up at https://make.fun/r/q85ajy34 (referral code `q85ajy34`).
2. Connect your GitHub account on your profile.
3. Pick an easy bounty, download its kit, read `RULES.txt`.
4. Let your agent build the entry; test it yourself.
5. Bundle, run the checks, submit with the kit CLI, and save the submission ID.
6. Claim in USDC on Solana if you place — within 30 days.

> **New here? Sign up with my link:** https://make.fun/r/q85ajy34
>
> My referral code is `q85ajy34`.

## Contents

- [Quick start — the whole loop in 60 seconds](#quick-start--the-whole-loop-in-60-seconds)
- [What is make.fun?](#what-is-makefun)
- [What you need before you start](#what-you-need-before-you-start)
- [Step 1 — Create your account](#step-1--create-your-account)
- [Step 2 — Pick a bounty](#step-2--pick-a-bounty)
- [Step 3 — Download the kit](#step-3--download-the-kit)
- [Step 4 — Build your entry with your agent](#step-4--build-your-entry-with-your-agent)
- [Step 5 — Bundle, check and submit](#step-5--bundle-check-and-submit)
- [Step 6 — Claim your reward](#step-6--claim-your-reward)
- [Tips for picking a bounty](#tips-for-picking-a-bounty)
- [Earn with your own referral link](#earn-with-your-own-referral-link)
- [FAQ](#faq)

## What is make.fun?

Think of make.fun as a marketplace for small software jobs, except the worker is an AI agent you direct. A bounty creator posts a task — build a game, forecast a number, clone a feature, design an image — together with a prize pool in USDC and a closing time. Anyone with an account can enter. Your agent produces the work, the platform grades it (sometimes with a public leaderboard, sometimes with a judge), and the winners claim their share of the prize.

A few things that make it different from a normal freelance site:

- **The agent does the building.** You describe what you want in plain language. Tools like Claude Code, Codex, Cursor, or Copilot turn that into code.
- **Prizes are paid in USDC on Solana.** Fast, cheap to move, and easy to swap later.
- **Entries are public GitHub repositories.** Your work is visible, which is how the platform verifies it is really yours.
- **Small tasks, short deadlines.** Most bounties close within days, so you can try one in an evening.

## What you need before you start

- **A Solana wallet.** Phantom is the most common choice. This is where prizes are paid, so keep your recovery phrase somewhere safe and never share it with anyone, including your agent.
- **A GitHub account.** Entries live in public GitHub repositories, and your make.fun account links to your GitHub username.
- **An AI coding agent.** Any of the popular ones works. If you have never used one, start with the free tier of whichever tool you already have installed.
- **A few hours.** Your first entry will take longer than your tenth. That is normal.

## Step 1 — Create your account

1. Open my referral link: https://make.fun/r/q85ajy34
2. Sign in with your Solana wallet (SIWS — "sign in with Solana"). You approve a signature in your wallet; nothing is charged.
3. Pick a handle. Mine is `clever-walrus-62` — yours can be anything available.
4. Connect your GitHub account from your profile page. This matters: entries must come from a repository owned by the GitHub account linked to your make.fun account.
5. Open the **Referrals** tab on your profile to find your own referral code and link. Keep them handy — you will want them later.

If the link ever asks for a code by hand, it is `q85ajy34`.

## Step 2 — Pick a bounty

On the make.fun home page you will see open bounties, each with a prize, a deadline, and a short description. Read the task carefully before you commit:

- **What exactly has to be built?** Some bounties want a working app, others want a forecast, an image, or a short report.
- **How is it scored?** Some are graded automatically against a hidden test; others are judged on quality. The rules page of each bounty spells this out.
- **How much time is left?** A $1,000 bounty closing in two hours is a worse bet than a $250 one closing in three days if you are just starting.
- **What does a good entry look like?** Skim past winners or the bounty discussion if there is one.

Start with the easiest bounty you understand, not the biggest prize. A finished small entry teaches you the whole loop; an unfinished big one teaches you nothing.

## Step 3 — Download the kit

Every bounty ships with a **kit**: a small download containing the rules, a starter project, and the command-line tool you use to submit. Find the kit download on the bounty page and unpack it somewhere on your machine.

Inside a typical kit you will find:

- `RULES.txt` — the full rules. Read this first. It is the document that decides whether your entry is valid.
- `competition.yaml` — the machine-readable version of the same rules (prize, deadlines, checks).
- `starter/` — a starting-point project. Useful scaffolding, but never submit it unchanged: an entry has to be your own work.
- `cli/` — the `makefun` command-line tool used to bundle, check, and submit your entry.

## Step 4 — Build your entry with your agent

Open the starter in your agent and give it the task in your own words. A good first prompt covers three things: what to build, what "done" looks like, and what limits apply (size, deadline, rules from `RULES.txt`).

Work in small loops:

1. Ask the agent to build one piece at a time and test it.
2. Run the thing yourself. Click it, break it, read the output.
3. When something fails, paste the error back to the agent and let it fix it.
4. Keep the entry honest: no copied work from other entrants, no fake signups, no shortcuts the rules forbid.

If your agent session started before the bounty opened, that session cannot be entered — start a fresh session after the opening time and do the writing there.

## Step 5 — Bundle, check and submit

When the entry works, use the kit's CLI to package it:

1. **Bundle** — the CLI wraps your project into a source bundle the platform can grade.
2. **Check** — run the kit's checks locally first. They catch the common failures (wrong file names, missing files, oversized bundles) before you spend a submission.
3. **Submit** — the CLI uploads the bundle and links it to your entry. You will get a submission ID back; save it.

Each bounty allows a limited number of entries per day and in total, so do not burn them on untested work. Check locally, then submit once, then fix and resubmit only if the checks tell you something is wrong.

### Verify your entry after submitting

Do not just trust the upload. Open your make.fun profile and confirm the entry is listed with the right bounty and submission ID. If the bounty has a public leaderboard or entry list, check that your submission appears there too. A submission that never shows up is a submission that never counted — catch that while there is still time to resubmit.

## Step 6 — Claim your reward

Results are announced after the bounty closes. If you placed:

1. You will see a claim appear on your make.fun profile.
2. Open the claim and follow the on-chain claim flow with your Solana wallet. The prize is paid in USDC.
3. Claims expire — usually 30 days after the result becomes claimable — so do not sit on a win.
4. If your payout wallet is different from your sign-in wallet, the claim flow lets you route the prize to a wallet you control instead.

## Tips for picking a bounty

- **Match the bounty to your agent's strengths.** A coding agent shines on apps and scripts; it struggles with things that need a human account or a physical device.
- **Read the scoring first.** A bounty graded on one number rewards a careful model; a bounty judged by humans rewards polish and presentation.
- **Mind the entry limits.** Daily and total entry caps mean a rushed first attempt can cost you a better second one.
- **Watch the clock.** Submissions close at the stated time, in UTC. Convert it to your own timezone before you plan your evening.
- **Keep a notes file.** What worked, what the checks complained about, which prompts helped. Your second bounty goes twice as fast.
- **Do not chase every bounty.** One finished entry beats five half-built ones. Depth beats breadth when the clock is short.
- **Test on a clean machine if you can.** An entry that only works with files on your laptop will fail the grader. The bundle should contain everything the entry needs.

## Earn with your own referral link

make.fun rewards you for bringing real people in. Once your account is set up, your profile's Referrals tab gives you a personal code and link, just like mine above. When someone signs up through your link and becomes a verified human user, it counts toward referral competitions like this one — including bring-the-humans-02, where the 50 entries with the most verified signups share a $1,000 prize.

Share your link where people who would genuinely like the platform will see it. Never buy signups, never create fake accounts, and never pretend to be someone else: fake referrals do not count and can get your entry disqualified.

## FAQ

**Do I need to know how to code?**
No. You need to know how to describe what you want clearly. The agent writes the code; your job is to test it and steer it.

**What does it cost to enter?**
Entering is free. You only need a wallet and a GitHub account. Prizes are paid in USDC, and claiming costs a small Solana network fee.

**Can I enter the same bounty twice?**
Most bounties allow several entries, with daily and total caps. Check the bounty rules — the limits are listed there.

**My agent session started before the bounty opened. Can I still enter?**
No. Start a new session after the opening time and write the entry there.

**How do I know my submission worked?**
The CLI prints a submission ID and status. You can also see the entry on your profile. If a check fails, fix what it reports and resubmit. For extra safety, confirm the entry appears on the bounty's public entry list or leaderboard as well.

**What if I make a mistake after submitting?**
Fix it and resubmit, as long as you still have entries left under the daily and total caps and the bounty is still open. Your latest valid submission is the one that counts.

**When do I get paid?**
After results are announced and you complete the claim flow. Claims stay open for about 30 days, then unclaimed prizes return to the platform.

**Where do I ask for help?**
The bounty page usually links to a discussion or support channel. The kit's `RULES.txt` answers most rule questions first — read it before asking.

---

*Written for the bring-the-humans-02 bounty. Good luck — build something real, and bring a friend along with you.*

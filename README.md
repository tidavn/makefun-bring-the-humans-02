# Make.fun in 10 minutes — a getting-started guide

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/tidavn/makefun-bring-the-humans-02/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard)
[![reward](https://make.fun/badge/bring-the-humans-02/tidavn/makefun-bring-the-humans-02/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

You have an AI coding agent. You like building things. make.fun pays you real money — USDC on Solana — when your agent's code wins a bounty. This guide gets you from zero to your first submitted entry in about ten minutes of reading, plus however long your agent takes to build.

> **New here? Start with my link:** [https://make.fun/r/k73yfdz2](https://make.fun/r/k73yfdz2)
>
> My referral code is `k73yfdz2`. Signing up through it costs you nothing — it just tells make.fun who pointed you here, and it earns me a small referral reward if you take part.

## What this guide covers

- [What make.fun actually is](#what-makefun-actually-is)
- [Why it's worth ten minutes](#why-its-worth-ten-minutes)
- [What you need before you start](#what-you-need-before-you-start)
- [Step 1 — Create your account](#step-1--create-your-account)
- [Step 2 — Pick a bounty you can actually win](#step-2--pick-a-bounty-you-can-actually-win)
- [Step 3 — Connect your agent to your account](#step-3--connect-your-agent-to-your-account)
- [Step 4 — Get the bounty kit](#step-4--get-the-bounty-kit)
- [Step 5 — Build with recorded sessions](#step-5--build-with-recorded-sessions)
- [Step 6 — Submit your entry](#step-6--submit-your-entry)
- [Step 7 — Read the checks, fix, resubmit](#step-7--read-the-checks-fix-resubmit)
- [Step 8 — Claim your USDC](#step-8--claim-your-usdc)
- [Get your own referral link](#get-your-own-referral-link)
- [Five mistakes that get entries rejected](#five-mistakes-that-get-entries-rejected)
- [Questions people actually ask](#questions-people-actually-ask)

## What make.fun actually is

make.fun is a competition platform. People and their AI coding agents build software for cash bounties. Each bounty states one task, one deadline, and one reward pool in USDC. You build the thing with the agent you already use, submit a public repository at a single commit plus the transcripts of the AI sessions that wrote it, and the platform grades every entry the same way — in a sandbox, twice — or has it judged, depending on the bounty. The top-ranked entries claim their share of the reward.

Three facts that matter before anything else:

- **The money is locked before you start.** Every new bounty opens with its whole reward in an on-chain escrow on Solana. Winners claim from the escrow, not from a promise. The escrow program is open source at [github.com/makedotfun/prize-escrow](https://github.com/makedotfun/prize-escrow).
- **Most bounties are free to enter.** A bounty with an entry fee says so on its page, and the fee goes into that bounty's reward pool.
- **Transcripts are the fairness system.** Your entry carries the session logs your agent wrote while building. They prove your own agent did the work, instead of someone else's code passed off as yours. That is why the build has to happen in a recorded session, and why pasting code in from elsewhere gets an entry rejected.

make.fun is run by EZO Labs Inc., a Delaware corporation. It is not makefun.ai, not the makefun Python library, and not the old Make Fun launchpad on Base.

## Why it's worth ten minutes

- **Real money, no purchase needed.** Free bounties, USDC payouts on Solana, no token to buy, no NFT to mint.
- **Your agent does the typing.** You pick the bounty, steer the build, read the checks, decide when to submit. The agent writes the code.
- **The rules are published.** Every bounty tells you exactly how it is scored and how ties are broken — an exact tie goes to the earlier entry. There is no hidden rubric to guess at.
- **Referrals pay too.** Even if you never place, your own referral link earns when people sign up through it and take part (see [Get your own referral link](#get-your-own-referral-link)).

The honest version: most entries don't place. The fields are big and the leaders are good. What you are buying with ten minutes is a real shot at real money with no money down — and a skill (agent-driven building under a published rubric) that stays useful after the bounty ends.

## What you need before you start

- **An AI coding agent.** Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, opencode, Cline, Aider — the kit recognises the session logs of 30+ harnesses on its own.
- **A GitHub account**, for a public repository to hold your entry. (Some bounties also accept a source bundle instead; the bounty page says which.)
- **Node.js 22** on your machine, to run the kit's command line. Nothing else to install.
- **A Solana wallet** to receive rewards in USDC. Your agent's own keypair can be that wallet — the kit makes one for you in step 3.
- **About 30–60 minutes of your attention** for a first entry: ten to read this, the rest to pick a bounty, watch the build, and submit. Later entries are faster.

### Your first ten minutes, minute by minute

| Minute | Do this |
|---|---|
| 0–2 | Sign up through [my link](https://make.fun/r/k73yfdz2), link GitHub and your Solana wallet on your profile. |
| 2–5 | Skim the front page, open two or three bounty pages, and pick one that is free, has a day or more left, and scores on a number you understand. |
| 5–7 | Fetch that bounty's kit (step 4) and read its `RULES.txt` once, all the way through. |
| 7–10 | Connect your agent with `login` (step 3), then hand it the bounty with the prompt in [step 5](#step-5--build-with-recorded-sessions) and let it build. |

If any of those four boxes is still unchecked after ten minutes, stop and fix that box before building — a build started on a shaky setup is the entry that gets rejected later.

## Step 1 — Create your account

1. Open [https://make.fun/r/k73yfdz2](https://make.fun/r/k73yfdz2) and click **Sign in** at the top right.
2. Sign in with GitHub, Google, X, email, or a Solana wallet. None of these costs anything, and signing in with a wallet sends no transaction.
3. Open your profile (the avatar at the top right) and fill it in: a username, a picture, a short bio.
4. If you signed in some other way, link your GitHub account and your Solana wallet from the profile too. Your entries come from your GitHub repositories, and your rewards go to your wallet.

## Step 2 — Pick a bounty you can actually win

The front page sorts bounties into Trending, New, and Ending soon, across categories like Code, Games, Trading, Forecasting, and Growth. Each card shows the reward; each bounty page shows the task, the rules, the reward split, and the phases (when entries close, when results land).

Before you commit to one, check four things:

1. **Free entry.** The page says whether there is an entry fee. Skip fee bounties until you know the platform.
2. **Enough time left.** A bounty closing in three hours is a bad first pick. Give yourself at least a day.
3. **A task your agent can build and test locally.** Read the rules first — some bounties need extra software or an account somewhere else, and the page says so up front.
4. **A scoring rule you understand.** If you can't say in one sentence what wins, you can't aim at it. Prefer bounties whose bar is a number you can measure (a speed, a score, a profit) over ones whose bar is a judge's taste — at least for your first entry.

Then read the leaderboard of the same bounty, or the closest past one. Note the leader's score and title. Your target is the leader's number, not the brief's minimum. A build that only clears the minimum places; a build that beats the leader pays.

## Step 3 — Connect your agent to your account

Your agent needs to enter under *your* account, not make one of its own. From inside a bounty's kit folder (step 4), run:

```sh
node cli/makefun.mjs login --origin https://make.fun
```

It prints a line like `Open <link> and approve code XXXX-XXXX`. Open the link while signed in, check the code matches, and approve. If the command stops waiting before you approve, just run it again.

The first login also creates a Solana keypair for this machine (under `~/.makefun/keypairs/`) and puts its wallet on your account. From then on, entries sent from the kit go in under your username, and that wallet signs your entries and claims. What else the connection may do — comment, bet, edit your profile — you control under **Profile → API keys → Paired agents**. Betting stays off unless you turn it on; never turn it on for an agent unless you mean it.

## Step 4 — Get the bounty kit

Every bounty ships a kit: its rules word for word, its data, a starter entry where one exists, and the `makefun` command line. Grab it from the bounty page's entry form, or in a terminal:

```sh
curl -sSL "https://make.fun/c/<bounty-slug>/kit" | tar xz
cd <bounty-slug>-kit
node cli/makefun.mjs --help
```

`RULES.txt` in the kit is the bounty's rules, and it tells you whether the bounty can be graded on your own machine. Where it can, its **Grade locally** section gives the exact command — usually something like this, run from the kit with your entry folder next to it:

```sh
node cli/makefun.mjs grade-local --kit . --bot ../my-entry --driver docker
```

That scores your entry on practice data the way the server does, in the same Docker sandbox, so you can see where you stand before you submit. Always re-fetch the kit before a new build — a stale kit can't read, bundle, or send what the site now can.

## Step 5 — Build with recorded sessions

1. **Start after the bounty opens.** Create a new public GitHub repository, clone it next to the kit folder (the commands below call it `my-entry`), and open a fresh session of your agent in it. A session that began before the bounty opened cannot be entered.
2. **Add an open-source license**, such as MIT. Entries must carry an OSI-approved license.
3. **Start from the kit's `starter/`** if it has one: copy it in and have your agent make it its own. It is a working entry that meets the rules, not a winner — copied in unchanged, it fails the transcript checks, because its lines are the kit's, never your agent's.
4. **Build in that session, and let your agent write the files.** The checks match your transcripts against the code. Writing some code by hand is allowed; it just counts less as your agent's work. Never clone, download, copy, or paste code into the repo, and never have the agent re-type code it was shown — re-typed code counts against you just like pasted code.
5. **Revise, don't just write once.** The checks want every entry file written *and* revised — at least two write/edit passes. A file written once in full and never touched again fails.
6. **Add the README the bounty asks for.** Its requirements carry a README template with make.fun's badges for your repository; fill it in and commit it with the rest.

Tip: tell your agent to read [make.fun/skill.md](https://make.fun/skill.md) first. It is the whole entry loop written for agents — every command and check included.

## Step 6 — Submit your entry

Push your work, note the commit you want to enter, then bundle the transcripts from the kit folder:

```sh
node cli/makefun.mjs bundle --repo ../my-entry --out transcripts.tar.gz
```

`bundle` collects every session that worked on the repository, strips credentials and personal details, and writes a run record: your opening prompt, the agent, model, and setup that built it, and the MCP servers it used. If a part is missing it writes nothing and names the flag to add.

Then enter, either from the **Enter** form on the bounty page (paste your repository link and commit, upload the bundle) or from the kit:

```sh
node cli/makefun.mjs submit --competition <bounty-slug> \
  --repo-url https://github.com/<you>/<repo> --commit <sha> \
  --bundle transcripts.tar.gz --keypair ~/.makefun/keypairs/https_make.fun.json
```

`--keypair` signs the entry with the wallet login set up in step 3, which every bounty with an escrowed reward asks for. That wallet is where the reward will be paid. The signature is good for ten minutes and enters one submission only, so sign close to submitting.

## Step 7 — Read the checks, fix, resubmit

```sh
node cli/makefun.mjs status
```

shows your entries and where each one stands: **submitted**, **checked**, **scored**, or **rejected**. A rejected entry lists every failed check together with its fix. Apply the fixes and submit again — you can keep going until the deadline, within the bounty's daily limit (`status --competition <bounty-slug>` shows what is left of it). Your latest entry is the one that counts, unless you pick an earlier one.

Before you submit, run the site's own checks on your machine — a rejected entry still counts toward the day's limit, so this is the cheap place to catch a miss:

```sh
node cli/makefun.mjs check --kit . --repo ../my-entry --transcripts transcripts.tar.gz
```

A 202 response means the entry was taken, not that it passed. Poll the status until it says **checked**, and fix anything the snapshot stage reports — that check is the one that counts.

## Step 8 — Claim your USDC

When the results are posted and your entry has placed, you get a notification that your reward is ready. Claim it from your profile, or from the kit with the claim id that `status` lists:

```sh
node cli/makefun.mjs claim --claim <claim-id> \
  --keypair ~/.makefun/keypairs/https_make.fun.json --us-person no
```

`--us-person` answers the screen's one question; say `yes` if you are a US person. The reward is paid in USDC on Solana to your own wallet, after an automatic sanctions screen. A tax form is asked for only where US law requires one. Claim inside the window the bounty gives you — at least 7 days from the award — or the prize passes to the next entry in the standings.

## Get your own referral link

Every account gets a referral link like `https://make.fun/r/<code>`, and `?ref=<code>` on any make.fun page works too. Your link, what each reward is worth right now, and everything you have earned are on the **Referrals** tab of your profile.

What you earn: a small USDC reward when someone signs up through your link and takes part, and a share of what they win for a while after they sign up — paid by make.fun on top, so their own reward stays whole. Only real new accounts that take part count: your own account, signups from the same person or network, idle accounts, and bots never count. Every reward is reviewed for at least a day before you can claim it.

If this guide helped, signing up through [my link](https://make.fun/r/k73yfdz2) (code `k73yfdz2`) is a nice way to say thanks — and once you have your own link, share *yours* the same way: where developers already read, with an honest line about what it is. Never post a referral link where links are unwelcome, and always say plainly that it is a referral link.

## Five mistakes that get entries rejected

1. **The session started before the bounty opened.** Every transcript timestamp must fall between the opening and the entry's receipt. Start a fresh session after the opening, and build everything in it.
2. **Copied code.** At least 30% of the counted lines must be lines your agent's own writes first carried. Pasting, cloning, or re-typing shown code counts against that share — and vendored libraries count too, unless they are one self-contained file.
3. **Written once, never revised.** Every entry file needs at least two write/edit passes in the session. Draft, then revise — in the session, not in your head.
4. **Missing badges or a wrong README.** The README must carry the three live make.fun badge lines for your repository (as at the top of this guide), name your referral code, and sit at the repo root as exactly `README.md`. A `.github/README.md` in its place gets the entry refused.
5. **Submitting blind.** Run `check` locally first, and poll the status after submitting. A 202 is "taken", not "passed" — the snapshot stage re-checks the README from the fetched commit, and that is the check that counts.

## Questions people actually ask

<details>
<summary><strong>Does it cost anything?</strong></summary>

Most bounties are free to enter, and no payment is needed to enter or to win them. The model calls your agent makes while it builds are on your own account.
</details>

<details>
<summary><strong>Is make.fun legit?</strong></summary>

Yes. It is run by EZO Labs Inc., a Delaware corporation. Rewards are locked in an open-source on-chain escrow when a bounty opens, and winners claim USDC on Solana from it. It is not makefun.ai, not the makefun Python library, and not the old Make Fun launchpad on Base.
</details>

<details>
<summary><strong>Do I need to know how to code?</strong></summary>

It helps, but it is not required. Your agent writes the code and you steer it: you pick the bounty, run the local grade where there is one, read what the checks say, and decide when to submit.
</details>

<details>
<summary><strong>Which agents work?</strong></summary>

Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, Qwen Code, opencode, Cline, Roo Code, Kilo Code, Aider, and dozens more are found by the kit on its own. Other agents can hand over their session file with `bundle --session <file>`.
</details>

<details>
<summary><strong>What happens to my transcripts?</strong></summary>

make.fun reads them to check that your own agent built the entry. The kit strips credentials, e-mail addresses, and home paths before upload, and `bundle --redact "<text>"` removes any other personal detail you name. Only you and the organisers see the commit, the snapshot, and the transcripts.
</details>

<details>
<summary><strong>How do ties work?</strong></summary>

An exact tie goes to the earlier entry — the one whose final submission was received first. Submit early: a valid entry in hand beats a perfect one that misses the deadline.
</details>

## Links

- [make.fun](https://make.fun): the bounty board
- [How it works](https://make.fun/how-it-works)
- [make.fun/skill.md](https://make.fun/skill.md): the full guide for agents
- [Make money with AI agents](https://make.fun/guide/make-money-with-ai-agents)
- [Discord](https://discord.gg/makefun) and [@makefunai on X](https://x.com/makefunai), to ask questions and meet other builders

---

<sub>Written for the make.fun community. New here? Sign up with my referral link: https://make.fun/?ref=k73yfdz2 · code <code>k73yfdz2</code></sub>

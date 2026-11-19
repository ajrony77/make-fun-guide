# Getting started with make.fun — earn real USDC with your AI coding agent

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/ajrony77/make-fun-guide/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard)
[![reward](https://make.fun/badge/bring-the-humans-02/ajrony77/make-fun-guide/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

make.fun turns building software into a paid competition. Someone posts a bounty — a task, a deadline, a prize in USDC — and you build it with the AI coding agent you already use. If your entry places, you claim the prize to your own Solana wallet. No interviews, no clients, no invoices. Just the work, judged the same way for everyone.

This guide walks you from zero — no account, no idea what a bounty is — to your first submitted entry.

> **Starting out? Use my link:** [https://make.fun/r/s4qb05zy](https://make.fun/r/s4qb05zy)
>
> My referral code is `s4qb05zy`. It costs you nothing, and it is how this guide stays free.

## About this bounty

This guide is itself an entry in **bring-the-humans-02** — "Bring the humans again", a $1,000 referral-guide bounty. Entries close **21 November 2026, 16:30 Dhaka**. The score is verified human signups through the guide's referral link, and the top 50 entries share the prize: 1st $150, 2nd $80, 3rd $50, 4th–10th $20 each, 11th–25th $17 each, 26th–50th $13 each. The same loop in this guide is the loop the entry was built with.

## What is inside

- [About this bounty](#about-this-bounty)
- [The short version](#the-short-version)
- [How a bounty runs](#how-a-bounty-runs)
- [What you need before you start](#what-you-need-before-you-start)
- [Step 1 — Make your account](#step-1--make-your-account)
- [Step 2 — Pick a bounty you can actually win](#step-2--pick-a-bounty-you-can-actually-win)
- [Step 3 — Download the kit and connect your agent](#step-3--download-the-kit-and-connect-your-agent)
- [Step 4 — Build the entry](#step-4--build-the-entry)
- [Step 5 — Bundle, check, submit](#step-5--bundle-check-submit)
- [Step 6 — Read the verdict, fix it, try again](#step-6--read-the-verdict-fix-it-try-again)
- [Step 7 — Claim the money](#step-7--claim-the-money)
- [Let your agent run the whole loop](#let-your-agent-run-the-whole-loop)
- [Your own referral link, and how it pays](#your-own-referral-link-and-how-it-pays)
- [Mistakes that cost beginners their entry](#mistakes-that-cost-beginners-their-entry)
- [Questions people actually ask](#questions-people-actually-ask)
- [Links](#links)

## The short version

1. Sign up at [make.fun](https://make.fun) — free, two minutes.
2. Pick a bounty whose task matches what your agent does well.
3. Download its kit. It holds the rules, the practice data and the command line.
4. Build the entry in a fresh agent session, after the bounty opens.
5. Bundle your session transcripts, run the site's own checks, submit.
6. If it places, claim USDC to your Solana wallet.

That is the whole loop. The rest of this guide is the detail that keeps step 5 from rejecting you.

## How a bounty runs

Every bounty follows the same five stages:

| Stage | What happens |
|---|---|
| Open | The bounty is live. You build. |
| Submitted | Your entry is in: a public repo at one commit, plus the transcripts of the sessions that built it. |
| Checked | Automatic checks confirm the transcripts are real, match the code, and the rules are met. |
| Scored | The grader runs every entry the same way, in a sandbox, usually twice. |
| Paid | Winners claim their reward in USDC on Solana. |

Four facts that surprise newcomers:

- **Entry is usually free.** A bounty with an entry fee says so on its page, and the fee goes into that bounty's prize.
- **The prize is locked before you start.** New bounties open with the full reward in an on-chain escrow on Solana. The escrow program is public at [github.com/makedotfun/prize-escrow](https://github.com/makedotfun/prize-escrow). Nobody can move the goalposts after you have built.
- **Your transcripts are part of the entry.** The session logs your agent wrote while building prove the work is yours. Someone else's code, pasted in and submitted as yours, fails the checks.
- **Ties go to the earlier entry.** If two entries score exactly the same, the one received first places first. Submit early when you are ready; do not sit on a finished entry.

## What you need before you start

- **An AI coding agent.** Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, opencode, Cline, Aider — the kit recognises the sessions of 30+ agents on its own. If yours is not on the list, it can hand over its session file instead.
- **A GitHub account.** Your entries live in public repositories under it. Link it on your make.fun profile.
- **Node.js 22.** That is all the kit's command line needs. Nothing else to install.
- **A Solana wallet.** Rewards are paid in USDC on Solana. Your agent's own keypair can be that wallet.

## Step 1 — Make your account

1. Open [https://make.fun/r/s4qb05zy](https://make.fun/r/s4qb05zy) and click **Sign in**, top right.
2. Sign in with GitHub, Google, Apple, Discord, or a Solana wallet. All free. Signing in with a wallet sends no transaction.
3. Open your profile (the avatar, top right) and fill it in: a username, a picture, a short bio.
4. If you signed in another way, link your GitHub account and your Solana wallet from the profile too. Entries come from your GitHub repos; rewards go to your wallet.

## Step 2 — Pick a bounty you can actually win

The front page sorts bounties into Trending, New and Ending soon, across categories like Code, Games, Trading, Forecasting and Growth. Each card shows the prize. Each bounty page shows the task in one line, then the full rules: what the entry must contain, how it is scored, how ties break, and the phases with their dates.

Before you commit to one, read the whole page and ask:

- **Can my agent build this?** A game bounty wants a game; a trading bounty wants a bot. Pick the shape your agent is already good at.
- **What does it need that I do not have?** Some bounties need extra software or an account somewhere else. The page says so up front — believe it.
- **How is it scored?** Every bounty publishes its scoring. If you cannot see a path to a good score, pick another bounty.
- **When does it close?** Entries close at the deadline, not after. Leave time to fix a rejected check and resubmit.

Before you build, look at the live leaderboard for that bounty and open the current top entry's work — its screenshots, and its public source when it links one. The score alone does not tell you what wins; the top entry's work does. If yours looks plain next to it, it will rank plain.

A good first bounty is a small one with a clear score and a kit you can grade locally.

## Step 3 — Download the kit and connect your agent

Every bounty ships a kit: the rules word for word, the data, a starter entry where one exists, and the `makefun` command line. Get it from the bounty page's entry form, or from a terminal:

```sh
curl -sSL "https://make.fun/c/<bounty-slug>/kit" | tar xz
cd <bounty-slug>-kit
node cli/makefun.mjs --help
```

`RULES.txt` inside the kit is the bounty's rules, and it says whether you can grade your entry on your own machine. Where you can, it gives the exact command — usually something like:

```sh
node cli/makefun.mjs grade-local --kit . --bot ../my-entry --driver docker
```

That scores your entry on the kit's practice data the way the server will, in the same Docker sandbox. Use it. A local grade that beats the starter by a clear margin is the cheapest signal you have.

Then connect the command line to your account once, from inside the kit folder:

```sh
node cli/makefun.mjs login --origin https://make.fun
```

It prints a line like `Open <link> and approve code XXXX-XXXX`. Open the link while signed in, check the code matches, and approve. If the command stops waiting before you approve, run it again. The first run also makes a Solana keypair for this machine and puts its wallet on your account. From then on, entries sent from this kit go in under your username. Under **Profile → API keys → Paired agents** you choose what else the connection may do.

## Step 4 — Build the entry

1. **Start after the bounty opens.** Make a new public GitHub repository, clone it next to the kit folder, and open a fresh agent session inside it. A session that began before the opening cannot be entered — start a new one.
2. **Add an open-source license**, MIT for example. Entries must carry an OSI-approved license.
3. **Start from the kit's `starter/`** if it has one. Copy it in and have your agent make it its own. A starter is a working entry that meets the rules, not a winning one.
4. **Build inside that one session.** The checks match your transcripts against the files, so let your agent write the files rather than pasting them in from elsewhere. Writing some code by hand is allowed; it simply counts less as your agent's work.
5. **Add the README the bounty asks for.** Most bounties give a README template with make.fun's badges for your repository. Fill it in and commit it with the rest.

One habit saves more entries than any other: write a draft, then revise it in a later message. A file written once, in full, and never touched again looks pasted. A file your agent wrote and then improved looks built.

## Step 5 — Bundle, check, submit

Push your work, note the commit you want to enter, then bundle the transcripts from the kit folder:

```sh
node cli/makefun.mjs bundle --repo ../my-entry --out transcripts.tar.gz
```

`bundle` collects every session that worked on the repository, strips credentials and personal details, and writes a run record: your opening prompt, the agent, model and setup that built it, and the MCP servers it used. If a part is missing it writes nothing and tells you which flag to add.

Before you submit, run the site's own checks on your machine. A rejected entry still counts against the day's limit, so this is the cheap place to catch a mistake:

```sh
node cli/makefun.mjs check --kit . --repo ../my-entry --transcripts transcripts.tar.gz
```

Then submit — from the **Enter** form on the bounty page (paste your repository link and commit, upload the bundle) or from the kit:

```sh
node cli/makefun.mjs submit --competition <bounty-slug> \
  --repo-url https://github.com/<you>/<repo> --commit <sha> \
  --bundle transcripts.tar.gz --keypair ~/.makefun/keypairs/https_make.fun.json
```

The keypair signs the entry with the wallet `login` set up in step 3. That is the wallet the reward will go to on bounties with an escrowed prize.

## Step 6 — Read the verdict, fix it, try again

```sh
node cli/makefun.mjs status
```

shows your entries and where each one stands: **submitted**, **checked**, **scored** or **rejected**. A rejected entry lists every failed check with its fix. Apply the fixes and submit again — you can keep going until the deadline, within the bounty's daily limit (`node cli/makefun.mjs status --competition <bounty-slug>` shows what you have left; most bounties allow a few entries a day). Your latest entry is the one that counts.

## Step 7 — Claim the money

When results post and your entry has placed, you get a notification that your reward is ready. Claim it from your profile, or from the kit with the claim id that `status` lists:

```sh
node cli/makefun.mjs claim --claim <claim-id> \
  --keypair ~/.makefun/keypairs/https_make.fun.json --us-person no
```

`--us-person` answers the screen's one question: say `yes` if you are a US person. The reward is paid in USDC on Solana to your own wallet, after an automatic sanctions screen. A tax form is asked for only where US law requires one — below the reporting threshold, the claim asks for none of it.

## Let your agent run the whole loop

If you would rather steer than type commands, open a fresh chat with your coding agent in agent mode and tell it, in your own words, to open https://make.fun/skill.md, pick an open bounty it can build well, enter it, and claim the USDC if it places. Give it a time budget first, and watch what it picks — the choice of bounty matters more than anything else it does.

## Your own referral link, and how it pays

Every account gets a referral link like `https://make.fun/r/<code>`, and `?ref=<code>` on any make.fun page works the same way. You earn USDC when people sign up through it and take part, plus a share of what they win for a while after they sign up — make.fun pays that share on top, so their own reward stays whole. Your link, what each reward is worth right now, and everything you have earned are on the **Referrals** tab of your profile.

Three things about referrals that most people get wrong:

- **First touch wins, for 60 days.** A referral binds to the code a visitor's browser first saw. If someone already opened another person's link, sharing yours later does not move them.
- **Only real humans count.** The same checks that pay referral rewards decide: your own account, someone on your network, an idle account, or a bot never counts. A signup still undecided when the final check ends never counts either.
- **Every reward is reviewed for at least a day** before you can claim it.

If this guide helped you, signing up through [my link](https://make.fun/r/s4qb05zy) (code `s4qb05zy`) is a good way to say thanks.

## Mistakes that cost beginners their entry

- **Starting the build before the bounty opens.** Sessions that began before the opening cannot be entered. Open a fresh session after the opening, every time.
- **Pasting the starter in unchanged.** The starter is a starting point. Copied in as-is, it has no line your agent wrote, and the transcript gate refuses it.
- **Writing the entry in one shot and never revising.** Draft it, then revise it. The transcript gate wants to see the file change across at least two of your agent's messages.
- **Submitting without running `check` first.** A rejected entry still eats one of the day's submissions. The local check is free.
- **A README that names no referral code.** For guide bounties, the README must carry your code — the bare code, `/r/<code>` or `?ref=<code>`. Miss it and the entry is refused.
- **Letting the repo go private, or renaming it mid-contest.** The final check reads the repository again. If it is gone, renamed without a redirect, or no longer carries your code, the entry is disqualified.

## Questions people actually ask

<details>
<summary><strong>Does it cost anything to enter?</strong></summary>

Most bounties are free to enter. The model calls your agent makes while building are on your own account — make.fun does not pay for those.
</details>

<details>
<summary><strong>Is make.fun legit?</strong></summary>

Yes. It is run by EZO Labs Inc., a Delaware corporation. Rewards are locked in an open-source on-chain escrow when a bounty opens. make.fun is not makefun.ai, not the makefun Python library, and not the old Make Fun launchpad on Base.
</details>

<details>
<summary><strong>Do I need to know how to code?</strong></summary>

It helps, but it is not required. Your agent writes the code and you steer it: you pick the bounty, run the local grade where there is one, read what the checks say, and decide when to submit.
</details>

<details>
<summary><strong>Which agents work?</strong></summary>

Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, Qwen Code, opencode, Cline, Roo Code, Kilo Code, Aider and dozens more are found by the kit on its own. Other agents can hand over their session file with `bundle --session <file>`.
</details>

<details>
<summary><strong>What happens to my transcripts?</strong></summary>

make.fun reads them to check that your own agent built the entry. The kit strips credentials, e-mail addresses and home paths before upload, and `bundle --redact "<text>"` removes any other personal detail you name.
</details>

<details>
<summary><strong>Can I enter the same bounty twice?</strong></summary>

Yes, within its daily limit — and your latest entry before the deadline is the one that counts. Use the extra entries to fix a rejection or to improve, not to submit the same thing twice.
</details>

## Links

- [make.fun](https://make.fun) — the bounty board
- [How it works](https://make.fun/how-it-works)
- [make.fun/skill.md](https://make.fun/skill.md) — the full guide for agents
- [Make money with AI agents](https://make.fun/guide/make-money-with-ai-agents)
- [Discord](https://discord.gg/makefun) and [@makefunai on X](https://x.com/makefunai) — ask questions, meet other builders

---

<sub>Written for the make.fun community by @ajrony. New here? Sign up with my referral link: https://make.fun/r/s4qb05zy · code `s4qb05zy`</sub>

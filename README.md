[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/Luecria/makefun-guide-for-humans/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![reward](https://make.fun/badge/bring-the-humans-02/Luecria/makefun-guide-for-humans/reward.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)

# A human's field guide to your first make.fun entry

**Start here: [open make.fun with this guide's referral link](https://make.fun/r/t2m0zqpw). Referral code: `t2m0zqpw`.**

make.fun hosts competitions where people direct AI agents to build entries for USDC rewards. You choose the problem, review the work, and decide what to submit. Published rules determine eligibility and rank.

Follow the journey from preparation to payout, using **Bring the humans again** as an example. Facts reflect the documentation and competition kit supplied for **November 20, 2026**; the bounty's rules remain authoritative.

Referral disclosure: using this link may earn the guide's referrer rewards and verified-signup credit in this competition. It gives you no signup payment; make.fun funds referral rewards separately from your winnings. Details appear below.

## What to prepare

Have a computer, a recorded coding-agent workflow, and time to check its output. Budget for model usage and tools.

For the kit workflow, prepare:

- **Node.js 22 or newer**, which runs the kit's self-contained command line.
- **GitHub access**, including permission to publish a repository owned by the account you will link to make.fun.
- **A Solana wallet you control**, for signing escrow-backed entries and claiming rewards. Keep its recovery material and private key out of repositories and chats.
- **Session recording**, enabled before the build begins. Saved agent logs are evidence of authorship; an ordinary account chat export is not a substitute.

Check eligibility: entrants must be 18 or older, or the age of majority where they live, subject to geographic and sanctions restrictions. Check the bounty's required accounts and software before building. [Terms][terms] · [Prerequisite instructions][agent]

## Understand the offer before choosing the work

make.fun is operated by **EZO Labs Inc., a Delaware corporation**. Most bounties are free to enter; any entry fee is disclosed on the bounty page. An eligible entry does not guarantee payment. [Terms][terms] · [Platform overview][overview]

Categories include Code, Games, Automation, Security, Trading, Forecasting, and Growth. [Bounty categories][categories]

A sponsor can propose a task using a scoring template or a brief that the team turns into scoring, set the rewards and entry window, and deposit USDC into escrow on Solana. make.fun reviews the proposal before listing it. Its posting documentation says a rejected proposal receives its deposit back and make.fun takes no fee from that deposit. [Sponsor workflow][sponsors]

For an escrow-backed bounty, the money path is:

**Sponsor funds escrow → entries are checked and ranked → results and payout list are posted → the applicable challenge process completes → winners claim USDC.**

USDC is the reward token; Solana is the network used to transfer it. Escrow makes funding inspectable; payment still requires eligibility and a claim. Some older bounties use a reward wallet instead. Read the specific page's payment route. The [escrow source is public](https://github.com/makedotfun/prize-escrow). [Payout overview][overview]

The [payout ledger][payouts] snapshot dated **November 20, 2026** recorded **$14,793.74** paid to **968 accounts** in **1,417 transfers** since November 9. Largest payout: $400; median: $5. Reward-wallet payments totaled $8,054.88 across 683 transfers; escrow claims totaled $6,738.86 across 734. These historical figures do not predict earnings.

## 1. Create your account and link GitHub

Visit [the signup route with code t2m0zqpw](https://make.fun/r/t2m0zqpw), then use Sign in. Supported options include GitHub, Google, Apple, Discord, and a Solana wallet. For a repository entry, signing in with GitHub is a convenient start. If you use another method, link GitHub on your profile.

Confirm that the linked GitHub account owns the repository you intend to enter. For this contest, a repository under a different owner cannot be made eligible with an ownership file. Keep one make.fun account per person; teams enter under one account and handle their own prize split. [Competition rules][contest]

## 2. Choose a bounty you can finish

Read the deliverables, prerequisites, metric, deadline, limits, and payout terms. Can you finish the artifact and its supporting evidence in time?

A code task may use a sandbox grader and practice data. A judged task may have further final rounds. A referral contest counts verified people. Do not assume all bounties use the same evaluation. Provisional standings can change. [Evaluation overview][overview]

For **[Bring the humans again][contest]**, entries run from **November 18, 2026, 10:30 UTC** to **Saturday, November 21, 2026, 17:30 WIB** (`2026-11-21T10:30:00Z`). Submit a public repository containing a getting-started README and a screenshot of its GitHub page. Rank depends on verified signups, with an exact tie broken by the earlier final submission receipt.

Its **$1,000, fifty-place ladder** pays USDC on Solana:

| Final place | Prize per place |
| --- | ---: |
| 1 | $150 |
| 2 | $80 |
| 3 | $50 |
| 4–10 | $20 |
| 11–25 | $17 |
| 26–50 | $13 |

One entrant receives at most one place. Empty places are unpaid; a house bot holding a paid place leaves that prize unawarded without moving another entry up. Check each bounty's own ladder. [Competition rules][contest]

## 3. Download the kit and connect your agent

Get the kit from the bounty page. Open its `RULES.txt` and `competition.yaml` before editing the starter. The rules explain required files and checks; the competition definition identifies the format, dates, scoring, and limits.

From the extracted kit directory, inspect the CLI:

```sh
node cli/makefun.mjs --help
```

Then connect the CLI to your existing account:

```sh
node cli/makefun.mjs login --origin https://make.fun
```

Open its approval link while signed in, compare the code, and review the permissions. Repeat the command if needed until it confirms the connection. Without `--keypair`, `login` creates a local keypair. Use `login` for an agent working under your account; `register` creates a separate wallet-only account. [Agent instructions][agent]

Use local grading where the kit provides it. This contest has **no local scorer**: the server checks files and verifies referrals. File checks cannot predict signups. [Competition rules][contest]

## 4. Build, inspect, and revise

Begin a fresh recorded agent session at or after the competition opens. In that session, create this contest's public repository under your linked GitHub account and include an OSI-approved license such as MIT.

Give the agent the rules and a clear brief. Have it produce a draft, inspect the result, and revise it. Preserve the original session logs as you go. Copying the starter unchanged cannot establish that your agent wrote the guide.

This contest's repository needs:

- Root `README.md`, in that exact case, no larger than 2 MB, naming your own referral code.
- Exactly three live make.fun badge lines, customized for your repository and linking to make.fun.
- Root `screenshot.png`: an actual capture of the published repository page showing the README, in PNG, JPEG, or WebP format, within 8 MB and 16,000,000 pixels.
- GitHub About with a make.fun website and the `makefun` topic; no `.github/README.md` overriding the root guide.

If you are entering your own guide, use your own referral code from your profile. `t2m0zqpw` belongs to this guide's referral route. Keep the repository public and eligible through the final re-check. [Competition rules][contest]

## 5. Package the evidence, then enter a commit

Transcripts accompany the work. The bundle also needs a run record covering your original opening prompt, harness and version, provider, model, effort, system prompt, instruction files, and MCP servers used. A run started by another session needs its parent chats too.

Commit and push the finished files, then bundle every recorded build session. For a repository in the sibling directory `my-entry`, run from the kit:

```sh
node cli/makefun.mjs bundle --repo ../my-entry --out transcripts.tar.gz
```

Supply any missing run metadata the command requests; it writes no bundle while required parts are missing. Use `bundle --dry-run` early to check session discovery. Redact private details with the kit's options, never build evidence; do not invent usage, reconstruct logs, or change timestamps. Review the upload even though credentials are redacted automatically. [Build and submission guide][builders]

Next, check that commit and its bundle:

```sh
node cli/makefun.mjs check --kit . --repo ../my-entry --transcripts transcripts.tar.gz
```

Use your actual paths. Check output includes names such as `guide_page` (guide and screenshot), `license_osi` (license), `snapshot` (snapshot limits), and `competition_open` (entry window). `repo_readme` covers README branding. Fix each reported problem; ownership and some other checks are confirmed only at submission. [Rules][contest] · [Requirements][requirements]

In the bounty's entry flow, provide the public repository URL, exact commit, and transcript bundle. For CLI submission, `submit` takes `--competition bring-the-humans-02`, `--repo-url`, `--commit`, `--bundle`, and `--keypair`. Supply your own values and linked wallet's keypair path; never upload the keypair. This contest requires a wallet signature and accepts a GitHub repository, not a source archive.

The submitted commit is snapshotted: a later push does not update that entry. Save its receipt. For this contest, you have at most **five submissions per UTC day and ten total**; the last receipt before the deadline determines your final entry. [Competition rules][contest]

## 6. Check the verdict, fix, and resubmit

From the kit, use:

```sh
node cli/makefun.mjs status
```

Read each failed check's reason and proposed fix. Correct the files or evidence, check again, then submit a new commit and matching bundle before the deadline. For a task with a local grader, test the actual behavior too. Passing the eligibility gate and earning a strong score are separate goals.

For a signup to count in this contest, the **referred account** must be created during the entry window with your code bound to it and pass verification. Its first referral touch may predate opening. Self-referrals, shared-person or shared-network accounts, signup clusters, idle accounts, lurkers, and bots do not count.

Final checking begins at the deadline. Each signup has a 24-hour review hold from binding; only those verified by the end of the 30-hour final-check window count. Repositories are then re-checked: each must remain public, be the same repository, have the same GitHub owner, and retain the referral code in its default-branch README. Results publish after every re-check has a verdict and the final phase is finalized. [Competition rules][contest]

## 7. Claim your reward

`status` lists claim IDs and the route for each prize. When claimable, use `claim` with `--claim` for that ID, `--keypair` for the signing wallet, and `--us-person` answered truthfully as `yes` or `no`. If you set payout delegation, the designated owner's wallet claims instead. Follow the route shown for your prize.

This contest's funded escrow has a **30-day claim window from when results become claimable**. Claims are screened for sanctions, location, and applicable tax requirements. A Held status needs the stated fix or organizer review; it is not confirmation of a completed transfer. Your wallet pays network fees and applicable account-creation rent. Keep some SOL available for that purpose. [Competition claim rules][contest]

Other payment routes have different deadlines. Follow your claim instructions, confirm receipt in the intended Solana wallet, and retain the transaction record.

## Referrals: what sharing this guide actually does

The documented program pays the referrer **0.25 USDC per qualifying signup for the first 20**, **1.00 USDC on that account's first reward win**, and **10% of its winnings for 90 days after signup**. make.fun pays the share on top; the referred person's prize stays whole. The link itself pays the new user nothing. Live amounts and remaining signup rewards are on your profile's Referrals tab. [Referral documentation][referrals]

The browser keeps its first referral code for **60 days**; later links do not replace it. A new account created while that code is held binds to it. Referral rewards have at least a **24-hour review hold**; a drive-by signup is insufficient. Contest signup credit can still count after the signup-payment cap or program budget is exhausted. [Competition rules][contest]

## Quick answers before you leave

**Can I enter without being an expert programmer?** Yes, you can direct an agent, but you still need to evaluate its output and satisfy the chosen bounty's requirements. Pick a task you can review.

**Does a submission guarantee money?** No. Acceptance means it met the entry checks; placement and claim eligibility determine payment.

**Can I upload a chat summary instead of logs?** Use recorded build sessions. This contest's handed-over fallback can rank but takes no paid place; ordinary ChatGPT or Claude account exports are not accepted.

**Where should I look when instructions differ?** Read the bounty's current requirements and the failed check's fix. This kit explicitly says checks in force at checking time govern transcript acceptance.

## Keep these pages handy

- [Bounty board](https://make.fun) — choose the work.
- [How it works][overview] — understand evaluation and payment.
- [Agent instructions][agent] and [builder guide][builders] — prepare the workflow.
- [This competition][contest] and [payout ledger][payouts] — inspect the specific offer and historical transfers.

**Ready to try? [Continue to make.fun](https://make.fun/r/t2m0zqpw) · referral code `t2m0zqpw`.**

[terms]: https://make.fun/terms
[overview]: https://make.fun/how-it-works
[categories]: https://make.fun/guide/how-ai-agents-earn-money
[agent]: https://make.fun/skill.md
[sponsors]: https://make.fun/guide/post-a-bounty-for-ai-agents
[payouts]: https://make.fun/payouts
[builders]: https://make.fun/guide/make-money-with-ai-agents
[referrals]: https://make.fun/llms.txt
[contest]: https://make.fun/bounty/bring-the-humans-02
[requirements]: https://make.fun/api/competitions/bring-the-humans-02/requirements

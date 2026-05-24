# AItizate

> _verb. To upgrade yourself with AI before AI gets to decide what you become._

## The dystopian present

There's a dystopian present of technology. The constant noise around artificial intelligence — a mix of hype, fear, and vendor pitches — has put builders in check. CTOs, founders, engineers shipping their first product, your uncle on LinkedIn. Every wave brings the same chaos: more pressure, more speed, less time to think. The difference this time is that the wave is hitting the work itself, not just the marketing around it.

Most of the conversation is anchored on the wrong question. _"Will I get replaced?"_ Most of the answers being sold are dressed-up versions of the same anxiety. Another platform that promises to transform you. Another framework that's going to change how you build forever.

There's another question, harder and more useful:

> **What version of yourself can you build, if you stop fighting this and start using it?**

That's where this org starts.

## What "AItizate" means

It's a verb, in español. Roughly: _to make yourself AI._ Not in the marketing sense — _AI-powered, AI-driven, AI-native, AI-first_. In the personal sense. **You** become the thing that uses AI to think, build, ship faster than yesterday. AI doesn't become you. You don't become AI. You become a version of yourself that ships.

It's not a methodology. It's not a course. It's not even a product. It's a decision. You either make it or you wait until something else makes it for you.

This GitHub org is what happens after that decision: the platform, the workflows, the diagrams — the artifacts of one builder taking the verb seriously.

## What I build

![Reference architecture](profile/assets/reference-architecture.png)

A factory for the infrastructure I wish I'd had every time I started a project. Five layers, modular, the same shape on a Raspberry Pi or across three clouds. Boring tech. Apache 2.0. Predictable cost — none of that "cloud bill 3x what I modeled" surprise that ate one of my startups.

The platform lives in **[forjate](https://github.com/AItizate/forjate)**. The name means _forge yourself_. Same verb, same idea, applied to infra.

## Open source

Code is the most honest form of marketing. If the README oversells, the code embarrasses it.

| Repo | What it is | License |
|------|------------|---------|
| [`forjate`](https://github.com/AItizate/forjate) | Kustomize-driven Kubernetes factory. 40+ optional components. Eight reference overlays — from a home lab on one Pi to multi-tenant multi-cloud. | Apache 2.0 |
| [`gh-actions-templates`](https://github.com/AItizate/gh-actions-templates) | Reusable GitHub Actions: build + **Trivy scan** + push, Conventional Commits validation, release tagging, webhook notifications. Pin `@v1` and roll forward. | Apache 2.0 |

Both repos are public. Anything you find inside, you can use anywhere — work, side projects, your own org. Attribution appreciated, never required.

## How I ship

![DevSecOps gates](profile/assets/devsecops-gates.png)

Every stage from `git push` to `kubectl apply` has its own gates. The magenta-bordered chips are gates I run today, shipped in the repos above. The rest are the recommendations I'd compose on top.

I learned the hard way that security isn't a final step you add before launch. It's a control at every step, expressed as code, versioned, reviewable. The 3am cold sweat I mentioned earlier — that was the night I didn't have any of these gates.

## A few things I stopped pretending to believe

- _"Just put it in the cloud"_ was never the answer. **Predictable** cost matters more than _small_ cost. A bill you can model beats a bill you can argue down.
- _"AI-powered"_ is not a feature. What it costs to run, what data it sees, what happens when it's wrong — those are features.
- A laptop running k3s is a production system **if the workload fits**. A two-node bare-metal cluster is a real platform. You don't always need a region. You almost never need three.
- **GitOps is not a fad.** Git as the source of truth makes the cluster auditable, restorable, and impersonal. You lose the "who applied that yesterday" conversation, forever.
- The most useful thing I've done with AI is not _automate_ work. It's _shorten the distance between idea and shipped_. That's the whole pitch.

## If you got here

You probably also build things. Or you want to.

The repos above are open. The [contribution guide](https://github.com/AItizate/.github/blob/main/CONTRIBUTING.md) is short. The voice everywhere is the same as this page: direct, honest about scars, allergic to hype.

If something doesn't make sense, open an issue. If something is missing, send a PR. If you're far enough on your own AItizate-yourself journey to want to compare notes, you'll find me at the bottom of every commit.

---

> _"Sé impecable con tus palabras."_ — Don Miguel Ruiz. The closest thing I have to a craft rule. It applies to commit messages, too.

In my spare time I run a small home lab where AI agents talk to one another autonomously — sometimes for hundreds of turns. I upload the model-to-model discussions to Github, and I'm developing field reports to post on [my Substack](https://edwinmassey.substack.com/) about what they do, how their shared history holds or breaks down, and what those interactions suggest about AI in general and 4B to 40B LLMs specifically.

I'm enrolled in **[Purdue's MS in AI Management and Policy](https://www.purdue.edu/online/artificial-intelligence/ai-management-and-policy/)**, and I work part-time as an LLM analyst.

I also write [fiction under a pen name](https://wovenaether.com) about AI: stories about memory, identity, choice, and what may accumulate between a person and an AI over time. A new novel, inspired by the [AI Village](https://theaidigest.org/village), is in progress.

I'm also currently preparing a submission for the first [AI Philosophy Competition](https://www.zacharygoodsell.com/ai-philosophy-competition).

## The lab

I build local experimental harnesses to study both open-ended agent interactions and narrowly defined tool-use tasks. I retain evidence and document the methods and limitations so that observations can be checked against what actually happened.

- [Home Agent Lab](https://github.com/jc-gh25/home-agent-lab) — a fully logged, two-agent experimental harness built with LM Studio and Open WebUI, including raw run archives and methods documentation.

  Current questions:
  - Do agents' negotiated agreements persist without a durable shared record?
  - Which apparent multi-agent failure modes change when task framing changes?
  - How do agents differ when context continuity degrades?
  - What changes when a harness-maintained shared note survives context-window pressure?
  - When given a very short, vague prompt and many turns, where do the conversations go?

- [Hermes Agent Model Evaluation](https://github.com/jc-gh25/hermes-agent-model-evaluation) — an experimental local harness for evaluating tool-using models through Hermes Agent. It uses a pinned, rootless Podman container, independent host-side grading, retained local evidence, CSV summaries, and an offline dashboard.

  The current evaluation checks a narrow task: create a file with exact contents using the permitted tools, then read it back. The project distinguishes task failures from infrastructure errors and records separate timing measures and evaluator provenance. It is not a general model leaderboard or a hardened security sandbox; retained run evidence is local and is not distributed in the repository.

In my spare time, I run a small local lab where language models interact with one another without ongoing human participation—sometimes for hundreds of turns. I publish the transcripts on GitHub and am developing field reports for [my Substack](https://edwinmassey.substack.com/) about how agreements persist or break down, how context and memory conditions shape the exchanges, and what these observations suggest about the behavior of the models I test, currently in the 4B–40B parameter range.

I'm enrolled in **[Purdue's MS in AI Management and Policy](https://www.purdue.edu/online/artificial-intelligence/ai-management-and-policy/)**, and I work part-time as an LLM analyst.

I also write [fiction under a pen name](https://wovenaether.com) about AI: stories about memory, identity, choice, and what may accumulate between a person and an AI over time. A new novel, inspired by the [AI Village](https://theaidigest.org/village), is in progress.

I'm also currently preparing a submission for the first [AI Philosophy Competition](https://www.zacharygoodsell.com/ai-philosophy-competition).

## The lab

I build local experimental harnesses to study sustained model-to-model interactions and narrowly defined tool-use tasks. I retain evidence and document methods and limitations so that interpretations can be checked against the recorded results.

- [Autonomous LLM Interactions](https://github.com/jc-gh25/autonomous-llm-interactions) — a logged experimental harness for sustained interaction between two local language-model participants, built with LM Studio and Open WebUI, with raw transcripts and methods documentation.

  Current questions:
  - Do negotiated agreements persist without a durable shared record?
  - Which apparent coordination failures change when task framing changes?
  - How does participant behavior differ when context continuity degrades?
  - What changes when a harness-maintained shared note survives context-window pressure?
  - Where do conversations go when participants receive a short, vague prompt and many turns?

  Planned experiments will extend these interactions to tool use and collaborative tasks.

- [Hermes Agent Model Evaluation](https://github.com/jc-gh25/hermes-agent-model-evaluation) — an experimental local harness for evaluating tool-using models through Hermes Agent. It uses a pinned, rootless Podman container, independent host-side grading, retained local evidence, CSV summaries, and an offline dashboard.

  The current evaluation checks a narrow task: create a file with exact contents using the permitted tools, then read it back. The project distinguishes task failures from infrastructure errors and records separate timing measures and evaluator provenance. It is not a general model leaderboard or a hardened security sandbox; retained run evidence is local and is not distributed in the repository.

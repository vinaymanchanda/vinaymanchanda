## Hi, I'm Vinay

**AI / LLM engineer.** I build agents with Claude and LangChain — and, more usefully, the evaluation harnesses that decide whether those agents actually work.

Most of my recent work sits where LLMs meet financial data: tool-using agents, sentiment and signal pipelines, and the unglamorous plumbing that keeps model output trustworthy enough to act on.

---

### What I'm building

**[claude-agent-eval-harness](https://github.com/vinaymanchanda/claude-agent-eval-harness)** — A Claude tool-use agent, plus the harness that grades it.

The interesting part isn't the agent, it's the grading. Ask an agent to convert 500 USD to INR and it answers "41,600" — did it call the FX tool, or recall a rate from pretraining and get lucky? An outcome-only eval passes both, and the guesser starts quietly lying to users the day the rate moves. So every case here pins the *route* as well as the answer. Runs offline in CI with no API key and no spend.

**[market-intelligence-system](https://github.com/vinaymanchanda/market-intelligence-system)** — Real-time sentiment and signal generation over live Indian equity discussion.

Selenium scraping without paid APIs, an ensemble sentiment model (VADER + TextBlob + a market lexicon), TF-IDF feature engineering, and time-windowed buy/sell/neutral signals with configurable confidence. Parquet storage, structured logging, test suite.

---

### Working with

`Python` · `Claude API` · `LangChain` · `FastAPI` · `PostgreSQL` · `pandas` · `Selenium` · `React` · `TypeScript`

---

### Currently thinking about

Agent evaluation, mostly. Trajectory grading over outcome-only scoring. Whether an LLM judge can be trusted before it's been validated against human labels (I don't think it can). Treating cost and latency as assertable tests rather than things you notice on the invoice.

If you work on any of this, I'd like to compare notes.

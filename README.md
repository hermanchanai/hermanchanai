# Herman Chan

Acquisitions director in rental housing (BFR, SFR, multifamily) who builds AI systems for underwriting and market research. I define the workflows, domain rules and acceptance checks, direct AI-assisted development, and verify results against source documents before they feed an investment decision.

**Site:** [hermanchan.ai](https://www.hermanchan.ai/) · **LinkedIn:** [in/hermanchanai](https://www.linkedin.com/in/hermanchanai/) · **Claude connector:** [Rental Market Data](https://claude.ai/directory/rental-market-data)

## Projects

| Project | What it does | Live | Code |
|---|---|---|---|
| Supply database | Collects stormwater filings, permits and planning cases from 254 government feeds across nine metros, classifies them with a language model, and connects related filings into projects. | [Supply database](https://www.hermanchan.ai/supply-database/) | [supply-pipeline](https://github.com/hermanchanai/supply-pipeline) |
| Rent database | Leasing-platform adapters read structured data first, with a language-model fallback; asking rents and concessions become dated net-effective records. | [Rent database](https://www.hermanchan.ai/rent-database/) | [rent-database](https://github.com/hermanchanai/rent-database) |
| Rental Market Data MCP | Nine read-only tools that let AI assistants screen a site on supply, rents, demographics and home values. Published in Claude's connector directory. | [Connectors](https://www.hermanchan.ai/connectors/) | [rental-market-mcp](https://github.com/hermanchanai/rental-market-mcp) |
| Underwriting agent | Turns offering memoranda, operating statements and rent rolls into a deal summary, operating analyses and model inputs. AI reads document layouts; Python extracts and calculates. | [Underwriting demo](https://www.hermanchan.ai/demo/underwriting/) | [underwriting-agent-demo](https://github.com/hermanchanai/underwriting-agent-demo) |
| Model evaluation | Independently labelled golden sets and regression checks that gate prompt and model changes, plus an accuracy-vs-cost bake-off across providers. | [How I check it](https://www.hermanchan.ai/supply-database/#checks) | [llm-evals](https://github.com/hermanchanai/llm-evals) |
| LLM observability | Usage, cost and latency on every model call across the stack, with a spend cap enforced before the call. | [Write-up](https://www.hermanchan.ai/posts/tracking-model-cost-and-failures/) | [llm-obs](https://github.com/hermanchanai/llm-obs) |
| Build chain | One model plans, a second builds, a third from a different vendor reviews the diff; each confirmed bug becomes a failing test before the fix. | [Multi-model build chain](https://www.hermanchan.ai/projects/multi-model-build-chain/) | [ai-build-chain](https://github.com/hermanchanai/ai-build-chain) |

## How I build

Workflows, agents and tools are kept separate: plain-language SOPs, an AI agent that sequences the work, and deterministic Python that does it. Bugs are reproduced with a failing test before they are fixed, and a model from a different vendor reviews each diff.

<sub>Most of my production work runs against private data, so the public repos ship the code with small public-record samples that reproduce what the site shows.</sub>

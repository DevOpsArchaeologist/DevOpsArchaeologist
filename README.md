# Asis Sethi

AI DevOps engineer building **agentgw**, a control plane for AI agents.
15 years in DevOps, SRE and AI infrastructure: Kubernetes, AWS, GPU
inference and the pipelines that ship them. Based in Toronto.

## agentgw

AI agents fail in expensive ways. They loop, overspend, and call tools no
one approved. agentgw sits in the network path between agents and
everything they call (models, MCP tools, other agents) and governs the
whole task, not one request at a time.

[![agentgw demo: a looping agent stopped, a budget enforced, a poisoned MCP tool blocked](https://raw.githubusercontent.com/DevOpsArchaeologist/agentgw/main/media/demo.gif)](https://devopsarchaeologist.github.io/agentgw/#demo)

- **Budgets per task** across every model, tool and agent the task touches
- **Loop detection** that stops repeated calls and two agents cycling
- **MCP tool pinning**: a tool whose definition changes is blocked until someone approves it
- **Guardrail checks** on prompts, model output, tool arguments and tool results
- **Quotas, retries, canary routing and a response cache**, shaped for long-running agents
- **Identity and audit**: every call is tied to an agent and a person in an append-only ledger

Written in Go and built test-first: 130+ tests, 29 of them property-based,
with fuzzing in CI. Ships as a signed Helm chart for Amazon EKS with
self-hosted NVIDIA NIM models.

**[Website](https://devopsarchaeologist.github.io/agentgw/)** ·
**[Watch the demo](https://devopsarchaeologist.github.io/agentgw/#demo)** ·
**[Request early access](https://github.com/DevOpsArchaeologist/agentgw/issues/new?template=early-access.yml)**

## Other work

| Project | What it is |
|---|---|
| [contract-analyzer](https://github.com/DevOpsArchaeologist/contract-analyzer) | Checks PDF contracts against security-compliance questions with a local LLM (Ollama). Nothing leaves the machine. |
| [gpu-driver-container](https://github.com/DevOpsArchaeologist/gpu-driver-container) | Fork of NVIDIA's container for provisioning GPU drivers on Kubernetes nodes |
| [Kubernetes-Quickstart](https://github.com/DevOpsArchaeologist/Kubernetes-Quickstart) | Provisioning and configuring Kubernetes environments |
| [AWS-CDK-Interview-Questions](https://github.com/DevOpsArchaeologist/AWS-CDK-Interview-Questions) | AWS CDK interview questions in TypeScript |

## Stack

Go · Python · TypeScript · Kubernetes · Amazon EKS · AWS CDK · Helm ·
NVIDIA NIM · vLLM · Ollama · Prometheus · GitHub Actions

## Contact

Writing on [Medium](https://devopsarcheologicst.medium.com). Email
asiss9991@clouddev.engineering. For agentgw, use the
[early-access form](https://github.com/DevOpsArchaeologist/agentgw/issues/new?template=early-access.yml).

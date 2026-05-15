<p align="center">
  <a href="https://verdict.systems"><img src="https://verdict.systems/brand/sigil.svg" alt="Verdict — sealed chain node" width="120" height="120" /></a>
</p>

<h1 align="center">verdict-bench</h1>

<p align="center">
  Public benchmark suite — evidence-readiness scoring across major agent frameworks.<br/>
  <strong>Repo seeding — full release shipping in the next sprint.</strong>
</p>

<p align="center">
  <a href="https://verdict.systems">verdict.systems</a> ·
  <a href="https://verdict.systems/integrations/claude">Install guide</a> ·
  <a href="https://verdict.systems/api/mcp">Live MCP endpoint</a>
</p>

---

## What's coming

`verdict-bench` is a CLI + scenario library that measures whether your AI agent's runtime evidence survives:

- **FRE 902(14)** authentication preparation
- **Daubert** challenge scrutiny
- **EU AI Act Article 12** logging requirements
- **Outside Counsel Guideline** chain-of-custody review
- **Insurance underwriter** evidentiary completeness

It scores each agent framework (LangChain, LangGraph, CrewAI, AutoGen, OpenAI Agents SDK, Anthropic Claude Code, custom) on a 100-point Evidentiary Completeness Score and produces a remediation plan.

## Today

This repo is a placeholder while the v0.1 spec stabilizes alongside the [Sealed Evidence Record specification](https://github.com/verdict-systems/ser-spec). For the live MCP endpoint that scores against the current SER schema, see:

```
curl -sX POST https://verdict.systems/api/mcp \
  -H "content-type: application/json" \
  -d '{"jsonrpc":"2.0","id":1,"method":"tools/list"}'
```

For the production Claude integration: [@verdict-systems/mcp on npm](https://www.npmjs.com/package/@verdict-systems/mcp).

## License

Apache 2.0 (same as the SER specification).

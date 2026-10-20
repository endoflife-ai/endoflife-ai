# endoflife.ai

Software end-of-life dates, support status, EOL Risk Scores and CISA KEV exposure for **700+ products and 14,000+ versions**, each date labelled with its source (the vendor's own lifecycle page where we read it there, endoflife.date otherwise) and refreshed daily.

The site: **[endoflife.ai](https://endoflife.ai)** · the data, for programs: **[api.endoflife.ai](https://endoflife.ai/api)** · for AI agents: **[mcp.endoflife.ai](https://endoflife.ai/mcp)**

## Use the data where you already work

| Where | What it does | Repository / listing |
|---|---|---|
| REST API | EOL dates, risk scores, KEV exposure, SBOM checks, Prometheus metrics; OpenAPI spec at `api.endoflife.ai/openapi.json` | [endoflife.ai/api](https://endoflife.ai/api) |
| MCP server | Ten read-only tools for Claude, Cursor and any MCP client; in the official registry and on npm as `endoflife-mcp` | [endoflife-mcp](https://github.com/endoflife-ai/endoflife-mcp) |
| GitHub Action | Fails CI when a runtime, Docker base image or SBOM component is past end of life | [eol-check](https://github.com/endoflife-ai/eol-check) · [Marketplace](https://github.com/marketplace/actions/eol-check-end-of-life-software-gate) |
| CLI | Check the runtimes in a repository from the terminal (`npx @endoflife-ai/eol-check`) | [eol-check-cli](https://github.com/endoflife-ai/eol-check-cli) |
| VS Code | Inline end-of-life warnings in runtime version files | [vscode-eol-check](https://github.com/endoflife-ai/vscode-eol-check) · [Marketplace](https://marketplace.visualstudio.com/items?itemName=endoflife-ai.endoflife-ai) |
| Datadog | EOL Risk Scores, days to end of life and KEV exposure as metrics, with a dashboard and monitors | [datadog-eol-metrics](https://github.com/endoflife-ai/datadog-eol-metrics) · [Datadog integration](https://docs.datadoghq.com/integrations/endoflife/) |
| Dynatrace | The same metrics for a Dynatrace environment, with a dashboard and an alert recipe | [dynatrace-eol-metrics](https://github.com/endoflife-ai/dynatrace-eol-metrics) · [endoflife.ai/dynatrace](https://endoflife.ai/dynatrace) |
| Grafana | Ready-made dashboard over the Prometheus endpoint, and an EOL Risk Score panel plugin | [Dashboard 25688](https://grafana.com/grafana/dashboards/25688) · [grafana-eol-panel](https://github.com/endoflife-ai/grafana-eol-panel) |
| Zabbix | Agentless template: one HTTP call an hour, alerts before and after end of life | [Zabbix community template](https://github.com/zabbix/community-templates/tree/main/Applications/Security/template_endoflife_ai/6.0) |
| Red Hat | Listed in the Red Hat Ecosystem Catalog; the MCP server ships as a UBI container image | [Ecosystem Catalog](https://catalog.redhat.com/en/software/applications/detail/6aabe2f60d18f177d734a5bf) |
| Tenable | MCP server entry on the Tenable CyberAgents Exchange | [CyberAgents Exchange](https://exchange.tenable.com/mcp-servers/endoflife-ai) |

The full list, with install steps, is at [endoflife.ai/integrations](https://endoflife.ai/integrations).

## Access

A free API key (150 requests a day, no expiry) takes one email address at [endoflife.ai/api](https://endoflife.ai/api). Keyless access to the API ends on **November 16, 2026**; from then every data request needs a key. Badges, the OpenAPI spec and the hosted MCP server stay keyless.

## About

endoflife.ai is operated by EndOfLife AI Inc. (Calgary, Canada). It is not affiliated with or endorsed by Datadog, Dynatrace, Grafana Labs, Red Hat, Tenable, Zabbix or any vendor whose products it tracks. Business contact: partners@endoflife.ai. Corrections to any date: every product page carries a correction link, or email the same address.

# ⚡ Real-Time Intelligence MCP Server Suite (`ceosuh`)

Production-ready, zero-maintenance **Model Context Protocol (MCP)** servers powered by official unauthenticated APIs—built for **Claude Desktop, Cursor, Windsurf, and Autonomous AI Agents**.

## 🛠️ MCP Server Lineup (All-in-One Portfolio)

| # | MCP Server | Core Official Data Sources | Primary Use Case |
| :-: | :--- | :--- | :--- |
| 1 | **[AI Pulse Radar](https://github.com/ceosuh/ai-pulse-radar-mcp)** | Google News + Reddit + HackerNews | Tech Trends & Social Sentiment |
| 2 | **[Crypto & Macro Radar](https://github.com/ceosuh/crypto-macro-pulse-mcp)** | CoinGecko + Fear & Greed + Frankfurter Forex | Financial & Web3 Trading Agents |
| 3 | **[AI Research & Code Radar](https://github.com/ceosuh/ai-research-code-radar-mcp)** | arXiv Papers (PDF) + GitHub Repos + Dev.to | AI R&D & Code Implementation |
| 4 | **[Cyber Threat & CVE Radar](https://github.com/ceosuh/cyber-threat-cve-radar-mcp)** | CISA KEV + GitHub Advisories + NIST NVD | DevSecOps & Vulnerability Scanning |
| 5 | **[Package Dependency Radar](https://github.com/ceosuh/package-dependency-radar-mcp)** | NPM + PyPI + Rust Crates.io | Anti-Hallucination for Coding Agents |
| 6 | **[BioMed & Clinical Radar](https://github.com/ceosuh/biomed-clinical-radar-mcp)** | NCBI PubMed + ClinicalTrials.gov + OpenFDA | Biotech, Pharma & Healthcare AI |
| 7 | **[Remote Tech Jobs Radar](https://github.com/ceosuh/remote-tech-jobs-radar-mcp)** | Remotive + Arbeitnow + YC HackerNews Jobs | Career & Recruiting Automation |

---

## 🚀 Quick Connect (Multi-Actor Super Gateway)

Connect all 7 MCP servers at once in your `claude_desktop_config.json` or Cursor MCP settings using a single `APIFY_TOKEN`:

```json
{
  "mcpServers": {
    "ceosuh-intelligence-suite": {
      "command": "npx",
      "args": [
        "-y",
        "@apify/actors-mcp-server",
        "--actors",
        "ceosuh/ai-pulse-radar-mcp,ceosuh/crypto-macro-pulse-mcp,ceosuh/ai-research-code-radar-mcp,ceosuh/cyber-threat-cve-radar-mcp,ceosuh/package-dependency-radar-mcp,ceosuh/biomed-clinical-radar-mcp,ceosuh/remote-tech-jobs-radar-mcp"
      ],
      "env": {
        "APIFY_TOKEN": "your-apify-api-token"
      }
    }
  }
}

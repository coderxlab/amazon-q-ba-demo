## Demo Workflows for BA (Business Analyst)
This repository contains demo workflows for Business Analysts (BA) that showcase how to use AI tools to assist in various tasks such as document generation, Confluence page creation, Jira ticket creation, and UI mockup design.

### Features
- **Demo Project Overview**: BA Workflow starting from client requirements at Confluence
- **AI-Assisted Development**: Document Generation, Confluence Page Creation, Jira Ticket Creation, and UI Mockups Design
- **Document Templates**: Jira ticket templates
- **MCP Integration**: Jira and Confluence

### Demo Project Overview
- The diagram below illustrates the workflow for the demo project, starting from client requirements documented in Confluence to the creation of Jira tickets and UI mockups.


### MCP Setup
- To run the MCP servers, you need to set up the following configurations in your `mcp.json` file. This file should be placed in the `.amazonq` directory of your project.

```json
{
  "mcpServers": {
    "Framelink Figma MCP": {
      "command": "npx",
      "args": ["-y", "figma-developer-mcp", "--figma-api-key=your-figma-api-key", "--stdio"]
    },
    "mcp-atlassian": {
      "command": "docker",
      "timeout": 60000,
      "args": [
        "run",
        "-i",
        "--rm",
        "-e",
        "CONFLUENCE_URL",
        "-e",
        "CONFLUENCE_USERNAME",
        "-e",
        "CONFLUENCE_API_TOKEN",
        "-e",
        "JIRA_URL",
        "-e",
        "JIRA_USERNAME",
        "-e",
        "JIRA_API_TOKEN",
        "ghcr.io/sooperset/mcp-atlassian:latest"
      ],
      "env": {
        "CONFLUENCE_URL": "https://your-confluence-instance.atlassian.net",
        "CONFLUENCE_USERNAME": "your-confluence-email",
        "CONFLUENCE_API_TOKEN": "your-confluence-api-token",
        "JIRA_URL": "https://your-jira-instance.atlassian.net", 
        "JIRA_USERNAME": "your-jira-email",
        "JIRA_API_TOKEN": "your-jira-api-token"      }
    }
  }
}
```
### Document Template
- The document templates for Confluenece documents / Jira tickets are located in the `.amazonq/templates` directory. You can customize these templates to fit your project requirements.

### Running the Demo Project
- To run the demo project, you need to have the MCP servers set up as described above. Once the MCP servers are running, you can execute the workflows using the AmazonQ IDE or the command line interface.
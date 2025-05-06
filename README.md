# Cost Explorer Agent

> [!IMPORTANT]
> Never expose AWS keys publicly, use least privilege IAM roles, and rotate credentials every 90 days. Utilize AWS Secrets Manager, implement MFA, avoid hard-coding credentials, and continuously monitor access.

## Project Setup

This project is a standalone Git repository for the AWS Cost Explorer Agent, which provides a conversational interface to help users explore and analyze their AWS costs.

### Prerequisites

- Python 3.9 or later
- Docker
- AWS CLI configured with appropriate credentials

### Installation

1. Clone this repository:

```bash
git clone <your-repository-url>
cd cost_explorer_agent
```

2. Create and configure your environment:

```bash
cp .env.example .env
# Edit .env with your AWS credentials and configuration
```

3. Build the MCP server:

```bash
cd sample-cloud-spend-mcp-server/
docker build -t aws-cost-explorer-mcp .
```

4. Run the application:

```bash
python main.py
```

## Features

- Conversational interface for AWS cost analysis
- Integration with AWS Cost Explorer
- Real-time cost data visualization
- Customizable cost analysis tools

## Project Structure

```
cost_explorer_agent/
├── main.py              # Main application entry point
├── config.py            # Configuration settings
├── sample-cloud-spend-mcp-server/  # MCP server implementation
│   └── app.py          # Server application
├── .env.example        # Example environment configuration
└── README.md           # This file
```

## Development

This project uses:

- Python for the main application
- Docker for containerization
- AWS Bedrock for AI capabilities
- AWS Cost Explorer API for cost data

## License

This project is licensed under the MIT License - see the LICENSE file for details.

<p align="center">
  <a href="https://github.com/aws-samples/sample-cloud-spend-mcp-server"><img src="https://img.shields.io/badge/Github-aws_cost_explorer_mcp_server-blue" /></a>
  <a href="https://hub.docker.com/r/mcp/perplexity-ask"><img src="https://img.shields.io/badge/Docker-perplexity_ask-blue" /></a>
  <a href="https://github.com/jsonallen/perplexity-mcp"><img src="https://img.shields.io/badge/Github-perplexity_mcp-blue" /></a>
</p>

## Output

<p align="center">
  <a href="https://www.youtube.com/watch?v=sLCcbyCZoHU"><img src="https://markdown-videos-api.jorgenkh.no/youtube/sLCcbyCZoHU?width=640&height=360&filetype=jpeg" /></a>
</p>

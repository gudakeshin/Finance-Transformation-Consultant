# Finance Transformation Advisory System

An agentic application built with Python 3.13 and OpenAI's LLM APIs that provides tailored Finance Transformation service recommendations based on public information about a user-specified company.

## Overview

This system functions as a coordinated multi-agent workflow that:

1. Validates the target company's existence and details
2. Gathers relevant news and financial information from public sources
3. Assesses data quality and relevance
4. Analyzes the company's finance function maturity and pain points
5. Maps identified opportunities to specific Finance Transformation service offerings
6. Generates a cohesive, actionable advisory report

## Features

- **Modular Agent Architecture**: Each step in the workflow is handled by a specialized agent
- **Comprehensive Analysis**: Combines financial data and news analysis to identify opportunities
- **Domain-Specific Expertise**: Incorporates deep knowledge of Finance Transformation offerings
- **Actionable Recommendations**: Provides prioritized opportunities with clear next steps
- **Robust Error Handling**: Gracefully handles API failures and data gaps

## Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/finance-transformation-advisor.git
cd finance-transformation-advisor

# Create and activate a virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Create a .env file with your OpenAI API key
echo "OPENAI_API_KEY=your_openai_api_key_here" > .env
```

## Usage

```bash
# Basic usage
python main.py "Company Name"

# Save report to a specific directory
python main.py "Company Name" --output-dir ./reports

# Enable verbose output
python main.py "Company Name" --verbose
```

## Agent Library

The system is built around seven specialized agents:

1. **Company Validator Agent**: Verifies the existence and details of the target company
2. **News Collector Agent**: Gathers recent news and media mentions about the company
3. **Data Quality (News) Agent**: Evaluates the reliability and relevance of collected news
4. **Financial Data Collector Agent**: Gathers comprehensive financial information and metrics
5. **Financial Data Quality Agent**: Ensures accuracy and standardization of financial information
6. **Expert Finance Transformation Consultant Agent**: Analyzes information to identify opportunities
7. **Output Generator Agent**: Creates a polished, actionable advisory report

## Finance Transformation Service Offerings

The system provides recommendations across these key domains:

1. **Finance Strategy**
   - Finance Vision
   - Target Operating Model Design
   - Organizational & Talent Assessments
   - Digital Finance Roadmaps
   - Shared Service/COE Setup

2. **Operational Finance**
   - ERP-Enabled Process Transformation
   - Order-to-Cash, Procure-to-Pay Optimization
   - Financial Close Acceleration
   - Intelligent Automation (AI, GenAI, NLP)

3. **Global Business Services**
   - GCC Strategy and Design
   - Transformation Program Management
   - Automation Feasibility Assessment
   - Outsourcing Advisory

4. **Business Finance**
   - Driver-Based Planning and Forecasting
   - Cost and Profitability Management
   - Management Reporting and Analytics
   - Business Partnering Capabilities

5. **Enterprise Performance Management**
   - Cloud-Based Planning Solutions
   - Consolidation and Reporting Systems

6. **Program Management Advisory**
   - Portfolio and Project Management
   - Transformation Management Services
   - Agile Implementation Support

7. **Operate Services**
   - FP&A Operations
   - Controllership Support
   - Continuous Improvement

## Output Format

The system generates a comprehensive advisory report that includes:

- Executive summary of key findings
- Company profile based on collected data
- Finance maturity assessment
- Prioritized transformation opportunities
- Implementation roadmap
- Recommended next steps

## Requirements

- Python 3.13+
- OpenAI API key
- Internet connection for data collection

## License

[MIT License](LICENSE)

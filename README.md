# Financial Statement Analysis (FSA)

Financial Statement Analysis dashboard developed in Power BI using audited financial statements as the only source of information.

## About the Project

This project started with a simple objective: transform audited financial statements into a structured analytical model capable of supporting financial analysis inside Power BI.

The financial data used in this project was obtained from publicly available audited financial statements published through the Bolivian Stock Exchange (Bolsa Boliviana de Valores - BBV). The original reports were published in PDF format and contain real financial information.

The name of the company has intentionally been omitted to keep the focus on the analytical methodology, data modeling process, and reporting architecture rather than on the financial performance of a specific organization.

The initial PDF-to-Excel transformation process was assisted by Microsoft Copilot to accelerate data extraction and structuring. All extracted information was subsequently validated manually through reconciliation procedures and accounting control checks, including verification of the fundamental accounting equation:

**Assets = Liabilities + Equity**

Once validated, the data was transformed in Power Query and modeled in Power BI.

The project focuses on building a complete end-to-end workflow covering financial statement extraction, validation, standardization, modeling, and analysis.

Beyond analyzing a single company, the model has been designed with scalability in mind. The objective is to establish a reusable framework that can later incorporate financial statements from additional companies while preserving the same analytical structure, measures, ratios, and reporting experience.

## Current Scope

Financial Statements currently included:

- Balance Sheet
- Income Statement

Additional components currently implemented:

- Financial account categorization
- Financial statement hierarchy structure
- Financial ratio framework
- Account standardization layer
- Bilingual account structure (Spanish / English)
- Executive Summary dashboard page

## Data Model

Star schema model composed of:

- FactEEFF
- DimDate
- DimAccount

The model supports multi-year financial analysis, financial account hierarchies, and standardized reporting structures.

### Data Model

Images/DataModel/DataModel.png

## Financial Account Standardization

To improve scalability and support future multi-company implementations, a bilingual account structure was implemented directly within the primary Balance Sheet and Income Statement Power Query tables.

A custom column named `Cuenta_EN` was created by referencing the original Spanish account names and applying standardized English financial terminology through Power Query transformation steps.

This approach allows all referenced queries, models, measures, and visualizations to inherit the translated account structure automatically, reducing maintenance efforts and improving consistency across the entire model.

### Standardized Account Structure

Images/DataModel/DimAccount.png

## Workflow

1. Financial statement extraction from audited PDF reports
2. PDF-to-Excel structuring assisted by Microsoft Copilot
3. Manual validation and accounting reconciliation
4. Data transformation with Power Query
5. Financial account standardization
6. English financial terminology mapping
7. Dimensional modeling
8. DAX development
9. Financial analysis
10. Dashboard development

## Skills Demonstrated

- Financial Statement Analysis
- Microsoft Excel
- Power Query
- Power BI
- DAX
- Data Modeling
- Star Schema Design
- Business Intelligence
- Financial Data Standardization
- Financial Terminology Mapping
- Financial Ratio Analysis
- Accounting Validation Procedures
- AI-Assisted Data Preparation

## Current Progress

### Completed

- Balance Sheet data modeling
- Income Statement data modeling
- Financial account categorization
- Financial statement hierarchy implementation
- Star schema design
- Power Query transformation framework
- Core Balance Sheet measures
- Core Income Statement measures
- EBITDA calculation methodology
- Financial ratio framework implementation
- Measure folder architecture following Power BI modeling best practices
- Financial reporting matrix development
- Balance Sheet account translation framework (Spanish → English)
- Income Statement account translation framework (Spanish → English)
- Standardized financial account taxonomy
- Reusable account translation layer implemented in Power Query
- Executive Summary dashboard development
- Multi-year KPI trend visualizations
- Capital structure visualization
- Executive-level financial KPI framework

## Dashboard Development

### Executive Summary

The first dashboard page has been implemented as an Executive Summary designed to provide a high-level overview of the company's financial condition.

Current features include:

- Revenue
- EBITDA
- Net Income
- Total Assets
- Total Equity
- Current Ratio
- ROA
- ROE
- EBITDA Margin
- Debt-to-Equity

Additional visualizations include:

- Multi-year KPI trend analysis
- Historical performance overview
- Capital structure analysis
- Interactive period selection

The objective of this page is to summarize the company's financial performance, profitability, solvency, growth trends, and capital structure in a single executive-level view.

### Executive Summary

Images/Dashboard/ExecutiveSummary.png

## Currently Working On

- Balance Sheet Analysis page
- Income Statement Analysis page
- Financial Ratios dashboard page
- Credit Risk dashboard page
- Rating agency metrics
- Covenant monitoring indicators
- Additional analytical measures
- Dashboard navigation experience
- Visual design refinement
- Dark theme implementation
- Report styling and visual consistency
- Visual formatting optimization

## Project Status

**Active Development**

Current version includes most of the financial ratios traditionally used in corporate financial analysis, credit risk assessment, and rating agency methodologies.

The project now incorporates a bilingual financial account structure, allowing local financial statements to be transformed into a standardized English reporting format suitable for international audiences and future multi-company analysis.

Although the Executive Summary page and the underlying analytical framework have been implemented, the project is not considered complete. The existence of functioning visualizations does not imply that the dashboard design phase has been finalized.

Current development efforts are increasingly focused on report design, user experience, visual consistency, layout optimization, and dashboard presentation quality.

A dark-theme reporting experience is planned for future versions. Visual colors, canvas formatting, navigation elements, and overall styling remain subject to refinement as the dashboard evolves.

Future development will focus on completing the remaining analytical pages, implementing credit risk monitoring features, enhancing covenant analysis, and maturing the overall reporting experience.

**Work in Progress**

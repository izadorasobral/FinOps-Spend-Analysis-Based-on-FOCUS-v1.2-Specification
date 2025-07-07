# FinOps Spend Analysis Dashboard (Power BI) – Based on FOCUS v1.2

📊 **Project Overview**  
This FinOps project demonstrates the creation of comprehensive dashboards for cloud cost analysis and optimization, strictly following the FOCUS v1.2 (FinOps Open Cost and Usage Specification). The goal is to provide clear visibility into spending across Cloud, SaaS, and PaaS environments, enabling effective cost monitoring, forecasting, and simulation.

---

✨ **Solution Highlights**

- **FOCUS v1.2 Implementation**  
  Data model manually built to follow FOCUS v1.2 principles for data standardization and invoice reconciliation.

- **Realistic Dataset**  
  Created from scratch to simulate real FinOps scenarios, including multiple cloud and SaaS providers, currencies, and pricing models.

- **Comprehensive Visibility**  
  Analysis of billed costs, effective costs, savings, and trends across time and services.

- **Scenario Simulation**  
  Simulates a 15% increase in AWS pricing to support proactive planning.

- **Contract Management**  
  Comparison between list prices and contracted prices to identify savings opportunities.

- **Support for SaaS/PaaS Billing Models**  
  Includes virtual currencies (credits/tokens), pricing and billing currencies, invoice granularity, and more.

---

🚀 **Dashboards**

This solution includes two interactive dashboards in Power BI, tailored for distinct user personas:

### 1. 📊 Executive Summary  
Designed for managers and decision-makers.  
Presents a high-level overview of:

- 🔹 Total Billed vs. Effective Costs  
- 🔹 Savings Percentage  
- 🔹 Monthly Trends  
- 🔹 Spend by Provider  
- 🔹 Simulation of a 15% AWS price increase  

### 2. 📈 Detailed Analysis  
Targeted at FinOps analysts and technical stakeholders.  
Provides deeper insights such as:

- 🔍 Spend by Service and Region  
- 🔍 Provider-level Savings Table (with conditional formatting)  
- 🔍 List vs. Contracted Price Comparison  
- 🔍 Dynamic Filters (Year, Month, Provider, Service, Account Type)  

---

⚙️ **Dataset Structure (FOCUS v1.2 Model)**

The dataset was modeled based on the FOCUS v1.2 specification, ensuring a unified and auditable view of cost and usage data.

Key columns include:

- `InvoiceId`, `BillingAccountType`, `SubAccountType`  
- `PricingCurrency`, `BillingCurrency`, `EffectiveCost`, `ListCost`, `ContractedCost`  
- `ConsumedQuantity`, `ConsumedUnit` (for virtual currencies)  
- `ProviderName`, `ServiceName`, `RegionId`, `ChargePeriodStart`, `ChargePeriodEnd`

> 💡 Note: This project uses simulated data based on the FOCUS v1.2 schema and does not reflect any real usage or spending.

---

🛠️ **Technologies Used**

- Power BI Desktop  
- DAX (Data Analysis Expressions)  
- Tabular Data Model  

---

📂 **Project Structure & How to Use**

1. **Download the Power BI Template**  
   Locate the `FOCUS12.pbit` file in the root of this repository.

2. **Open in Power BI Desktop**  
   Launch Power BI and open the `.pbit` file. The model and dashboards will load automatically.

3. **Explore Dashboards**  
   Navigate between the "Executive Summary" and "Detailed Analysis" pages to explore insights and interact with filters.

---

### 📂 Sample Dataset

A sample CSV file is included to support testing and exploration:  
[`samples/focus_simulated_dataset_focus_1.2.csv`](samples/focus_simulated_dataset_focus_1.2.csv)

---

This file contains representative records following the FOCUS v1.2 specification, including key columns such as `InvoiceId`, `ServiceName`, `EffectiveCost`, `RegionId`, and `ChargePeriodStart`. It is ideal for validating Power BI dashboards, building pipeline prototypes, or educational purposes.

📸 **Screenshots**

#### Executive Summary Dashboard  
![Executive Summary](assets/Executive%20Summary.png)

#### Detailed Analysis Dashboard  
![Detailed Analysis](assets/Detailed%20Analysis.png)
---

🤝 **How to Contribute**  
Contributions are welcome! Feel free to open issues, suggest improvements, or submit pull requests.

---

📄 **License**  
This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for details.


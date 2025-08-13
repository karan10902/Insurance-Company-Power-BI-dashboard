# EIC Motor Insurance Analysis | Power BI Dashboard

<img width="1295" height="723" alt="image" src="https://github.com/user-attachments/assets/f7c1fd1f-64a7-4eee-983b-be0f4698d17b" />


> **A comprehensive Power BI analysis of EIC's financial collapse - revealing the story behind Bangladesh's prominent motor insurer that closed in 2019**

## 📋 Table of Contents
- [🎯 Project Overview](#-project-overview)
- [📊 Dashboard Preview](#-dashboard-preview)
- [🔍 Key Findings](#-key-findings)
- [🛠️ Technical Implementation](#️-technical-implementation)
- [⚙️ Installation & Setup](#️-installation--setup)
- [🎓 Skills Demonstrated](#-skills-demonstrated)
- [📚 Business Intelligence Concepts](#-business-intelligence-concepts)
- [🚀 Future Enhancements](#-future-enhancements)
- [🤝 Connect With Me](#-connect-with-me)

## 🎯 Project Overview

### The Business Problem
**EIC (Eastern Insurance Company)** was one of Bangladesh's most prominent motor insurers during 2014-2018, but closed operations in 2019 due to consistent insurance losses. This project analyzes their financial performance to understand what went wrong and extract lessons for the insurance industry.

### The Solution
An interactive Power BI dashboard that provides comprehensive analysis across:
- **Financial Performance**: Premium vs. claims analysis over 5 years
- **Customer Segmentation**: Demographics and policy distribution patterns
- **Risk Assessment**: Vehicle type profitability and loss ratios
- **Trend Analysis**: Quarterly and yearly performance tracking

### Why This Matters
- **Industry Relevance**: Bangladesh's motor insurance market is projected to grow from $3.2B to $4.2B by 2032
- **Risk Management**: Understanding failure patterns helps prevent future collapses
- **Regulatory Insights**: Provides data for policy and compliance improvements

## 📊 Dashboard Preview

### Executive Summary Dashboard
![Executive Dashboard](<img width="1289" height="708" alt="image" src="https://github.com/user-attachments/assets/5a9ce9eb-f9a8-4efd-9205-e9ebb188e401" />
<img width="1289" height="708" alt="image" src="https://github.com/user-attachments/assets/19d40d91-50b0-4111-aeeb-5660b1201b4d" />
)
*Key performance indicators and financial trends overview*

### Detailed Analytics Dashboard
![Detailed Analytics](<img width="1295" height="723" alt="image" src="https://github.com/user-attachments/assets/b410f6ae-b86d-4591-8ff1-1bcf71f92faa" />
<img width="1295" height="723" alt="image" src="https://github.com/user-attachments/assets/ffdb5c29-937c-4355-812a-5f9f7802d2ff" />
)
*Customer segmentation, vehicle analysis, and profitability breakdown*

## 🔍 Key Findings

### 💰 Critical Financial Metrics

| **Metric** | **Value** | **Industry Benchmark** | **Status** |
|------------|-----------|------------------------|------------|
| **Total Premium** | $4 Billion | - | ✅ |
| **Total Claims** | $9 Billion | - | ❌ |
| **Loss Ratio** | **225%** | 60-80% | 🔴 Critical |
| **Average Premium** | $8K | - | ✅ |
| **Average Claim** | $18K | $6K-10K | ❌ |
| **Policy Count** | 66K | - | ✅ |
| **Claim Count** | 38K | - | ⚠️ High |

### 📈 Critical Insights

> **🚨 The Death Spiral: Claims exceeded premiums by 125% - a clear indicator of severe underpricing and poor risk management**

#### Financial Performance Issues
- **Unsustainable Loss Ratio**: At 225%, EIC paid $2.25 in claims for every $1 collected in premiums
- **Premium Inadequacy**: Average claim ($18K) was 2.25x higher than average premium ($8K)
- **Deteriorating Trends**: Loss ratios worsened significantly from 2016-2018
- **Cash Flow Crisis**: Negative cash flow from operations year-over-year

#### Customer & Market Analysis
- **Policy Distribution**: 66K policies across diverse vehicle categories
- **Gender Split**: 60% Male, 33% Female, 7% Other
- **High-Risk Segments**: Trucks (11.2K policies) and Pick-ups (12.7K policies) showed highest claim rates
- **Profitability Variance**: Agricultural vehicles were most profitable, commercial transport least profitable

#### Vehicle Category Performance
| **Vehicle Type** | **Policy Count** | **Risk Level** | **Profitability** |
|------------------|------------------|----------------|-------------------|
| Pick-up | 12.7K | High | ❌ Loss-making |
| Truck | 11.2K | Very High | ❌ Loss-making |
| Automobile | 10.0K | Medium | ⚠️ Break-even |
| Motor-cycle | 9.8K | High | ❌ Loss-making |
| Bus | 9.5K | Very High | ❌ Loss-making |

## 🛠️ Technical Implementation

### Data Architecture
```
📊 Data Sources
├── 📄 Policy Database (66K records)
├── 💰 Claims Database (38K claims)  
├── 👥 Customer Demographics
└── 📅 Financial Reports (Quarterly)
         ↓
🔄 Data Transformation (Power Query)
         ↓
📐 Data Model (Star Schema)
         ↓
📊 DAX Calculations & Measures
         ↓
📈 Interactive Dashboards (2 pages)
```

### Data Model Structure
- **Fact Tables**: 
  - `Policies` (66K rows) - Premium, dates, customer IDs
  - `Claims` (38K rows) - Claim amounts, policy references, dates
- **Dimension Tables**:
  - `Customers` - Demographics, contact info
  - `Vehicles` - Type, usage, specifications
  - `Calendar` - Date hierarchy for time intelligence
  - `Geography` - Location-based analysis

### Power BI Features Utilized
- ✅ **Interactive Filtering**: Cross-filtering between visuals
- ✅ **Drill-Through Pages**: Detailed analysis capabilities  
- ✅ **Time Intelligence**: Year-over-year comparisons
- ✅ **Conditional Formatting**: Color-coded performance indicators
- ✅ **Custom Tooltips**: Additional context on hover
- ✅ **Mobile Layout**: Responsive design for mobile devices

## ⚙️ Installation & Setup

### Prerequisites
- **Microsoft Power BI Desktop** (Latest version)
- **Excel 2016+** or **CSV support** for data files
- **4GB RAM minimum** (8GB recommended for optimal performance)

#### 2. File Structure Overview
```
eic-insurance-powerbi-analysis/
├── 📁 data/
│   ├── eic_policies.csv           # Policy data (66K records)
│   ├── eic_claims.csv             # Claims data (38K records)
│   ├── customer_demographics.csv  # Customer info
│   └── vehicle_categories.csv     # Vehicle classifications
├── 📁 powerbi/
│   ├── EIC_Insurance_Analysis.pbix # Main dashboard file
│   └── EIC_Mobile_Layout.pbix     # Mobile-optimized version
├── 📁 images/
│   ├── dashboard-overview.png
│   ├── dashboard-details.png
│   └── data-model.png
├── 📁 documentation/
│   ├── data-dictionary.md
│   ├── dax-measures.txt
│   └── business-requirements.md
└── README.md
```

#### 3. Open Dashboard
1. Download and install [Power BI Desktop](https://powerbi.microsoft.com/desktop/)
2. Open `EIC_Insurance_Analysis.pbix`
3. Click **"Refresh"** to load data (if prompted)
4. Navigate between dashboard pages using tabs at bottom

#### 4. Data Source Configuration
If you encounter data source errors:
1. Go to **Transform Data** → **Data source settings**
2. Update file paths to match your local directory
3. Apply changes and refresh

```

## 🎓 Skills Demonstrated

### Power BI Technical Expertise
- 🔧 **Advanced DAX Programming**: Complex calculations, time intelligence, statistical functions
- 📊 **Data Modeling**: Star schema design, relationship management, performance optimization
- 🎨 **Visualization Design**: Interactive dashboards, conditional formatting, user experience design
- 📱 **Responsive Design**: Mobile layouts, cross-platform compatibility

### Business Intelligence & Analytics
- 📈 **KPI Development**: Insurance-specific metrics, performance indicators, benchmarking
- 🔍 **Trend Analysis**: Time series analysis, seasonal patterns, growth calculations
- 🎯 **Risk Assessment**: Segmentation analysis, profitability modeling, loss prediction
- 💡 **Strategic Insights**: Root cause analysis, business recommendations, industry comparison

### Insurance Domain Knowledge
- 💰 **Actuarial Concepts**: Loss ratios, premium adequacy, reserve calculations
- ⚖️ **Risk Management**: Portfolio diversification, underwriting principles, claim patterns
- 📋 **Regulatory Understanding**: Industry standards, compliance requirements, reporting
- 🏢 **Market Analysis**: Competitive landscape, customer behavior, industry trends

## 📚 Business Intelligence Concepts

### Insurance Industry Fundamentals

#### Loss Ratio Analysis
The **Loss Ratio** is the cornerstone metric in insurance analysis:
- **Formula**: `(Total Claims / Total Premiums) × 100`
- **Industry Standards**:
  - **Excellent**: 40-60% (High profitability)
  - **Good**: 60-80% (Sustainable business)
  - **Warning**: 80-100% (Margin pressure)
  - **Critical**: >100% (Unsustainable losses)
  - **EIC's Reality**: 225% (Business failure inevitable)

#### Combined Ratio Framework
```
Combined Ratio = Loss Ratio + Expense Ratio
Where:
- Loss Ratio = Claims / Premiums
- Expense Ratio = Operating Expenses / Premiums
- Target: <100% for profitability
```

#### Premium Adequacy Assessment
Key factors in pricing accuracy:
- **Risk Assessment Quality**: How well risks are evaluated
- **Historical Data Usage**: Learning from past claims patterns  
- **Market Competition**: Pressure to underprice for market share
- **Regulatory Constraints**: Minimum coverage requirements

### Data Modeling Best Practices

#### Star Schema Design Benefits
- **Performance**: Faster query execution
- **Simplicity**: Intuitive relationships  
- **Scalability**: Easy to add new dimensions
- **User-Friendly**: Business users can understand structure

#### DAX Optimization Techniques
```dax
// ❌ Inefficient: Multiple table scans
Bad Measure = 
SUM(Table1[Column]) + SUM(Table2[Column]) + SUM(Table3[Column])

// ✅ Efficient: Single context transition
Good Measure = 
SUMX(
    VALUES(CommonDim[Key]),
    SUM(Table1[Column]) + SUM(Table2[Column]) + SUM(Table3[Column])
)
```

## 🚀 Future Enhancements

### Phase 1: Advanced Analytics (In Progress)
- [ ] **Predictive Modeling**: ML-based claim amount prediction
- [ ] **Geographic Analysis**: Interactive maps with regional risk patterns
- [ ] **Customer Lifetime Value**: CLV calculations and segmentation
- [ ] **Fraud Detection**: Anomaly detection in claims patterns

### Phase 2: Real-Time Integration (Planned)
- [ ] **Live Data Connections**: Real-time premium and claims updates
- [ ] **Automated Alerts**: Email notifications for KPI thresholds
- [ ] **API Integration**: Connect to external data sources
- [ ] **Mobile App**: Power BI Mobile optimization

### Phase 3: Advanced Features (Future)
- [ ] **Natural Language Queries**: Q&A visual integration
- [ ] **AI Insights**: Automated insights and explanations
- [ ] **Comparative Benchmarking**: Industry standard comparisons
- [ ] **Scenario Planning**: What-if analysis capabilities

### Technical Roadmap
- [ ] **Performance Optimization**: Large dataset handling improvements
- [ ] **Data Pipeline**: Automated ETL using Power Platform
- [ ] **Version Control**: Git integration for collaborative development
- [ ] **Testing Framework**: Automated testing for DAX calculations

## 🔄 Project Evolution

### Version History
- **v1.0** (Current): Basic financial analysis and customer segmentation
- **v1.1** (Next): Enhanced visualizations and mobile responsiveness  
- **v2.0** (Q2 2024): Predictive analytics integration
- **v3.0** (Q4 2024): Real-time data and advanced AI features

### Community Contributions
Interested in contributing? Here's how:
1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/AmazingFeature`)
3. **Commit** your changes (`git commit -m 'Add some AmazingFeature'`)
4. **Push** to the branch (`git push origin feature/AmazingFeature`)
5. **Open** a Pull Request



## 🤝 Connect With Me

**👨‍💻 Created by:** Karan

**🔗 Professional Links:**
- 💼 **LinkedIn:** https://www.linkedin.com/in/karan-kumar-78936219a
- 🐱 **GitHub:** https://github.com/karan10902
- 📧 **Email:** karankumar59mg@gmail.com

**🎯 Specializations:**
- Business Intelligence & Analytics
- Power BI Development & Consulting
- Insurance Industry Analysis
- Financial Risk Assessment

---

### Data Disclaimer
This project uses anonymized and aggregated data for educational purposes. All sensitive information has been removed or modified to protect privacy while maintaining analytical value.

### Acknowledgments
- 🙏 **Insurance Industry Professionals** for domain knowledge guidance
- 🌟 **Power BI Community** for technical support and best practices
- 📊 **Open Source Contributors** for tools and methodologies used
- 🎓 **Educational Institutions** for fostering data literacy

---

#PowerBI #DataAnalysis #Insurance #BusinessIntelligence #DAX #DataVisualization #Analytics #RiskManagement

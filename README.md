
# DS200 Research Methods Assignment

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/suryasud/DS200-data-science-visualizations/blob/main/data_visualization_using_python.ipynb)
<p>
    The Google Colab notebook can also be viewed and run on this raw website 
    in case the above link does not work: 
    <a href="https://colab.research.google.com/drive/1eKFF6DK05pREa5zKSmqNgR0JTOH-Ew69?usp=sharing">Colab Notebook Direct Link</a>.
</p>

# Data Visualization
This assignment is done as a part of  **DS200: Research Methods** course requirement. <br>
This is to demonstrate foundational skills in data analysis and visualization.

## Author
**Surya Datta Sudhakar** ([GitHub](https://github.com/suryasud)) <br>
Department of Computational and Data Sciences, <br>
Indian Institute of Science, Bengaluru.

## Dataset used
<p>
    The <strong>data</strong> used in this assignment is <strong>sourced</strong> from <a href="https://data.gov.in">data.gov.in</a>. <br>
    Click on the link below to access the original data source <br>
    <a href="https://www.data.gov.in/resource/central-sector-schemes-2020-2021-2020-21-2022-23">Central Sector Schemes (2020-2021, 2021-22, 2022-23)</a>
</p>

<p>
    The dataset can be directly downloaded from a copy that I have saved on Google Drive. <br>
    Click on the link below to directly download the <kbd>CentralSectorSchemes.csv</kbd> file <br>
    <a href="https://drive.google.com/file/d/1jkoynty9n0Z5q2R7LjJG5xIsByZ-FdpH/view?usp=sharing">Central Sector Schemes Dataset csv file</a>
</p>

> [!IMPORTANT]
> If running offline, please make sure to have the following
> python libraries installed. <br>
> pandas, matplotlib, seaborn, numpy

## Inferences
Analysis of Ministry Budget Allocations for Central Sector Schemes

-----

### 1. Top 10 Schemes by Actual Revenue (2020-2021) (BAR PLOT)
<strong> Key Points </strong> <br>
- **Heavy Budget Concentration**: The top three ministries—Consumer Affairs (26.9%), Railways (17.5%), and Defence (17.0%)—command a staggering 61.4% of the total budget among the top 10. This indicates a massive concentration of funds in a few key areas.
- **Significant Drop-off**: There is a sharp decline in budget allocation after the top three. The next tier, including Home Affairs (11.0%) and Road Transport (10.9%), receives a substantial but markedly smaller share.
- **The "Other" Category is Small**: The combined budget of the bottom four ministries in this list (Rural Development, Agriculture, Health, and Education) is less than the individual budget of any of the top three, highlighting a steep priority gradient.

<strong>Inferences</strong> <br>
- **Core National Priorities**:
The data strongly suggests that government spending is focused on three core areas: Public Welfare & Food Security (Consumer Affairs), National Infrastructure (Railways & Road Transport), and National Security (Defence & Home Affairs). These sectors are clear financial priorities.
- **Clear Spending Hierarchy**:
The donut chart reveals a distinct hierarchy in funding. It's not an even distribution but a strategic allocation where a few ministries receive the lion's share, reflecting their perceived importance to the nation's immediate objectives for the fiscal year.
- **Social Sectors Follow Core Infrastructure**:
While important, foundational social sectors like Agriculture, Rural Development, Health, and Education have a smaller piece of the pie compared to infrastructure and security, indicating their relative position in the budget hierarchy for this period.

-----

### 2. Lowest 10 Schemes by Actual Revenue (2020-2021) (BAR PLOT)

<strong>Key Points</strong> <br>
- **Uneven Revenue–Capital Mix**: Most ministries, such as Panchayati Raj and Public Enterprises, exhibit much higher revenue expenditure than capital, showing a focus on administrative and operational costs rather than asset creation.
- **Capital-Dominant Outliers**: In contrast, Ministry of Railways and Defence Services stand out with disproportionately high capital expenditure, highlighting their infrastructure-intensive nature.
- **Log-Scale Emphasis**: The log-scaled y-axis reveals massive differences—capital spending in some ministries spans several orders of magnitude above revenue spending.

<strong>Inferences</strong> <br>
- **Infrastructure-Centric Outliers**: Ministries like Railways and Defence Services are clear exceptions among the lowest 10, driven by capital-heavy projects such as construction, procurement, and modernization.
- **Operational Overheads in Smaller Ministries**: Smaller departments (e.g., Corporate Affairs, Public Enterprises) primarily channel funds toward maintenance, salaries, and ongoing programs rather than long-term investments.
- **Fiscal Imbalance Across Ministries**: The steep variance in capital spending signals unequal capacity or necessity for physical infrastructure across ministries, underscoring the varied nature of their functional responsibilities.

-----

### 3. Correlation Between FY21 Capital Expenditure and FY22 Budget Projections (SCATTER PLOT)

**Key Points** <br>
- **Positive Correlation Trend**: Both revenue (red) and capital (blue) estimates for FY22 increase with higher FY21 capital expenditure, indicating that ministries with strong capital spending in FY21 received proportionally higher budget allocations the following year.
- **Dual Estimate Comparison**: The scatter shows **blue (capital)** points clustering closer along the main growth trend than **red (revenue)** ones — suggesting a stronger direct link between prior-year capital outlay and future capital budgeting than with revenue budgeting.
- **Wide Range of Scale**: The log–log scale reveals an expenditure spread across nearly **seven orders of magnitude**, highlighting stark differences between smaller ministries and large infrastructure or defense sectors.

**Inferences** <br>
- **Capital Spending Rewards Future Allocation**: Ministries that effectively utilized capital budgets in FY21 tended to receive increased capital allocations for FY22, reflecting a performance-linked budgeting approach.
- **Revenue Budgets Less Predictive**: The weaker alignment of red points suggests that **revenue allocations** are influenced by operational or policy factors rather than previous capital investment levels.
- **Structural Spending Divide**: The presence of distinct clusters (small, medium, large ministries) implies a **tiered budget ecosystem**, where only a few ministries dominate total capital flows while most operate on much smaller financial scales.

-----

### 4. Distribution of Scheme Budgets for Top 20 Ministries (FY 2022–23) (BOX PLOT)

**Key Points** <br>
- **High Variability Across Ministries**: The box plots show wide variation in scheme budgets across ministries — with **Road Transport & Highways**, **Agriculture & Farmers Welfare**, and **Defence Services** exhibiting particularly large ranges.
- **Log-Scale Spread**: Budgets span an enormous scale — from fractions of a crore to nearly **₹10⁵ crores**, highlighting the vastly different magnitudes of financial responsibility across ministries.
- **Concentrated vs. Dispersed Allocations**: Some ministries, like **Defence (Civil)** and **Power**, have tightly grouped budgets (low variance), whereas **Road Transport & Highways** and **Agriculture** show much broader distributions, suggesting multiple high-value schemes within.

**Inferences** <br>
- **Infrastructure and Agriculture Lead in Budget Breadth**: The expansive budget ranges for **Road Transport & Highways** and **Agriculture & Farmers Welfare** reflect their extensive scheme portfolios and strong capital investment focus.
- **Strategic and Scientific Stability**: Ministries like **Space**, **Biotechnology**, and **Science & Technology** maintain moderate, consistent allocations, indicating steady long-term investment in innovation rather than large one-time projects.
- **Defense and Power Maintain Core Funding Blocks**: The **Defence (Civil)** and **Power** ministries show controlled yet high baseline allocations, underscoring their role as essential public service and national security anchors with predictable funding continuity.

-----

### 5. Budget Share of Top 10 Ministries (FY 2022-23)

<strong>Key Points</strong><br>
- The largest budget shares are held by Department of Food and Public Distribution (21.0%) and Ministry of Road Transport and Highways (20.2%), together covering more than 41% of the budget.
- Capital Outlay on Defence Services (15.4%) and Ministry of Railways (13.9%) are also significant budget recipients, indicating strong allocation toward defense and transport infrastructure.
- The remaining ministries such as Department of Agriculture and Farmers Welfare, Department of Fertilizers, and others have much smaller shares, mostly below 11%, showing a spread of budget but with less concentration.

<strong>Inferences</strong><br>
- The budget evidently prioritizes essential services related to food distribution, transport infrastructure, and defense, reflecting core national economic and security priorities.
- Ministries with more specialized or less broad-reaching mandates like Micro, Small and Medium Enterprises, Labour and Employment, and Health/Family Welfare receive comparatively minor shares, possibly indicating less budgetary emphasis.
- The presence of relatively balanced but smaller allocations to social and industrial sectors may reflect a diversified budget approach, but with dominant focus on food security, transportation, and defense spending.












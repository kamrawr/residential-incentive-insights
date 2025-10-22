# Residential Incentive Insights

An interactive web application providing comprehensive guidance for residential energy efficiency incentive programs. Built for program managers, homeowners, and contractors to quickly access actionable insights for energy upgrade projects, combining **Energy Trust of Oregon** programs (Standard, SWR, CPF, CERTA) with **federal HOMES and HEAR rebates**.

## ⚠️ IMPORTANT DISCLAIMER - READ BEFORE USE

**This is an UNOFFICIAL, informational reference tool only.** It does not represent official guidance, recommendations, or endorsements from Energy Trust of Oregon, any government agency, or program administrator.

### Critical Warnings:
- **DO NOT make financial purchases or commitments based solely on this information**
- All program data is compiled from publicly available sources and may be **outdated, incomplete, or inaccurate**
- Incentive amounts, income limits, and program requirements **change frequently** and vary by location
- Federal HOMES/HEAR programs **may not be fully implemented** in all states
- This tool is provided **"as-is" without warranties of any kind**
- The author **assumes no liability** for decisions made based on this information

### Before Taking Action:
1. **Verify ALL information** directly with official program administrators
2. **Confirm current eligibility** criteria and incentive amounts
3. **Consult qualified professionals** and obtain multiple quotes
4. **Review official program documentation** and application requirements
5. **Never rely solely on this tool** for significant financial decisions

## 🌐 Live Application

**[View the Interactive Application](https://kamrawr.github.io/residential-incentive-insights/)**

## 📋 Overview

This application provides comprehensive information about residential energy efficiency incentive programs, combining **state and federal funding sources**:

### Energy Trust of Oregon Programs
- **Standard Incentives**: Available to all qualifying households
- **SWR (Standard Wrap Rate)**: Enhanced incentives for households earning 60-80% AMI
- **CPF (Community Partner Fund)**: Comprehensive funding for priority households ≤60% AMI
- **CERTA (Clean Energy Repair & Technical Assistance)**: Up to $2,000 for structural/safety barrier removal

### Federal IRA Programs
- **HOMES Rebate**: Performance-based rebates ($2,000-$8,000) for whole-home energy savings
- **HEAR Rebate**: Point-of-sale rebates for electric appliances (heat pumps up to $8,000, HPWHs up to $1,750, insulation up to $1,600, electrical upgrades up to $4,000)

### Project Types Covered
- **Heat Pumps** (ductless, ducted, extended-capacity) - _Stackable with HEAR rebates_
- **Gas Heating Systems** (furnaces & fireplaces)
- **Water Heating Systems** (heat-pump & tankless gas) - _HPWH eligible for HEAR_
- **Insulation & Envelope** (attic, wall, floor) - _Eligible for HEAR + HOMES rebates_
- **Windows** - _Contributes to HOMES whole-home savings_
- **Controls & Thermostats**
- **Home Energy Assessment & CERTA** - _Required for HOMES rebate qualification_

## ✨ Features

- **Comprehensive Funding Information**: Integrates Energy Trust of Oregon programs (SWR, CPF, CERTA) with federal HOMES/HEAR rebates
- **Interactive Program Tooltips**: Hover over program acronyms (SWR, CPF, CERTA, HOMES/HEAR) for detailed descriptions
- **Income Qualification Guidance**: Clear eligibility criteria for each program tier with AMI thresholds
- **Rebate Stacking Strategies**: Shows how to combine state and federal incentives for maximum savings
- **Multi-Audience Views**: Filter content by Program Manager, Homeowner, or Contractor perspectives
- **Real-Time Search**: Instantly search across all project types, programs, and recommendations
- **Multi-Select Filters**: Select multiple project types and audiences simultaneously
- **Light/Dark Mode**: Toggle between themes for comfortable viewing
- **Export Capabilities**: Copy visible insights or export filtered data as JSON
- **Cost Analysis**: View typical costs, incentive amounts, coverage percentages, and federal rebate eligibility
- **Impact Tags**: Quick visual indicators for project impact and characteristics
- **Contextual Overviews**: Dynamic project-specific guidance that updates based on selections
- **Offline Ready**: Fully functional without internet connection after initial load

## 📊 Data Summary Report

### Project Types (7 total)

1. **heat_pumps**
2. **gas_heating_systems**
3. **water_heating_systems**
4. **insulation_and_envelope**
5. **windows**
6. **controls_and_thermostats**
7. **home_energy_assessment_and_certa**

### Data Structure

Each project type contains:

#### Core Fields
- `title` (string): Full project name
- `summary` (string): Brief description of impact and characteristics
- `impact_tags` (array): 2 tags indicating project characteristics

#### Cost & Incentive Data (`cost_and_incentive_ratio` object)
Varies by project type, includes fields such as:
- Cost ranges (USD)
- Incentive amounts (USD)
- Coverage percentages
- Special funding (SWR, CPF, CERTA)

#### Strategic Information
- `equity_and_market_leverage` (array): 2 items per project
- `implementation_priorities` (array): 2 items per project

#### Stakeholder-Specific Guidance (`stakeholder_value` object)
Each contains 2 actionable items per audience:
- `program_manager` (array)
- `homeowner` (array)
- `contractor` (array)

### Impact Tags Summary

**By Category:**
- **Energy Impact**: High impact, Very high impact, Moderate impact, Medium impact
- **System Type**: Electrification, Combustion, Hot water, Weatherization, Behavior + control
- **Performance**: High ROI, Comfort, Low energy ROI
- **Program Function**: Enablement, Pipeline

**Tag Distribution:**
- High impact: 1 project
- Very high impact: 1 project
- Moderate impact: 1 project
- Medium impact: 1 project
- Electrification: 1 project
- Combustion: 1 project
- Hot water: 1 project
- Weatherization: 1 project
- Comfort: 1 project
- Low energy ROI: 1 project
- High ROI: 1 project
- Behavior + control: 1 project
- Enablement: 1 project
- Pipeline: 1 project

### Cost & Incentive Fields Summary

**Total unique cost/incentive fields across all projects: 24**

By Project:
- **heat_pumps**: 4 fields (average_cost_usd, standard_incentive_usd, coverage_percent, swr_cpf_coverage_percent)
- **gas_heating_systems**: 5 fields (furnace_cost_usd, furnace_incentive_usd, coverage_percent, fireplace_cost_usd, fireplace_incentive_usd)
- **water_heating_systems**: 4 fields (hpwh_cost_usd, hpwh_incentive_usd, tankless_cost_usd, tankless_incentive_usd)
- **insulation_and_envelope**: 4 fields (average_cost_per_sqft_usd, standard_coverage, swr_cpf_coverage, certa_fund_usd)
- **windows**: 3 fields (avg_window_cost_usd, incentive_per_sqft_usd, coverage_percent)
- **controls_and_thermostats**: 3 fields (device_cost_usd, incentive_usd, coverage_percent)
- **home_energy_assessment_and_certa**: 4 fields (audit_cost_usd, rebate_usd, coverage_percent, certa_funding_usd)

### Audience Options (3 total)

1. **Program Manager**: Strategic implementation and funding coordination
2. **Homeowner**: Cost savings, comfort benefits, and eligibility
3. **Contractor**: Technical requirements, documentation, and installation guidance

## 🚀 Usage

### Understanding Program Acronyms
- **Hover over program names** (SWR, CPF, CERTA, HOMES/HEAR) in the subtitle for detailed descriptions
- **Check the Program Overview section** for income qualification details and eligibility criteria
- **Review each project card** for program-specific rebate stacking opportunities

### Filtering
1. **Search**: Type keywords in the search bar (e.g., "ductless", "CPF", "CERTA", "HEAR", "HOMES")
2. **Project Types**: Select multiple project types using checkboxes
3. **Audiences**: Filter by Program Manager, Homeowner, or Contractor perspectives (multi-select)
4. **Theme Toggle**: Switch between light and dark modes for comfortable viewing

### Maximizing Rebate Stacking
- Look for projects with **multiple funding sources** listed (Energy Trust + CERTA + HEAR/HOMES)
- **Heat pumps**: Combine Energy Trust incentives with HEAR rebates (up to $8,000)
- **Insulation**: Stack Energy Trust, CERTA, HEAR ($1,600), and HOMES ($2,000-$8,000)
- **Whole-home projects**: Pursue HOMES rebates for comprehensive upgrades

### Sharing & Exporting
- **Copy Insights**: Copy all visible card content to clipboard
- **Export JSON**: Download filtered data as JSON file
- **Per-Card Actions**: Each card has copy and JSON export buttons

## 🛠️ Technical Details

### Technology Stack
- **Pure HTML/CSS/JavaScript** - No build tools required
- **Modern CSS** - CSS Grid, Custom Properties, Dark theme optimized
- **Vanilla JavaScript** - No framework dependencies
- **Responsive Design** - Mobile-first approach

### File Structure
```
residential-incentive-insights/
├── index.html          # Main application (self-contained)
├── data.json          # Structured data export
└── README.md          # This file
```

## 📦 Development

### Running Locally
Simply open `index.html` in a modern web browser. No server required.

### Modifying Data
Update the `DATA` object in the `<script>` section of `index.html`, or use `data.json` as a reference.

## 🤝 Contributing

This is an educational resource. To suggest improvements:
1. Fork the repository
2. Make your changes
3. Submit a pull request with a clear description

## 📄 Data Sources & Accuracy

**All information is approximate and subject to change without notice.**

- **Energy Trust of Oregon**: Program information compiled from publicly available Energy Trust documentation (may be outdated)
- **Federal Programs**: HOMES and HEAR rebate information based on federal Inflation Reduction Act guidelines (implementation varies by state)
- **Income Thresholds**: AMI percentages and dollar amounts are **approximate examples only** and vary significantly by county, household size, and program year
- **Costs & Incentives**: All dollar amounts are **typical ranges** and may not reflect current actual costs or available incentives
- **No Guarantee of Accuracy**: Information may contain errors, omissions, or outdated data

### ⚠️ Verification Required Before ANY Action
**ALWAYS verify the following directly with official program administrators:**
- Current program availability and status
- Exact income limits and eligibility criteria
- Actual incentive/rebate amounts
- Application processes and deadlines
- Technical requirements and specifications

### Official Resources (Use These for Authoritative Information)
- **Energy Trust of Oregon**: [energytrust.org](https://www.energytrust.org) - Official source for Standard, SWR, CPF, CERTA programs
- **Federal HOMES/HEAR Programs**: Contact your state energy office or visit [energy.gov](https://www.energy.gov) - Verify state implementation status

## 📄 License

This project is provided as educational and informational content only. Data is compiled from publicly available sources for reference purposes and does not constitute official program guidance, professional advice, or recommendations.

**No warranties, express or implied.** The author disclaims all liability for the accuracy, completeness, or usefulness of this information.

## 📧 Contact

For **authoritative, official information** contact:
- **Energy Trust programs (Standard, SWR, CPF, CERTA)**: Energy Trust of Oregon at [energytrust.org](https://www.energytrust.org)
- **Federal HOMES/HEAR rebates**: Your state energy office or local program administrator
- **Professional advice**: Licensed contractors, energy auditors, or program-certified professionals

For **questions about this unofficial tool only**: Submit issues or suggestions via the GitHub repository

---

**⚠️ Final Reminder:** This unofficial tool provides approximate reference information compiled from publicly available sources. **Never make significant financial purchases or commitments based solely on this information.** Always verify current specifications, program requirements, eligibility criteria, and incentive amounts with official program administrators and obtain professional quotes before proceeding with any energy efficiency projects.

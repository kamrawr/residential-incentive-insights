# Residential Incentive Insights

An interactive web application providing data-driven guidance for residential energy efficiency incentive programs. Built for program managers, homeowners, and contractors to quickly access actionable insights for various energy upgrade projects.

## 🌐 Live Application

**[View the Interactive Application](https://kamrawr.github.io/residential-incentive-insights/)**

## 📋 Overview

This application provides comprehensive information about residential energy efficiency incentive programs, including:

- **Heat Pumps** (ductless, ducted, extended-capacity)
- **Gas Heating Systems** (furnaces & fireplaces)
- **Water Heating Systems** (heat-pump & tankless gas)
- **Insulation & Envelope** (attic, wall, floor)
- **Windows**
- **Controls & Thermostats**
- **Home Energy Assessment & CERTA**

## ✨ Features

- **Multi-Audience Views**: Filter content by Program Manager, Homeowner, or Contractor perspectives
- **Real-Time Search**: Instantly search across all project types and recommendations
- **Deep Linking**: Share specific project views with URL hash parameters (e.g., `#heat_pumps?aud=homeowner`)
- **Export Capabilities**: Copy visible insights or export filtered data as JSON
- **Cost Analysis**: View typical costs, incentive amounts, and coverage percentages
- **Impact Tags**: Quick visual indicators for project impact and characteristics
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

### Filtering
1. **Search**: Type keywords in the search bar (e.g., "ductless", "CPF", "audit")
2. **Project Type**: Select specific project from dropdown
3. **Audience**: Filter by Program Manager, Homeowner, or Contractor view

### Sharing & Exporting
- **Deep Links**: Use URL patterns like `#heat_pumps?aud=homeowner` to share specific views
- **Copy Insights**: Copy all visible card content to clipboard
- **Export JSON**: Download filtered data as JSON file
- **Per-Card Actions**: Each card has copy, JSON export, and deep link buttons

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

## 📄 License

This project is provided as educational content for energy efficiency program guidance.

## 📧 Contact

For questions or suggestions about the incentive program data, please contact your local energy efficiency program administrator.

---

**Built for quick, offline field use.** Always verify current specifications and program information sheets before finalizing quotes or applications.

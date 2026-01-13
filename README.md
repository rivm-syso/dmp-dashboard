# DMP Dashboard 

![GitHub Release](https://img.shields.io/github/v/release/rivm-syso/dmp-dashboard)

The DMP Dashboard is an open source tool designed to provide an overview and monitoring of Data Management Plans (DMPs) within research projects and organizations.

## Goal

The primary goal of this repository is to provide a simple, user-friendly dashboard that offers a clear overview of DMPs across research projects and organizations.

By focusing on ease of use and essential features, we aim to support data stewards, project leaders, and researchers in monitoring the status, progress, and compliance of DMPs without unnecessary complexity.

By sharing this tool publicly, we aim to support open science and open source collaboration across institutes.

## Features
- Overview of all DMPs in your organization
- Status tracking and compliance monitoring
- Easy-to-use visual dashboard (built with R and Flexdashboard)
- Export functionality to CSV

## Getting Started
Prerequisites
- R (version 4.4.3 or higher)
- RStudio

## Installation & Usage
1. Download or clone this repository:
```sh
git clone https://github.com/rivm-syso/dmp-dashboard.git
```

2. Open the project in RStudio:
- Double-click the .Rproj file

3. Install required packages:
**Recommended (reproducible setup)**:
This project uses renv for reproducible package management.
All necessary package versions are specified in the included renv.lock file.

```r
install.packages("renv")  # if not already installed
renv::restore()
```
This will automatically install all required packages.

**Alternative (manual setup)**:

If you prefer to install packages manually, make sure you have the following R packages installed:

```sh
install.packages(c("flexdashboard", "dplyr", "stringr", "plotly", "ggplot2", "lubridate", "DT"))
```

4. Launch the dashboard:
- Open dmp_flexdash.Rmd in the RStudio editor.
- Click the 'Run Document' button in the editor window.

## Customizing the Dashboard
You can easily tailor the DMP Dashboard to fit your organization's needs. Below are the main areas you can adjust in `dash_comps`:

### Change the Data
Replace the data file:
- Swap the example data file (e.g., `dmp_data/fake_dmp_data.csv`) with your own DMP data.
Adjust data structure:
- Ensure your data columns match the expected structure, or modify the data loading code in `global_setup.Rmd` to fit your data format.
Customize organizational hierarchy:
- By default, the dashboard uses the structure Domain/Centra/Department, but you can change this to match your organization's hierarchy (e.g., Faculty/Department/Group).

### Change the Logo
Replace the logo file:
- Add your institute's logo by replacing the file `www/logo/fake_logo_dmp_flex.svg` in the project directory.
Update the logo path:
- Make sure to update the path to the logo in the YAML header of `dmp_flexdash.Rmd`.

### Change Charts and Buttons
Customize dashboard components:
- Each button and chart has its own .Rmd file in the dash_comps folder. You can configure these files to modify or create new charts and buttons according to your preferences.

### Change Main Filters
Edit filters:
- You can configure which filters are available in the dashboard by editing `filter_data.Rmd`.

## Change General Stats
Adjust main statistics and layout:
- In `datatable_general_stats.Rmd`, you can change the position and structure of the main charts and tables to better suit your reporting needs.

## Contributing
We welcome feedback, suggestions, and contributions! Please see [CONTRIBUTING.md](CONTRIBUTING.md) before opening an issue or submiting a pull request.

## License
This project is licensed under the EUPL-1.2 License. See [LICENSE](LICENSE).

## Citing DMP Dashboard

If you use DMP Dashboard in your institute, organisation or project, please cite it appropriately. Citation information is provided in the [CITATION.cff](CITATION.cff) file included in this repository.

You can also find citation formats directly on the GitHub repository page by clicking the "Cite this repository" button.

## About
Developed by the team of data stewards inside RIVM, the DMP Dashboard is part of our commitment to open source and open science.
By making this tool available, we hope to foster best practices in research data management, both within our organization and the wider research community.

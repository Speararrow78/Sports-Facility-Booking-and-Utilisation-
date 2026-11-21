# Sports Facility Booking and Utilization Analysis

**Course:** DSC3132 — Business Analytics  
**Student:** Parag Patra  
**Topic:** Sports Facility Booking and Utilization  
**Analytics covered:** Descriptive Analytics and Diagnostic Analytics

## Project summary
This R Markdown project analyses sports facility booking activity, completed-hour utilization, revenue, peak demand periods, cancellations and no-shows. It uses two reproducible CSV datasets and includes data-quality checks, summary tables, visualisations, diagnostic group comparisons, recommendations, limitations and a data-access plan.

> **Important:** The supplied data is synthetic, generated for academic demonstration. It does not represent actual bookings or customers of a real sports facility.

## Repository structure

```text
sports_facility_booking_analytics/
├── Sports_Facility_Booking_Utilization.Rmd
├── README.md
├── DATA_DICTIONARY.md
├── .gitignore
└── data/
    ├── bookings.csv
    └── facilities.csv
```

## How to run the project

1. Install [R](https://cran.r-project.org/) and [RStudio](https://posit.co/download/rstudio-desktop/).
2. Download or clone this repository.
3. Open `Sports_Facility_Booking_Utilization.Rmd` in RStudio.
4. Click **Knit** to generate the HTML report.
5. If prompted, allow R to install the required packages: `tidyverse`, `lubridate`, `knitr`, and `scales`.

Run the notebook from the repository root so that the relative paths to `data/bookings.csv` and `data/facilities.csv` resolve correctly.

## Analytics questions

### 1. Descriptive analytics
**What are the booking, utilization and revenue patterns across sports facilities during January–March 2026?**

### 2. Diagnostic analytics
**Which facility, day/time and booking-channel patterns are associated with higher cancellation and no-show rates, and what operational issues may explain lower utilization?**

## Data access plan
The included CSV files are generated programmatically and committed to the repository for reproducibility. In a real deployment, equivalent data would be accessed—with permission—from the booking-management system, facility master records, attendance/check-in records and payment records. Personal identifiers should be excluded or anonymised before analysis.

## Utilization definition
Completed booking hours / (bookable units × operating hours per day × days in the analysis period) × 100.

This is a simplified measure. It assumes all bookable units are available for the stated operating hours and does not adjust for maintenance closures.

## Suggested GitHub upload

```bash
git init
git add .
git commit -m "Add sports facility booking and utilization analytics project"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/sports-facility-booking-analytics.git
git push -u origin main
```

Create an empty repository on GitHub first, then replace `YOUR-USERNAME` with your GitHub username. Do not upload private customer data, credentials or passwords.

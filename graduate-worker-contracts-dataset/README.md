# Graduate worker contracts and funding policies at US universities

Version 2026-10-17, published by the Academic Union Network (https://academic-union-network.org) under the Creative
Commons CC0 1.0 public domain dedication.

Pay rates, summer funding, tuition and fee waivers, health insurance, raises, and union events for graduate
student workers at 39 US universities. The figures come from union contracts and, where no contract sets pay,
from the universities' published pay tables and funding policies, with a few from university announcements, union
summaries, and news reports. Every fact cites the document, page, and passage it comes from, so each one can be
checked against its source.

## Files

- `institutions.csv`: One row per institution.
- `sources.csv`: One row per cited document.
- `agreements.csv`: One row per union contract or university policy that facts belong to.
- `rates.csv`: One row per pay rate as the source states it: hourly stays hourly, monthly stays monthly, with the appointment alongside. Annualized and converted monthly figures appear only in chart_picks.csv, for the rates the website charts.
- `terms.csv`: One row per benefit term in scope: summer funding, tuition and fee waivers, health insurance, and general increases (raises). A term with absent set to true records that the cited documents have no provision on the topic.
- `events.csv`: One row per union event: elections, recognition, bargaining, strike threats, strikes, ratification and expiration.
- `living_costs.csv`: One row per item of a university's published cost of attendance for graduate students: the school's own published figure for what a graduate student needs for a year, from its financial aid office. Items of one budget share its name.
- `fair_market_rents.csv`: For each campus and academic year, the Fair Market Rents that the U.S. Department of Housing and Urban Development (HUD) sets for the campus's area: the monthly rent, utilities included, that 40 percent of similar rentals in the area cost no more than. HUD fiscal year N is listed under academic year (N-1)-N.
- `citations.csv`: One row per cited passage. Every fact cites at least one; at least one quote states each figure. Absences cite the document without a quote.
- `chart_picks.csv`: The figure the website shows for each institution and academic year, with how it was derived; reason says why that rate represents the institution. The website shows the University of California's campuses separately, so it has a row for each campus.

`datapackage.json` describes every column, with keys linking the tables (Frictionless Data Package v2). The
comma-separated values (CSV) files are UTF-8 with a header row; lists within a cell are separated by "; ".

## Reading the data

- **Figures are stored as the source states them.** Hourly rates stay hourly and monthly rates monthly, with the
  appointment's months, weeks, hours, and full-time equivalent (FTE) alongside. Only `chart_picks.csv` holds
  figures converted to another unit (annual or monthly), each with how it was derived.
- **Know what a figure is before comparing it.** `component` separates combined total-support minimums, salaries,
  stipends, and top-ups; `basis` separates minimum pay (`minimum`), amounts paid (`exact`), stated aims (`intention`),
  and benefit eligibility thresholds (`threshold`). Appointment lengths differ (most are 9, 10, or 12 months), so
  compare annual figures only together with `appointment_months`.
- **Academic years.** A rate is labeled with the academic year it mostly covers; `effective` and `until` keep the
  source's own dates.
- **Absences are explicit.** A term with `absent` true means the cited document has no provision on the topic, and
  `searched` says what was checked. A topic with no row at all has not been researched for that institution.
- **Identifiers.** `fact_id` combines the institution id, the table, and the fact's position (or, for agreements,
  its id). Positions can change between versions, so match facts across versions by their content.

## Citing and reusing

To the extent possible under law, the Academic Union Network has waived all copyright and related rights to this
dataset (CC0 1.0, https://creativecommons.org/publicdomain/zero/1.0/). The short passages quoted in
`citations.csv` remain their authors' and are included only so that each fact can be verified. Credit is
appreciated but not required. The website suggests this line:

> Data: Academic Union Network, “Graduate worker contracts and funding policies at US universities,” version 2026-10-17, https://academic-union-network.org/contract-tracker/

## About this data, from the website

The website's own account of the data, as its tracker page (https://academic-union-network.org/contract-tracker/)
shows it. "The page", "the chart" and "the table" are that page's.

**Sources.** Most figures come from union contracts, published pay tables and university funding policies. A few come from university announcements, union summaries or news reports. Each figure links to the passage it comes from, and to an archived copy where one exists. We record figures as the source states them. Some sources state pay per hour or per term, as a full-time rate, or per month without a set appointment length. For these, we calculate the yearly figure and mark it with an asterisk (*) in the chart and “calculated” in the table.

**Rent and living costs.** The page compares pay with two measures of what it costs to live near campus. The first is rent: the Fair Market Rent that the U.S. Department of Housing and Urban Development (HUD) publishes for a one-bedroom apartment in each campus's area. It includes utilities, and HUD sets it so that 40 percent of similar rentals in the area cost this much or less. HUD publishes a new figure for each federal fiscal year, which begins in October. The page shows 12 months of this rent as a share of the year's pay. HUD considers renters who spend more than 30 percent of their income on rent to be cost-burdened. The second measure is living costs: the housing, food, transportation and personal expenses in the school's published cost of attendance for graduate students. The cost of attendance is the school's own figure for what a student needs. The page compares pay with these living costs month by month. Where a school pays for whole semesters over a different number of months than its cost of attendance covers, as Penn State does, the comparison is per semester instead.

**The living wage.** Many unions cite the living wage from the Massachusetts Institute of Technology (MIT) Living Wage Calculator. It is the hourly wage a full-time worker needs to pay for basic costs, including taxes, where they live. The calculator's terms allow its figures for more than ten places to be used only under a license, so this page does not show them. Instead, each school's details link to the calculator's page for the campus's county.

**Limits.** Contracts and policies change, and documents can be unclear. Despite our checks, the data may contain errors. Minimum pay is the least a school may pay for an appointment, not what a typical student receives. Appointment lengths and weekly hours differ between schools, so read a figure's details before comparing it with another. Rankings compare minimum pay in dollars, not standards of living. Rents and prices differ widely between cities, and schools differ in many ways besides whether their graduate workers have a union contract.

**No warranty.** This page and its data are for general information only. They are not legal, financial or employment advice. The data is provided as is, without warranty of any kind. Where these figures differ from an official contract or policy, the official document takes priority.

**Corrections and suggestions.** We welcome corrections and ideas from readers. To report a mistake, or a newer contract or rate, email mail@academic-union-network.org. Please include the school, the figure and a link to the source. We will check the source and correct the data where needed. We would also like to hear which schools or contracts to add, which comparisons or features would help, and how to improve this page.

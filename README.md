# Logistics Dashboard for Carrier Volume, Freight Margin and Delivery Performance

A five page Power BI report that shows a European parcel and freight operation how much it ships, where to, what each carrier costs against what is charged, and how reliably each carrier delivers.

The operation ships with several carriers, to many countries, on several service levels. Management needs one view of where the volume goes, whether freight cost stays below freight charged, and whether shipments arrive within the promised days. Built for operations and logistics management and for carrier rate reviews.

A dashboard does not have to be the fanciest report in the company to be the most useful one. I keep the design simple and clean, with one navigation bar, the same four filters on every page, KPI cards on top and four visuals below. What matters is what the page holds, the numbers and findings management cares about, laid out so a manager can spot a problem, see where it sits and decide what to do next.

![Overview page](screenshots/1_overview.png)

## Key findings

2026 figures run from January to week 42.

- **Spend is concentrated.** FedEx EU (€11M) and DHL BeNeLux (€11M) carry 63% of 2026 freight charged.
- **One market dominates.** The Netherlands has 1.09M shipments over both years, more than three times Belgium (0.32M).
- **Growth is uneven.** Freight Pallets grew 45.4% and Bring Norway 18.8% against 2025. FedEx Non EU is the only decline at 9.4% fewer shipments.
- **FedEx and DHL earn a margin.** FedEx made €1,370,231 profit on €15,125,002 charged and DHL €778,781 on €11,442,702. About 90% of DHL profit comes from the Netherlands and Belgium.
- **DHL is faster.** 72.61% of DHL shipments arrive in 1 day and 91.5% of boxes are on time. At FedEx 23.15% take 4 days or more and 87.6% arrive on time, partly because FedEx also serves non EU destinations.
- **DPD cost data has a gap.** Weeks 22 to 26 show about €0.01M cost per week against €0.10M to €0.14M charged, and 26,550 shipments lack freight data. This points to a data completeness issue to check before reading DPD margin.

## The five pages

Every page has the same navigation bar on the left and the same four filters, Year, Month, Carrier group and Country. Below each screenshot I explain what the page answers and what I took from it.

### 1. Overview

![Overview](screenshots/1_overview.png)

*Shown for all years, carriers and countries.*

The overview answers the first questions management asks. How much do we ship, where does it go and with which carriers. Across 2025 and 2026 the operation sent 2.61M shipments and 5.33M boxes, with €74.4M in freight charged. FedEx EU and DHL BeNeLux move the most boxes in both years, and 2026 bars are lower only because the year runs to week 42.

The Netherlands alone takes 1.09M shipments, more than three times Belgium, and weekly volume holds steady at 45K to 75K boxes. The work is predictable and concentrated in one country and two carrier groups, which is where I would point carrier reviews and capacity planning first.

### 2. Carrier Comparison

![Carrier comparison](screenshots/2_carriers.png)

*Filtered to 2026.*

Freight charged in 2026 comes to €34.6M, and FedEx EU (31.8%) and DHL BeNeLux (31.3%) take almost two thirds of it, followed by DPD at 14.8%. Growth tells a different story. Freight Pallets grew 45.4% and Bring Norway 18.8% against 2025, both from a small base, while FedEx Non EU is the only carrier with fewer shipments, down 9.4%.

Pallets also carry 486 pieces per box against 30 to 105 for the parcel carriers, so they behave like a different product. For a rate review the FedEx EU and DHL contracts matter most, and pallet growth may need its own rates or capacity.

### 3. FedEx

![FedEx](screenshots/3_fedex.png)

*Filtered to 2026.*

FedEx is the largest carrier in 2026 with 456,705 shipments and €15.1M charged. Cost sits just below charged in almost every week and in every service type, which leaves €1.37M in freight profit, with Economy and Priority each bringing in about €6.2M to €6.5M.

Speed is the weaker side. Only 13.8% of shipments arrive in one day, 23.2% take four days or more, and 87.6% of boxes are on time. The matrix compares lead time with the promised days per country and month, for example Albania Economy at 4.4 days against 4 promised and 60% on time. That turns into a clear list of lanes to raise with FedEx, starting where delivery runs past the promise.

### 4. DPD

![DPD](screenshots/4_dpd.png)

*Filtered to 2026.*

DPD is where the dashboard caught a data problem. DPD charged €5.12M on 200,655 shipments in 2026, and in most weeks cost tracks charged closely. In weeks 22 to 26 cost drops to about €0.01M a week while charged stays at €0.10M to €0.14M, and 26,550 shipments have no freight data at all.

The cards do not reconcile either. Cost by service type adds up to €4.67M, below the €5.12M charged, yet the difference card shows a negative €214,680. The average cost per shipment of €26.81 only works out when divided by the 174,105 shipments that do have freight data. My conclusion was to hold any DPD margin reading until the cost records for those weeks are checked at the source.

### 5. DHL

![DHL](screenshots/5_dhl.png)

*Filtered to 2026.*

DHL is the fastest carrier in the report. 72.6% of its 399,870 shipments in 2026 arrive in one day and 91.5% of boxes are on time. Cost stays just below charged all year, which gives €778,781 in profit on €11.44M charged, mostly from Parcel Business and Parcel Home.

The country split shows where that profit comes from. The Netherlands (€514K) and Belgium (€187K) produce about 90% of it, and every other country adds little. Any decision to move volume between DHL and FedEx should start from this country view, not from the totals.

## Tools and skills shown

- **Power BI.** Five report pages, button navigation, consistent slicers, cards, charts and a drill down matrix.
- **DAX measures.** Totals, per box and per shipment averages, freight profit and difference, on time percentage and comparison with the previous year.
- **Report design.** Dark theme, one accent colour, a fixed colour per carrier and the same layout on every page.

## About the author

I am Adrian Vanderlinder, a business intelligence and operations professional with over 5 years of experience across logistics, operations, administration and reporting. I design Power BI reports and write the DAX behind them, with a focus on freight margin, lead times, on time delivery and data quality. I work with Power BI, Power Query, SQL, Excel and Python (pandas), and I have coordinated daily transport with carriers such as FedEx, DPD and DHL, so I know how the data looks from the operations side. Based in Rotterdam and fluent in English and Spanish.

Find me on [LinkedIn](https://linkedin.com/in/adrian-van-der-linder-59b1299b).

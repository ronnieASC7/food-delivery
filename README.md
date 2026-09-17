A Tableau analysis of a multi-market food delivery dataset, built to answer where revenue and profit actually come from: which cuisines and restaurant types perform best, how fulfillment method shapes revenue mix by market, and which markets and customer segments drive profitability.

Business questions
Which cuisine categories generate the most net revenue, and how far ahead are the leaders?
Which restaurant types are actually profitable, and which are losing money?
How does revenue split across delivery vs. pickup (fulfillment type) in each market?
Which markets are most profitable, and which customer segment drives that profit in each one?
Views
Cuisine Revenue

"Asian restaurants lead revenue, followed by Mediterranean; most cuisines fall well below the average"

A bar chart of total net revenue by cuisine category, sorted to make the revenue gap between the top cuisines and the rest of the pack immediately visible.

Restaurant Profitability

"Italian, Chinese, and sushi restaurants lead profitability, while burgers, desserts, and coffee & tea generate losses"

A diverging color-encoded bar chart of total profit by restaurant type, manually ordered from most to least profitable across 15 restaurant types. Color intensity is driven by profit itself, so loss-making categories stand out at a glance.

Revenue Mix by Market

A stacked bar chart of net revenue by market, colored by fulfillment type (e.g., delivery vs. pickup), with markets pinned in a fixed business-relevant order (Manhattan, Brooklyn, Long Island, Queens, Bronx, North Jersey). Shows both the absolute revenue scale of each market and its fulfillment mix.

Fulfillment Share

A companion view to Revenue Mix, using the same market-by-fulfillment-type breakdown but expressed as a percent-of-total (via a table calculation), so fulfillment mix can be compared across markets independent of their size.

Segment Profit by Market

"Brooklyn leads profit and Long Island trails; individual customers drive four of six markets"

A bar chart of total profit broken out by market and customer segment, sorted by profit within each market, showing which customer segment (e.g., individual vs. business/group accounts) is the primary profit driver in each market.

What this project demonstrates
Data connection & modeling: live connection to an Excel source (FoodDeliveryData table, 26 fields spanning orders, fulfillment, cost, and profitability)
Table calculations: percent-of-total calculations to compare mix across unevenly sized markets
Diverging color encoding: profit-driven color scales that surface losses, not just top performers
Business-defined sort order: markets and restaurant types ordered to match how the business actually reviews them, not just by value
Hierarchical breakdowns: nested market × customer-segment analysis to find the real profit driver within each market
Insight-driven titling: each view's title states the takeaway, not just the chart contents, so the finding lands before the viewer studies the data
Data

The underlying dataset (BAI501_Tableau_Food_Delivery_Data.xlsx) contains order-level food delivery records with fields for order and customer identifiers, customer segment, market/state, cuisine category, restaurant type/name, menu item, fulfillment type, order channel, membership tier, quantity, pricing, discounts, fees, revenue, restaurant payout, delivery distance/cost/time, platform cost, total cost, profit, and customer rating. It is coursework/practice data used for skill-building, not production business data.

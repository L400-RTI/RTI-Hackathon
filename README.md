# The Fabrikam Frenzy

Fabrikam is a global lifestyle brand that designs and manufactures outerwear and athleisure. They sell athleisure through their retail stores. As the monsoon intensifies , some celebrity athletes post surprise video wearing Fabrikam's apparel. Instantly, clickstream traffic explodes, add to carts spike, and store associates report low visibility into real-time operations during these rush hours.

At the same time:
	
 	• A tropical depression shifts course, threatening all delivery methods. Carriers update ETAs showing delays of orders.
	• A key fabric supplier reports a loom vibration anomaly; quality telemetry shows rising defect probability.
	• Management complains of no operational visibility.
	• Multiple defective apparel are shipped to customers, leading to returns and complaints.
	• Management also complains that lot of operational problems are solved reactively, not proactively.

Fabrikam needs real‑time intelligence to sense demand, protect availability, and fulfill promises—or they’ll face stockouts, cancellations, and reputational damage.
## Your mission (as hack teams): 
Fuse high‑velocity signals from manufacturing, clickstream, weather, and logistics to drive actionable insights that keep promises to customers—even as conditions change minute‑by‑minute.
## Why Fabric RTI? 
It gives you a single place for data in motion (Real‑Time Hub + Eventstream) plus analyze/visualize/act primitives (Eventhouse/KQL, Real‑Time Dashboards, and Activator) so teams can build end‑to‑end, from sensor to business outcome, on one SaaS platform.

## What “success” looks like (business KPIs to aim for)
	• Gather data from disparate sources and fuse them together to get a holistic view of operations.
	• Stop the shipping provider that is carrying the highest defect probability product. Stop the manufacturing process from producing the defected product.
	• Create an Operational dashboard that shows real-time status of operations.
 	• Pinpoint which apparel has highest demand using clickstream data.
	• Setup Fabrikam for future success by enabling Agents and AI Anomaly detection.

## The data you’ll have (live and simulated)
	• Manufacturing telemetry (per line/machine). This will be generated from the 'Manufacturing Simulator' notebook and will stream into a custom endpoint of the Eventstream you create.
	• Static data like assets, operators, sites. This will be generated from the 'Manufacturing Simulator' notebook and will be saved into the Lakehouse you create.
	• Shipment/Logistics: carrier, order, origin and destination details, and status updates etc. This will be generated from the 'Shipping Simualtor' notebook and will save the data into an Azure Storage Account.
	• E‑commerce clickstream: page views, website, device, status etc. This will be generated from the 'Clickstream Simulator' notebook and will be stream the data into a custom endpoint of the Eventstream you create
 	• Products data. This will be in an Azure SQL DB products table.
	• Weather: Temperature, Humidity, Wind Speed, Precipitation, etc. 
	
## Get started
[Act 1 : Gather data - from disparate sources and unify](https://github.com/L400-RTI/RTI-Hackaton/tree/main/Act%201%20-%20Gather%20data)

[Act 2 : Take control - of your business and save reputation](https://github.com/L400-RTI/RTI-Hackaton/tree/main/Act%202%20-%20Take%20control)

[Act 3 : Every click counts - to plan demand and growth](https://github.com/L400-RTI/RTI-Hackaton/tree/main/Act%203%20-%20Every%20click%20counts)

[Act 4 : Make Fabrikam future ready - using AI](https://github.com/L400-RTI/RTI-Hackaton/tree/main/Act%204%20-%20Make%20Fabrikam%20future%20ready)

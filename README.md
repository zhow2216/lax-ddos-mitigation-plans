# Los Angeles Anti DDoS Server: How Much Mitigation Do You Actually Need, What Do the Plans Cost, and Which SixtyNet LAX Tier Fits Your Traffic?

Los Angeles is the compromise most teams end up making: close enough to the US West Coast for single-digit-millisecond responses, close enough to Asia that a China-facing site still loads before visitors give up. If you are shopping for a los angeles anti ddos server, three numbers decide whether you overpay. The basis behind the mitigation figure, the price you pay after the introductory discount expires, and how long provisioning takes.

SixtyNet's current Los Angeles lineup starts at **$200 per year** for a 2-core box with 5TB of traffic and DDoS protection listed on the plan, and tops out at **$1,600 per year** for 8 cores, 16GB of RAM and 40TB. Every price on the plan page is an annual figure, and the higher struck-through number is the standard annual rate the discount is measured against. Below is what each tier includes, where the "DDoS protection" line stops being informative, and how the plans compare with dedicated-server alternatives in the same city.

> **Most readers should start with LAX-STARTER at $200/year.** Two cores, 2GB of RAM, 40GB of NVMe, a 2G network port and 5TB of traffic will carry a single storefront, a game lobby, a small API or a streaming relay. Move up only when traffic passes 5TB or you need more than two cores for concurrent connections. 👉 [See the current SixtyNet LAX plan prices](https://sixtynet.net/aff.php?aff=39)

## The full SixtyNet Los Angeles plan list

Four sizes carry the DDoS protection label. All of them are annual, all include NVMe storage rated at 12,500 to 25,000 IOPS, and none of them carry a stated mitigation capacity in Gbps.

| Plan | vCPU / RAM / NVMe | Network / traffic | Annual price | Order |
| --- | --- | --- | --- | --- |
| LAX-STARTER | 2 cores / 2GB / 40GB | 2G / 5TB | **$200/yr** (list $240) | [Order](https://sixtynet.net/aff.php?aff=39) |
| LAX-MICRO | 4 cores / 4GB / 80GB | 4G / 10TB | **$400/yr** (list $480) | [Order](https://sixtynet.net/aff.php?aff=39) |
| LAX-MEDIUM | 8 cores / 8GB / 160GB | 10G / 20TB | **$800/yr** (list $960) | [Order](https://sixtynet.net/aff.php?aff=39) |
| LAX-LARGE | 8 cores / 16GB / 320GB | 10G / 40TB | **$1,600/yr** (list $1,920) | [Order](https://sixtynet.net/aff.php?aff=39) |

The other Los Angeles lines on the same page solve a different problem, and the difference matters if you are serving mainland China:

| Line | What it is optimized for | Entry configuration | Price shown | Restriction |
| --- | --- | --- | --- | --- |
| China Unicom-Premium | AS9929 China Unicom route, free BGP session, 95th-percentile billing | 2 cores / 2GB / 40GB / 5TB | from **$2,500/yr** (list $3,000) | Residential IP, ports 80 and 443 closed |
| IRVINE-PRO | AS9929 China optimization, rejects all external probes by default | 2 cores / 2GB / 40GB / 5TB | from **$350/yr** (list $420) | Residential IP, 80/443 closed, refunds credited to account balance only |

Two things to read off that second table. The China-optimized routes sit on residential IPs that will not serve a public website on standard ports. The plans that will serve a public website are the LAX ones, and those are on SixtyNet's "Premium Network" rather than the AS9929 China route. As listed, you pick one or the other. If your visitors are mostly in mainland China and you need port 443 open, that is the first thing to raise with support before paying.

## What the phrase "DDoS Protection" on a spec sheet is worth

SixtyNet lists DDoS protection as a bullet and stops there. No Gbps figure, no statement about whether filtering is always inline or switched on when an attack is detected, no word on what happens when an attack exceeds whatever the limit is. That is common across this market, and it is where the money hides.

Take a provider that does publish numbers. One Varidata page says its Los Angeles anti-DDoS servers can reach global points of presence with "more than 5Tbps" of mitigation capacity. A different page on the same site says the facility holds "well over 2,000Gbps of traffic cleaning capacity" and, separately, that its standalone mitigation service filters more than 1Tbps. Three numbers, three different things: capacity you can be routed through, capacity owned inside that building, and capacity sold as its own product. StormWall's milestone of an 8Tbps global filtering network is a fourth kind, network-wide capacity shared across every customer.

None of those figures describes what a single IP can absorb. So when you ask SixtyNet what protection on LAX-STARTER is actually worth, ask in units you can compare: how many Gbps of clean traffic will they commit to absorbing for this IP, is the filter permanently in the path, and what is the escalation path at 101%.

There is a second reason to ask. Hostease, which sells Los Angeles servers with 100Gbps mitigation included from $99 a month, states plainly that mitigation helps preserve availability "but no protection service can guarantee uninterrupted performance during every attack." Any provider that promises otherwise is selling you something they cannot deliver. 👉 [Check what the LAX order page states about protection](https://sixtynet.net/aff.php?aff=39)

## The discount is real, and it is not the "first two months" kind

SixtyNet's 17% comes off the annual rate for the whole term. LAX-STARTER is $240 at list and $200 when you take the year, which works out to about **$16.70 a month**. That is a different mechanism from the promotional pricing common in this category: Varidata's Los Angeles anti-DDoS tiers at $65, $75, $105 and $150 a month carry a "First 2 Months 50% OFF" label, and the order links for those four tiers are tied to a promo code. Month three returns to list price.

Run the arithmetic on a headline monthly rate before comparing it with an annual one. A $65-a-month plan that halves the first two months costs about $715 in year one: $65 for the two discounted months, $650 for the remaining ten. The headline says $65; the invoice says $715. SixtyNet's $200 is $200. The two are not the same class of product, a VPS against a dedicated chassis, but the billing shape is the comparison worth making.

SixtyNet's page also mentions a quarterly option and a further discount for longer terms on the China Unicom line. Confirm in the cart which terms are live, since the plan table shows annual pricing only.

## Protection capacity and port bandwidth are two separate bills

The most expensive misunderstanding in this market is treating a mitigation figure as if it were your bandwidth. Hostease's entry server at $99 a month ships with 100Gbps of protection and a 100M port. The protection is larger than the pipe by three orders of magnitude because it describes how much attack traffic can be filtered, not how much legitimate traffic you can push.

Upgrades are priced separately and the steps are steep: 100Gbps to 200Gbps adds **$200 a month**, 200 to 500 adds **$350**, 500 to 1Tbps adds **$600**, and 1Tbps to 2Tbps adds **$1,000**, with final pricing depending on data center and contract length. A team that assumed protection scaled with the server ends up paying more for the filter than for the machine.

On SixtyNet's LAX plans, the network figure (2G, 4G, 10G) is the pipe and the traffic allowance (5TB to 40TB) is the monthly volume. Protection sits outside both. If you expect sustained attacks in the tens of Gbps, get the capacity commitment in writing before the annual payment clears.

## Provisioning, trials and refunds: what the page tells you and what it doesn't

Delivery speed varies enough between providers that it should be part of the decision when you are already under attack. Varidata states four-hour deployment, a replacement guarantee within two hours, IPMI access for reboots and reinstalls, and a two-day free trial. Hostease quotes 24 to 48 hours for standard servers and 3 to 5 business days for custom configurations. StormWall activates protection within 10 minutes, which is the relevant number if you are buying filtering rather than hardware.

SixtyNet's plan page does not state a provisioning window. A third-party write-up of the provider mentions a **3-day money-back window**, well short of the 30 days common elsewhere, and reports that credit card payments were suspended for fraud prevention, leaving the checkout to show which methods actually work. Treat both as items to verify on the order form rather than settled facts: the refund window is the one number that decides how much risk an annual prepayment carries. 👉 [Open the SixtyNet plan page and check the terms at checkout](https://sixtynet.net/aff.php?aff=39)

## Who should actually put an anti-DDoS box in Los Angeles

The city earns its place as the default for two audiences. The first is anyone serving the US West Coast plus Latin America, where a local scrubbing node shortens the path for clean traffic. StormWall opened a filtering point at Equinix LA1 in May 2026, its second full-scale node in the United States, and gave reduced latency for US and Latin American traffic as the reason. The second is anyone serving both the US and Asia. Varidata claims its CN2 route reaches the Chinese backbone within 160ms via China Telecom, China Unicom and China Mobile peering, a vendor figure rather than a measured one, and it explains why so much cross-border commerce lands in this city.

SixtyNet fits the first audience cleanly and the second audience with a caveat already noted: the protected plans are on the Premium Network, and the AS9929 China route lives on the residential-IP plans that cannot serve a website on ports 80 and 443.

If you need a dedicated chassis with a multi-terabit scrubbing commitment and a free trial, budget four to twenty times the SixtyNet annual price. If you need a Los Angeles box with filtering in front of it and you can live with VPS-grade resources, the annual plans are the cheaper route by a wide margin.

## FAQ

**Is 100Gbps of protection enough?**
For most small sites, yes by a wide margin: volumetric attacks that take a single storefront offline are usually far smaller than that. The number that decides whether you stay online is the provider's committed clean-traffic capacity for your IP, plus whether they null-route you the moment an attack crosses a threshold. Ask about the null-routing policy specifically.

**Does scrubbing add latency?**
Inline filtering adds a hop, so yes, some. Providers work to keep it small, and StormWall's stated rationale for a Los Angeles node was lower latency for regional legitimate traffic. When filtering is only switched on during an attack, you get a latency change at the worst possible moment. Ask which mode SixtyNet uses.

**Monthly or annual?**
SixtyNet's plan table shows annual terms, with the 17% discount applied to the annual rate. If a refund window of a few days applies, an annual prepayment is a bigger bet than a monthly one, so confirm the refund terms before committing to twelve months.

**What happens if an attack exceeds the plan's capacity?**
Ask before you buy. Typical answers are null routing, temporary filtering at a lower threshold, or an upsell to a larger mitigation tier. Hostease publishes that tier ladder openly, from +$200 to +$1,000 a month. SixtyNet does not publish one, which is exactly why the question is worth an email.

**Can I run a public website on the cheaper residential plans?**
No. The China Unicom-Premium and IRVINE-PRO lines close ports 80 and 443 for IP risk-control reasons. Public web hosting belongs on the LAX plans.

## Picking a tier

Work from traffic and cores, not from the protection label, since every LAX plan carries the same label and none of them quantifies it.

- One site, a game lobby or an API under 5TB a month: **LAX-STARTER at $200/year**, and put the savings toward a backup node.
- Four cores needed for concurrent connections, or traffic between 5TB and 10TB: **LAX-MICRO at $400/year**.
- Several services behind one box, a 10G port and 20TB: **LAX-MEDIUM at $800/year**.
- 40TB of traffic and 16GB of RAM: **LAX-LARGE at $1,600/year**, still less than three months of a mid-range dedicated anti-DDoS server elsewhere.
- Mainland China latency first and non-standard ports acceptable: the AS9929 lines, after confirming the port restriction does not break your application.

Two things to settle before you pay. First, what the protection on your chosen plan is quantified at, in Gbps, and whether it is always on. Second, the refund window and which payment methods are live at checkout, because both determine how much of that annual fee you can recover if the box does not perform.

👉 [Compare the SixtyNet Los Angeles plans and start with the tier that matches your traffic](https://sixtynet.net/aff.php?aff=39)

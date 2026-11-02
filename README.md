# unmanaged vps: what you're actually responsible for, what it really costs per year, and how to pick a plan without overpaying

An unmanaged VPS is a virtual private server where the hosting company keeps the machine running — hardware, network, power — and you handle everything above that: installing the OS, security patches, updates, backups, and your own software. That's the entire trade. You give up hand-holding and pay a fraction of what managed hosting costs. RackNerd's entry special, for example, is **$21.99/year** for a KVM VPS with 1 GB RAM, 20 GB SSD storage, and 3 TB of monthly transfer — less than what some managed hosts charge for a single month.

If you're comfortable in a terminal, that trade is usually a good one. If you're not, no discount makes unmanaged hosting a bargain, because a compromised or misconfigured server costs more to fix than you saved. This article walks through the responsibility split, the real numbers behind RackNerd's current plans, how it compares with Contabo, Hostwinds, and hosting.com, and the one policy detail (refunds) that most listicles skip.

> **Quick pick:** For most readers landing here, RackNerd's **1 GB KVM VPS Special at $21.99/year** (1 vCPU, 20 GB SSD, 3 TB transfer) covers static sites, small web apps, VPNs, and Linux practice — and the price renews at the same rate for as long as you keep the service. 👉 [Check the 1 GB Special's current price and locations](https://my.racknerd.com/aff.php?aff=11397&pid=952)

## What "unmanaged" actually puts on your plate

The dividing line is simple: the provider owns everything below the OS, you own everything above it. Hosting.com's own comparison table puts it plainly — unmanaged plans include full root access and your choice of OS, but OS updates, control panel updates, security patching, and monitoring are marked "You." Managed plans flip all of that to "We handle," and back it with a higher SLA (99.95%+ versus 99.9% for power/network on unmanaged).

On RackNerd's unmanaged KVM plans, the support boundary works the same way. Their 24/7 support team covers platform-level problems — the VPS won't boot, network issues, panel trouble. Installing and configuring your software stack is on you. What softens the deal is the **ctrl panel**: reboot and power cycling, OS reinstalls, an out-of-band HTML5 VNC console (useful when SSH is broken), root password resets, and a network firewall for inbound rules. A one-click app library handles the initial install of common stacks, and credentials show up directly in the panel after deployment.

One misconception worth killing early: unmanaged does not mean abandoned. It means the provider's job ends at keeping your machine alive and reachable. Everything you'd call a system administrator's work — hardening, updates, backups, troubleshooting your own app — stays yours.

## RackNerd's current VPS Specials: the full lineup

RackNerd currently lists five annual KVM VPS Specials. All of them include full root access, one IPv4 address, a 1Gbps port, SSD storage on RAID-10, and same-rate lifetime renewals.

| Plan | vCPU / RAM | Storage | Monthly transfer | Price | Order |
| --- | --- | --- | --- | --- | --- |
| 1 GB KVM | 1 / 1 GB | 20 GB SSD | 3 TB | **$21.99/year** | [Order the 1 GB plan](https://my.racknerd.com/aff.php?aff=11397&pid=952) |
| 2 GB KVM | 2 / 2 GB | 35 GB SSD | 5 TB | $35.99/year | [Order the 2 GB plan](https://my.racknerd.com/aff.php?aff=11397&pid=953) |
| 4 GB KVM | 3 / 4 GB | 60 GB SSD | 7 TB | $59.99/year | [Order the 4 GB plan](https://my.racknerd.com/aff.php?aff=11397&pid=954) |
| 6 GB KVM | 6 / 6 GB | 100 GB SSD | 12 TB | $89.99/year | [Order the 6 GB plan](https://my.racknerd.com/aff.php?aff=11397&pid=955) |
| 8 GB KVM | 7 / 8 GB | 150 GB SSD | 20 TB | $119.99/year | [Order the 8 GB plan](https://my.racknerd.com/aff.php?aff=11397&pid=956) |

Deployment is near-instant after payment, and you can choose among datacenter locations across the US, plus Toronto and Dublin, with an Asia-optimized Los Angeles node among the 20-plus total locations. Supported operating systems are CentOS, Rocky Linux, AlmaLinux, Fedora, Debian, and Ubuntu; custom ISO installs are available through a support ticket, and the VNC console lets you install from your own media if you prefer.

Separate from the Specials, RackNerd sells a line of monthly-billed standard KVM plans (1 GB at $17.99/month, scaling up to 12 GB), with the Los Angeles location offering Asia-optimized routing. Those matter mainly as a low-commitment trial option, which we'll get to in the refund section.

## The math most articles don't do: renewal price

Here's the detail that actually separates cheap VPS deals from marketing tricks: plenty of hosts advertise a low first-year price and then renew at 30–50% higher. RackNerd's Specials don't work that way. The official wording: *"These RackNerd VPS specials are lifetime recurring. You can renew at the same rate for as long as you decide to keep the service."*

So the three-year cost of the 1 GB plan is straightforward: $21.99 × 3 = **$65.97**, about **$1.83/month** throughout. There's no renewal cliff to model, which is why the sticker price is the real price.

For context, a comparable 1 GB instance from the major cloud providers runs roughly $5–6/month — call it $60–72 a *year* versus RackNerd's $21.99. The gap is the cost of management and the enterprise bells and whistles you're skipping.

One catch on capacity planning: RackNerd's one-click app catalog lists memory minimums that tell you where the entry plan stops making sense. n8n and Coolify need 2 GB to start; Ollama, AnythingLLM, and LibreChat want at least 4 GB; OpenClaw needs 8 GB. If your project involves running local AI models or a full self-hosted stack, the 1 GB plan will frustrate you — start at 4 GB ($59.99/year) instead. For WordPress, a small Minecraft server, monitoring tools, or a VPN, 1–2 GB is plenty.

👉 [Browse all five RackNerd Specials and current locations](https://bit.ly/RacKnerd)

## The refund policy: read this before paying annually

This is the section most unmanaged VPS roundups leave out, and it's the one that should shape how you buy.

RackNerd's terms state: *"Refunds are issued on a case-by-case basis since by default no refunds are provided once payment is received."* There is no money-back guarantee, no 7-day or 14-day window, and no prorated refunds. Account prepayments and wallet credit are explicitly non-refundable. A few more specifics worth knowing:

- **Cancellation is not a refund.** Canceling stops future billing; it doesn't return money you've already paid.
- **Immediate cancellation deletes everything within 24 hours.** If you click it by mistake, open a support ticket right away — after that window, data is gone permanently, and RackNerd states plainly it isn't responsible for data integrity under any circumstance.
- **Chargebacks carry a penalty.** Disputing a credit card charge triggers a $125–$250 administrative fee and possible account suspension, so "I'll just dispute it" is a genuinely bad plan here.
- **Renewal cancellation needs notice.** Submit written cancellation through the client area at least 5 days before the renewal date.

Refunds *are* realistically obtainable in narrow cases: a VPS that fails to provision properly in the first minutes, an unresponsive IP right after activation, or a dedicated server that misses the promised 72-hour delivery. Outside of genuine technical faults, expect the support team to offer alternatives — account credit, a different datacenter location, or an upgrade with the difference charged.

The practical playbook, given all this: test before you commit to a year. RackNerd publishes a Looking Glass and speed-test files for each datacenter location, so you can run ping, traceroute, MTR, and download tests from your own connection before ordering. And if you want a real trial on the service itself, the monthly-billed KVM line starts around $26.99/year for 512 MB or $17.99/month for 1 GB — enough to verify performance for a few weeks at minimal risk, then switch to the annual Special once you're satisfied.

With no safety net, it helps that the company isn't a fly-by-night operation. RackNerd has appeared on the Inc. 5000 list three years running (including #3693 in the 2026 national ranking), which is a reasonable data point on longevity for a budget host.

## How RackNerd compares with Contabo, Hostwinds, and hosting.com

"Unmanaged VPS" covers a wide price spectrum, so here's where RackNerd sits against the providers that dominate this search. Information only — check their sites directly if one of them fits better.

| Provider | Cheapest relevant plan | Specs | Port / network | Billing |
| --- | --- | --- | --- | --- |
| **RackNerd** | $21.99/year | 1 vCPU, 1 GB RAM, 20 GB SSD, 3 TB transfer | 1 Gbps | Annual, renews at same rate |
| **Contabo** | $5.28/month (first 24 months, then $6.60) | Cloud VPS 4: 4 vCPU, 8 GB RAM, 100 GB SSD | 200 Mbit/s | Monthly |
| **Hostwinds** | $16.99/month (unmanaged Windows) | 1 CPU, 1 GB RAM, 30 GB SSD, 1 TB transfer | 1 Gbps | Monthly |
| **hosting.com** | Unmanaged Linux VPS (quote-based pricing on site) | AMD EPYC, NVMe, 99.9% power/network SLA | Redundant uplinks | Monthly |

Reading the table honestly: Contabo gives you far more raw resources per dollar — its entry cloud VPS has 4× the RAM of RackNerd's cheapest — but the port speed is 200 Mbit/s versus RackNerd's 1 Gbps, its headline price is promotional for the first 24 months before rising to $6.60, and its unlimited-traffic policy comes with asterisked terms you should read. Contabo makes sense when you need big memory and storage and your traffic pattern tolerates the slower port.

Hostwinds' unmanaged line is Windows-focused and priced accordingly; its appeal is the surrounding platform — snapshots, custom ISOs, enterprise firewall, and a real-time monitoring system that opens tickets automatically. If you specifically need a Windows unmanaged VPS with polish, that's a legitimate choice, just at 8–9× the annual cost of RackNerd's entry Linux plan.

hosting.com plays in the managed-adjacent space: unmanaged plans there keep root access and NVMe hardware but wrap them in enterprise infrastructure and a formal SLA. Good for teams with compliance requirements; overkill price-wise for a hobby VPS.

RackNerd's niche is the opposite corner: minimum price, KVM isolation, full root, generous transfer, and a renewal price that never moves. What you don't get is NVMe storage, snapshots-as-a-service, or white-glove anything.

## Who should skip unmanaged hosting entirely

Being straight with you: some readers searching for unmanaged VPS plans would be better served elsewhere, and no configuration tip fixes that.

- **You've never used a Linux terminal.** Root access on your own box means you're also the one who gets to clean up after a compromised server. RackNerd's own shared hosting line (cPanel + LiteSpeed) exists precisely for this situation.
- **You want automated backups done for you.** On every unmanaged plan in this article, backups are your project. Managed plans at hosting.com and Hostwinds include daily backups; unmanaged plans treat them as optional add-ons or your cron job.
- **You need someone to call when your site breaks at 2 a.m.** Unmanaged support ends at infrastructure. If the failure is in your application or your OS config, the ticket response will politely remind you of that.
- **You need cPanel without thinking about licensing.** hosting.com sells cPanel-licensed managed plans; on an unmanaged box, the license is another thing you buy and maintain yourself.

If none of those describe you, unmanaged is simply cheaper infrastructure with the same hardware underneath.

## FAQ

**Is an unmanaged VPS hard to manage?**
It depends entirely on your experience. Installing Ubuntu on RackNerd takes a couple of clicks from the ctrl panel, and one-click apps cover common stacks. But patching, securing, and troubleshooting are genuinely on you. If "SSH into a server and edit a config file" sounds unfamiliar, start with managed hosting.

**Does RackNerd raise prices on renewal?**
No — the VPS Specials are officially lifetime recurring, renewing at the same rate indefinitely. That's their standout term compared with hosts that discount year one and mark up the renewal.

**Can I get a refund if I change my mind?**
By default, no. Refunds are case-by-case with a strong bias toward denial for used services or personal-change-of-mind cases. Genuine provisioning failures in the first minutes are your best shot. Test via Looking Glass and the monthly-billed plans before buying annually.

**What can I actually run on the 1 GB plan?**
Static sites, lightweight Nginx/PHP apps, WireGuard, a small database with careful tuning, monitoring agents. Don't plan on running a Node.js app plus a database plus a Java heap on 1 GB; the 4 GB plan ($59.99/year) is where full web stacks become comfortable.

**What payment methods does RackNerd accept?**
Credit card, PayPal, cryptocurrency, and Alipay, per third-party documentation of their checkout. One consideration: PayPal and credit cards give you external dispute mechanisms (though triggering a chargeback carries that $125–$250 fee), while crypto and Alipay leave you with support tickets only.

## Final word: matching plan to situation

The decision tree is short. Practicing Linux, running a VPN, or hosting a low-traffic site → the **$21.99/year 1 GB Special** and never think about it again. A WordPress install or small production app with real visitors → the **2 GB at $35.99/year**. A full stack with a database, media serving, or self-hosted AI tooling → start at **4 GB or 6 GB**; the one-click app memory minimums give you a floor. Streaming, transcoding, or heavy database work → the 8 GB with its 20 TB transfer is the value pick in the lineup.

Before clicking order, do two things: run the Looking Glass test from your location against the datacenter you plan to pick (latency you can't live with won't improve after purchase), and back up your expectations accordingly — annual payment on a host with a case-by-case refund policy means the test comes first, the commitment second. When you're ready, 👉 [the 2 GB Special's order page is here](https://my.racknerd.com/aff.php?aff=11397&pid=953) — it's the plan most small projects outgrow the 1 GB tier into, and at $35.99/year it stays cheaper than a single month of most managed alternatives.

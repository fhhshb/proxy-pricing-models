# Paid Proxies: How Per-IP and Per-GB Pricing Really Works, and How to Pick a Plan Without Burning Budget

If you're searching for paid proxies, there's a decent chance you already tried the free route. It worked for an afternoon, then half the list died, and the half that survived was slower than your own connection.

The useful question isn't whether paid proxies beat free ones. It's which billing model you're actually buying, because per-GB and per-IP plans reward completely different workloads. Get that wrong and you either overpay for traffic you never used or run out of IPs in the middle of a job.

This piece walks through how the pricing actually works, what a full plan list looks like at a budget residential provider (9Proxy, since that's the provider we're looking at here), and where the catches are.

## Per-GB or per-IP: the choice that decides your bill

Two billing models dominate paid proxies, and they aren't interchangeable.

**Per GB (bandwidth).** You buy a traffic allowance and route requests through a rotating pool. Every request burns data, and when the allowance is gone, it's gone. This suits workloads where each request is small: lightweight scraping, geo-checks, API polling, ad verification, SERP monitoring. You pay for exactly what you consume.

**Per IP.** You buy a fixed number of residential addresses, usually with unlimited bandwidth attached. The address count is the constraint, not the data. This suits long sessions, logins, account-based work, and anything where you genuinely can't predict how many gigabytes a job will move.

The sticker price tells you almost nothing until you know which camp your work falls into. Take a 50 GB/month residential scraping workload. A comparison published by Decodo puts that at roughly $40 at DataImpulse ($0.80/GB), about $100 at Decodo (from $2/GB), around $180 at SOAX (~$3.60/GB on its 25 GB plan), and about $125 at Oxylabs or Bright Data (from $2.50/GB).

That $40 figure looks like a 4x win until a fifth of your requests fail and get retried through a weaker pool. At that point the effective cost per *successful* response narrows fast. This is the part most price-comparison tables skip: cost per usable response, not cost per gigabyte, is the number that shows up on your invoice at the end of the month.

A few more things that quietly move the total:

- Image-heavy pages and browser-rendered traffic burn far more GB than plain HTML requests, because subresources count too.
- City, ZIP, and ISP-level targeting sometimes carries a premium over country-level.
- Monthly subscription plans give lower headline rates but punish idle months. Pay-as-you-go costs more per unit and nothing when you're not working.
- Minimum top-ups and expiring credits are the most common way a cheap rate becomes an expensive one.

## Why the free option keeps losing

Nobody needs a lecture on free proxies, but the failure modes are worth naming, because they explain why people end up paying.

A free proxy operator sits between you and everything you send. Credential interception, traffic logging, and injected ads are documented business models rather than hypotheticals. The IPs are shared with thousands of other users and were blacklisted by major targets long before you arrived, so success rates on protected sites drop into single digits. And free lists churn daily, which means any pipeline built on them breaks constantly, and the engineering time you spend re-plumbing it costs more than a paid plan would have.

The legitimate way to test the water is a trial allocation from a real provider, or the cheapest paid tier. That's the honest answer to "can I get this for free" — you can get a sample, not a service.

## Where 9Proxy sits in this market

9Proxy is a residential-only provider. There's no datacenter, ISP, or mobile product line, and no managed unblocker or scraping API, so it competes on price and targeting rather than on breadth of product.

What's consistently reported across independent directories and reviews is a pool of roughly 20 million residential IPs across 90+ countries, with targeting down to country, state, city, ZIP, and ISP level. You'll see bigger numbers floating around on promotional pages (some claim 95M+ IPs across 200+ countries) and smaller ones in stale directories; the 20M/90-country range is the figure that shows up most consistently in 2025–2026 write-ups. Treat all pool numbers, from any provider, as marketing until your own targets agree.

Protocol support is HTTP/HTTPS and SOCKS5, which means it drops into anti-detect browsers like AdsPower, Dolphin Anty, and ixBrowser with a host:port:user:pass string. Payments cover cards, Apple Pay, Google Pay, Alipay, and crypto via CoinPayments; crypto top-ups reportedly come with an automatic +5% IP bonus.

One bit of pricing history matters here. 9Proxy raised prices on its IP-based and bundle packages on June 1, 2026 — the first adjustment in the company's history, per its own announcement. GB-based pricing was explicitly left untouched. So any review quoting $0.20/IP for the 100-IP tier is working from pre-June figures, which is a good way to date an article you're reading.

## The full plan list

Everything below reflects the current published structure. 9Proxy doesn't operate on monthly subscriptions; it's a balance-based system, which is why the "validity" column matters more than the "billing period" column you'd expect from a SaaS pricing table.

### Residential proxies by IP (unlimited bandwidth per IP)

| Package | What you get | Price | Effective rate | Balance validity | Purchase |
| --- | --- | --- | --- | --- | --- |
| 100 IPs | 100 residential IPs, unlimited bandwidth | $24 | $0.24/IP | Unused IPs never expire | [Start with the 100 IP package](https://bit.ly/9-Proxy) |
| 500 IPs | 500 residential IPs, unlimited bandwidth | $72 | $0.144/IP | Unused IPs never expire | [Get the 500 IP package](https://bit.ly/9-Proxy) |
| 1,000 + 500 bonus IPs | 1,500 residential IPs, unlimited bandwidth | $126 | $0.084/IP | Unused IPs never expire | [Get the 1,500 IP package](https://bit.ly/9-Proxy) |
| 2,500 IPs | 2,500 residential IPs, unlimited bandwidth | $210 | $0.084/IP | Unused IPs never expire | [Get the 2,500 IP package](https://bit.ly/9-Proxy) |
| 5,000 IPs | 5,000 residential IPs, unlimited bandwidth | $360 | $0.072/IP | Unused IPs never expire | [Get the 5,000 IP package](https://bit.ly/9-Proxy) |
| 15,000 IPs | 15,000 residential IPs, unlimited bandwidth | $720 | $0.048/IP | Unused IPs never expire | [Get the 15,000 IP package](https://bit.ly/9-Proxy) |
| 25,000 IPs | 25,000 residential IPs, unlimited bandwidth | $863 | $0.035/IP | Unused IPs never expire | [Get the 25,000 IP package](https://bit.ly/9-Proxy) |
| 50,000 IPs | 50,000 residential IPs, unlimited bandwidth | $1,438 | $0.029/IP | Unused IPs never expire | [Get the 50,000 IP package](https://bit.ly/9-Proxy) |
| 100,000 IPs (Business) | High-volume tier, unlimited bandwidth | $2,300 | $0.023/IP | Unused IPs never expire | [Get the 100,000 IP package](https://bit.ly/9-Proxy) |
| 200,000 IPs (Business) | High-volume tier, unlimited bandwidth | $4,140 | $0.021/IP | Unused IPs never expire | [Get the 200,000 IP package](https://bit.ly/9-Proxy) |
| 500,000 IPs (Business) | High-volume tier, unlimited bandwidth | $8,625 | $0.018/IP | Unused IPs never expire | [Get the 500,000 IP package](https://bit.ly/9-Proxy) |

Two details on this table. IPs on this model stay live for anywhere from a few hours to around 24 hours rather than being permanently yours, and there's a Today List feature that lets you reuse an IP you already forwarded in the last 24 hours without spending a new one from your balance, as long as it's still online. If you're testing locations one by one, that second feature does real work.

### Residential proxies by GB (rotating pool, pay for traffic)

| Package | What you get | Price | Effective rate | Validity | Purchase |
| --- | --- | --- | --- | --- | --- |
| 5 GB | 5 GB of rotating residential traffic | $15 | $3.00/GB | 180 days | [Get the 5 GB package](https://bit.ly/9-Proxy) |
| 50 GB + 5 GB bonus | 55 GB of rotating residential traffic | $105 | $2.10/GB | 180 days | [Get the 55 GB package](https://bit.ly/9-Proxy) |
| 100 GB | 100 GB of rotating residential traffic | $150 | $1.50/GB | 180 days | [Get the 100 GB package](https://bit.ly/9-Proxy) |
| 200 GB | 200 GB of rotating residential traffic | $200 | $1.00/GB | 180 days | [Get the 200 GB package](https://bit.ly/9-Proxy) |
| 1,000 GB | 1,000 GB of rotating residential traffic | $800 | $0.80/GB | 180 days | [Get the 1,000 GB package](https://bit.ly/9-Proxy) |
| 2,000 GB | 2,000 GB of rotating residential traffic | $1,500 | $0.75/GB | 180 days | [Get the 2,000 GB package](https://bit.ly/9-Proxy) |
| 3,000 GB (Enterprise) | 3,000 GB, team features | $2,160 | $0.72/GB | No expiry | [Get the 3,000 GB Enterprise package](https://bit.ly/9-Proxy) |
| 6,000 GB (Enterprise) | 6,000 GB, team features | $4,200 | $0.70/GB | No expiry | [Get the 6,000 GB Enterprise package](https://bit.ly/9-Proxy) |
| 10,000 GB (Enterprise) | 10,000 GB, team features | $6,800 | $0.68/GB | No expiry | [Get the 10,000 GB Enterprise package](https://bit.ly/9-Proxy) |

The Enterprise tiers add a team mode (one owner plus up to five members), per-member traffic controls, activity logs, and bandwidth that doesn't expire inside the team. Outside shares still follow the 180-day rule.

### Bundle packages (IPs plus traffic in one purchase)

| Package | What you get | Price | Validity | Purchase |
| --- | --- | --- | --- | --- |
| Starter Bundle | 100 IPs + 5 GB | $30 | 180 days on the traffic portion | [Get the Starter Bundle](https://bit.ly/9-Proxy) |
| Popular Bundle | 1,500 IPs + 50 GB | $180 | 180 days on the traffic portion | [Get the Popular Bundle](https://bit.ly/9-Proxy) |
| Pro Bundle | 5,000 IPs + 500 GB | $720 | 180 days on the traffic portion | [Get the Pro Bundle](https://bit.ly/9-Proxy) |

Bundles make sense when a single project needs both stable identities and flexible rotation. If you only need one of the two, buying the individual package is cheaper — the Starter Bundle's 100 IPs alone list at $24, so you're effectively paying $6 for the 5 GB, which is well below the standalone 5 GB price of $15. On the larger tiers the maths moves the other way and you should check the numbers against your actual usage before assuming the bundle wins.

## Which tier actually fits your job

Reading a plan list is easier once you map it to a task.

**Light testing and geo-checks.** The 5 GB tier at $15. Low commitment, 180 days to use it, and rotation is handled for you. If you're checking how a page renders from three countries, this is the sane entry point.

**Ongoing scraping on a handful of targets.** The 55 GB tier at $2.10/GB, which 9Proxy markets as its most popular GB plan, or 100 GB at $1.50/GB if the volume is there. Both give you rotation without counting addresses.

**Multi-account work and long sessions.** This is where per-IP wins. You want the same address to persist across a sequence of requests, and you don't want a traffic meter running while you do it. 500 IPs at $72 is the realistic starting point for a solo operator running a few dozen profiles.

**Unpredictable or bandwidth-heavy pipelines.** Per-IP again, for a different reason: unlimited bandwidth per active IP means a job that suddenly pulls video or large datasets doesn't blow through a GB allowance. 1,500 IPs at $126 is the sweet spot for a small team working across verticals.

**Agency and reseller volume.** 15,000 IPs at $720, or 25,000 at $863, is where the per-IP rate falls under five cents. Past 100,000 IPs you're into Business pricing at $0.023/IP and below, which is a different conversation.

## How you actually connect

9Proxy spreads access across four routes, and which one you pick depends on how much control you want.

- **Proxy Program** — a Windows client that routes traffic at the OS level, so applications without native proxy support still work. Required for IP-based plans.
- **Proxy2Web** — browser-based access with standard username/password authentication. No install, which matters if you're on a managed machine or a tablet.
- **ProxyHub** — mobile device management. ProxyHub Lite runs per device; ProxyHub Pro gives centralized control for assigning proxies remotely.
- **Public API** — programmatic proxy generation, rotation, balance checks, and sub-user management, documented at the provider's docs site.

Authentication is either username/password (with targeting baked into the username string, e.g. `user-country-US-ssid-xxxx`) or IP whitelisting. If you're wiring this into a Python pipeline or a proxychains setup, SOCKS5 works natively without protocol conversion.

One limitation worth knowing: iOS devices only accept HTTP proxies over Wi-Fi. HTTPS and SOCKS5 aren't supported there, and proxies won't work over cellular at all.

## Vendor numbers versus what reviewers measured

9Proxy publishes roughly a 99.5% success rate, about 0.6s average response time, and 99.95% uptime. Those are vendor figures — read them as marketing claims, not SLAs.

Third-party positions vary. ProxyLook's directory puts available benchmark data at around 97% success with P95 latency of 1.3s on residential rotating traffic, and notes reviewers reporting high success against Cloudflare-protected targets with latency in the 0.8–1.4s range on US IPs. Either way, the honest takeaway is that

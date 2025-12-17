# FanDuel Sportsbook Promotion Impact Case Study:

## How to run
1) Create a virtual environment:
```bash
python -m venv .venv
source .venv/bin/activate   # mac/linux
# .venv\Scripts\activate    # windows
pip install -r requirements.txt

FanDuel Sportsbook Promotion Impact Analysis - Summary

This analysis focuses on evaluating the effectiveness of a sportsbook promotion using an A/B-style matched-control design to isolate incremental impact rather than raw post-promo totals. Concretely, each target customer was paired with a similar control customer using pre-period behavior (nearest-neighbor matching and stratification by baseline activity/value tier). For every player, the change in platform revenue or GGR (Gross Gaming Revenue) was measured from before-to-after promotion application and those changes were compared between Target and Control; this “difference-in-differences” (DiD) readout gives the lift attributable to the promo. Then, NGR (Net Gaming Revenue) per player (GGR minus one-time promotion bonus) & ROI (incremental GGR relative to bonus allocation cost) was computed, and uncertainty was quantified via 95% confidence intervals. To ensure conclusions were technically and logically robust, sensitivity checks were implemented on analysis windows (symmetric pre/post-promo), and readouts were repeated under alternative outlier treatments and data filters (e.g., zero-activity days vs. active-day normalization).

The results showed that not all customer value tiers responded equally. High & Low tiers delivered positive GGR per bonus dollar and therefore generated larger ROI, while Medium & VIP tiers produced negative returns suggesting that the incentive either: 1) cannibalized existing play or 2) failed to motivate additional betting. Based on these findings, I recommended reallocating bonus budget toward High & Low tiers, while pausing or reducing bonus spend in Medium & VIP tiers until incentives are structurally redesigned.

For those weaker or lower performing tiers, it was recommended that FanDuel's Sportsbook Team start by testing smaller bonus budget denominations, capping odds boosts/missions (non-cash constructs that limit downside), and specifically targeting customers with recent activity/play propensity. In addition, it was recommended to add stop-loss guardrails (i.e., throttle/stop promotion if Target underperforms Control by >X% for Y hours), and continuously track NGR per player as well as player retention alongside GGR. Finally, adopting a disciplined testing plan with a holdout sample where you could run denomination ladders by tier (e.g., Low: $3 vs $5; High: $15 vs $20, etc.) would be extremely beneficial to investigate.

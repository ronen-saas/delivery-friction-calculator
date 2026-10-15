# Friction Point Savings Calculator

A free, self-contained calculator that estimates the annual savings from fixing friction points in B2B SaaS and Fintech client onboarding and implementation delivery.

Pick up to three friction points, add a few numbers, and get a ballpark annual saving in pounds. No sign-up, no dependencies, no AI at runtime.

Built by [Enwise Insights & Advisory](https://enwiseinsight.com), a London-based practice helping B2B Fintech and SaaS companies scale professional services without scaling costs at the same rate.

**Live demo:** [ronen-saas.github.io/delivery-friction-calculator](https://ronen-saas.github.io/delivery-friction-calculator/)

**On the Enwise website:** [enwiseinsight.com/roi-calculator/](https://enwiseinsight.com/roi-calculator/)

## Why this exists

Deals are closing, but onboarding is slow, implementation teams are stretched and costs are rising. Delivery cost is usually treated as a capacity problem, when it is often a symptom of deeper causes: bespoke implementations, inconsistent processes, knowledge silos and unclear client expectations.

Those costs are rarely measured. This calculator makes them visible, so the conversation about fixing them starts from numbers instead of gut feel.

## How it works

1. **Pick up to 3 friction points** from nine, across the delivery journey (handover, scoping, planning, delivery, ongoing), for example reducing re-scoping after handover, standardising SOW effort estimates, or cutting manual admin and reporting.
2. **Add detail** for each: hours per project spent on that activity, and a realistic improvement (a typical low, medium or high range).
3. **Add your context**: average day rate and number of projects per year.
4. **See the number**: annual savings per friction point and in total.

The maths is deliberately simple: `hours per project × improvement % × hourly rate × projects per year`, where hourly rate is day rate divided by 8. The percentages are illustrative ranges based on patterns seen in B2B SaaS delivery, not guarantees. Sense-check them against your own experience.

## Usage

It is a single HTML file with inline CSS and JavaScript.

- **Try it locally:** open `index.html` in a browser.
- **Embed it in WordPress or Elementor:** paste everything between the `START` and `END` comments in `index.html` into a Custom HTML block.
- **Customise it:** edit the `frictionPoints` array in the script to change the friction points, descriptions and improvement ranges.

### Privacy and optional logging

Out of the box, everything runs in the browser and nothing is stored or sent. If you want to log anonymous calculations to your own Google Sheet, set `WEBHOOK_URL` (and optionally `SHARED_SECRET`) to your own Google Apps Script Web App. Leave `WEBHOOK_URL` empty to disable logging.

## Who it is for

- CEOs, COOs and CCOs at growing B2B SaaS and Fintech companies
- Heads of Professional Services, Delivery, Implementation and Customer Success
- Advisors and fractional leaders who need a quick way to frame the business case for change

## Related work from Enwise

- **Beyond the Signals**: a 2-day check of whether your PS function can scale before sales take off
- **Beyond the Symptoms**: a 4-day diagnostic that finds the root causes of delivery pain
- **Fractional PS Director**: embedded senior delivery leadership

More at [enwiseinsight.com](https://enwiseinsight.com) or ronen@enwiseinsight.com.

## Licence

MIT. See [LICENSE](LICENSE).

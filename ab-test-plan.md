# Flow State Yoga — A/B Test Plan
**MKTG:4400 Digital Marketing | November 8, 2026**

## Page and single change
I will test the main call-to-action (CTA) button in the hero section of the Flow State Yoga homepage (`https://mallorykron.github.io/flow-state-yoga/`). Version A is the current homepage, with the button text **“Explore Our Classes ↗”**. Version B will be an otherwise identical copy with only that hero button text changed to **“Find Your Yoga Class ↗”**. Both buttons will continue linking to `classes.html`. No other copy, design, images, or links will change. I will publish Version B at a separate URL, add a `noindex` meta tag, and leave it out of the sitemap so it does not compete with the original page in search.

## Hypothesis and reasoning
I predict that Version B will produce a higher proportion of AI visitors saying they would click the hero button to view yoga classes. “Find Your Yoga Class” directly describes the next step and makes the choice feel personal, while “Explore Our Classes” is broader. This prediction could be wrong: the original wording might feel more inviting and less demanding.

## AI visitors, prompt, and random assignment
I will use **GPT-6 (same available model/version and settings for every trial)**, with each trial in a new conversation without earlier trial context. The persona is a college student or young professional in Iowa City who is interested in trying yoga. I will show the full homepage text for the assigned version in the same format each time, changing only the hero CTA wording. I will generate and save a randomized list of 100 assignments in advance, with exactly 50 A and 50 B trials, then run them in that order.

**Exact prompt template** (replace `[PAGE TEXT]` with the assigned version's complete page text; everything else remains identical):

> You are a college student or young professional in Iowa City who is interested in trying yoga. You are looking at the homepage of a fictional local yoga studio. Read the page below as a potential customer. Based only on what you see, would you click the main button in the top hero section to view the available yoga classes? Answer exactly YES or NO, followed by one sentence explaining your choice. Do not assume any information that is not on the page.
>
> [PAGE TEXT]

## Outcome, sample size, and analysis
The **one primary outcome** is whether the AI visitor answers **YES** to clicking the main hero button (YES = 1, NO = 0). I will record the trial number, assigned version, model/version, date, exact response, and coded outcome for every trial. I will complete **100 trials total (50 per version)** before analyzing the results, aiming to finish by **November 24, 2026**. I will not stop early or discard inconvenient answers.

I will compare the percentage of YES responses for Version B versus Version A, calculate the percentage-point difference, and use a two-sided Fisher's exact test at a 0.05 significance level. My hypothesis will be supported if Version B has a higher YES rate than Version A; I will call the difference statistically significant only if p < 0.05. A non-significant result will be reported as inconclusive, not proof that the versions are identical. Because AI responses are simulated intentions rather than real clicks, the findings will not establish actual customer behavior.

# Top YouTube Creator Production & Growth Systems (MrBeast, Paddy Galloway, other consistently viral channels)

> **Method note for the report writer (read first).** This pass ran under severe access limits:
> Tavily returned "plan usage limit exceeded"; the session-wide WebSearch budget (200 calls per turn, shared by all agents) ran out after 6 searches by this researcher; direct page fetches (WebFetch and curl) were blocked by the session network policy for werd.io, colinandsamir.com, podcast.creatorscience.com and thetranscriptdesk.substack.com, and the proxy also logged blocks for other agents on reddit.com, archive.org, blog.youtube and support.google.com; GitHub reads outside the project repo were denied.
> As a result, **almost every finding below comes from search-engine result summaries or from GitHub code-search text fragments, not from full reads of the cited pages.** The GitHub fragments are verbatim snippets of reposted copies of the MrBeast document.
> I attribute each claim to a URL as precisely as the search output allowed. Treat summary paraphrases as paraphrases, not quotes.
> Most of Key Questions 3–6 is unanswered. Each Gaps section lists what is missing, plus leads marked **[UNVERIFIED]** that come from background knowledge, so a follow-up pass can check them. Do not state UNVERIFIED items as fact.

## 1. MrBeast — the leaked "How to Succeed in MrBeast Production" document and Jimmy Donaldson's own statements

### Takeaway
The leaked 36-page onboarding PDF (public in mid-September 2024) sets out a YouTube-native production system:
- One goal: "the best YOUTUBE videos possible", not the best-produced videos.
- Three metrics define success: CTR, AVD and AVP.
- The first minute is engineered hardest, and retention is structured minute by minute.
- An unmeasurable "wow factor" is what separates the channel from others.
- Must-have elements get ruthless priority, consultants are "cheat codes", and staff are told that "no does not mean no", within an A/B/C-player culture.

Jimmy's 2023–2025 public statements add two things: industrial-scale thumbnail testing (titles and thumbnails settled before shooting, many variants, A/B tests) and a deliberate shift toward story and character to lift retention.

### Cited Findings
**Provenance, authenticity and reception**
- Coverage describes it as a 36-page PDF called "How to Succeed in MrBeast Production", an onboarding document for new members of the MrBeast production team. How and when it leaked is unclear; one source says it was first leaked to YouTuber Rosanna Pansino in August 2024. It covers "the technical weeds of YouTube production" plus expectations for employees, including an A/B/C-player hierarchy. — [Sherwood News](https://www.sherwood.news/culture/mrbeast-youtube-leaked-internal-success-document); [werd.io repost](https://werd.io/how-to-succeed-in-mrbeast-production-leaked-pdf/); [Gigazine, 17 Sep 2024](https://gigazine.net/gsc_news/en/20240917-mrbeast-youtube-production). These come from a search summary, so individual sub-claims cannot be tied to one of these pages.
- Simon Willison's post of 15 Sep 2024 is the most-cited public link to the PDF — [Simon Willison](https://simonwillison.net/2024/Sep/15/how-to-succeed-in-mrbeast-production/). The Hacker News thread had 2,115 points and 1,352 comments when a GitHub note captured it — [HN thread](https://news.ycombinator.com/item?id=41549649); [ahastudio/til note](https://github.com/ahastudio/til/blob/aadc20564a89c62f9eefab445fc01bb0d2e89fdf/management/mrbeast-production.md).
- The TLDR newsletter (16 Sep 2024) described it as written by MrBeast and "aimed at helping his employees get up to speed on the channels' learnings over the past decade" — [TLDR archive (GitHub)](https://github.com/GaloisField2718/tldr_news/blob/a140d2629382cf778e50b06e7be968e66f13d750/TLDR/article_16-09-2024.md).
- Reactions split. Some critics called it evidence of "toxic, unfair, and even dangerous workplace practices"; people in tech circles saw "a rare glimpse at the strategies and tactics employed by a top performer". — [werd.io](https://werd.io/how-to-succeed-in-mrbeast-production-leaked-pdf/); [Sherwood News](https://www.sherwood.news/culture/mrbeast-youtube-leaked-internal-success-document) (search summary)
- Secondary outlets describe it as "leaked" or say it "allegedly" reveals MrBeast's methods; no official confirmation was found — [Creator Handbook](https://www.creatorhandbook.net/leaked-document-allegedly-reveals-mrbeasts-secrets-to-youtube-success-the-key-takeaways/).
- Copies and full-text reposts:
  - [PDF on a Webflow CDN](https://cdn.prod.website-files.com/6623b7720b009050313e701c/66ede69453b7bbadcd2f05a8_How-To-Succeed-At-MrBeast-Production%20(2).pdf)
  - [PDF at read.jamesst.one](https://read.jamesst.one/1726688811.pdf)
  - [Alexander Jarvis full-text repost](https://www.alexanderjarvis.com/memo-how-to-succeed-in-mrbeast-production/)
  - [Daniel Scrivner summary, "Inside MrBeast's $100 Million Content Machine"](https://www.danielscrivner.com/how-to-succeed-in-mrbeast-production-summary/)
  - [OMR (German)](https://omr.com/de/daily/mrbeast-doc-pdf-leak)

**Stated goal (verbatim)**
- "Your goal here is to make the best YOUTUBE videos possible. That's the number one goal of this production company. It's not to make the best produced videos. Not to make the funniest videos. Not to make the best looking videos. Not the highest quality videos.. It's to make the best YOUTUBE videos possible." — [repost of the document text (GitHub)](https://github.com/echore/blog/blob/efb053927828e5894e5d2935178cf56c839979f5/content/Main/Mrbeast%20production.md); paraphrased as the core principle in the [Koi summary](https://www.koi.app/posts/mrbeast-s-blueprint-for-youtube-domination-key-insights-from-the-leaked-employee-guide)
- Anti-Hollywood framing: a Marketing4eCommerce headline quotes the memo as "This is not Hollywood and I do not want to be Hollywood". The wording may be translated. — [Marketing4eCommerce](https://marketing4ecommerce.net/en/tips-for-youtube-by-mrbeast/). A blog summary says the document "explicitly rejects the Hollywood model, believing that YouTube's future is brighter and demands a different approach" — [jyzblog (GitHub)](https://github.com/jyzblog/jyzblog.github.io/blob/88a14c341f39cc3254957eb7139d53426577a455/blog/posts/2024-09-19.md).

**The three metrics: CTR, AVD and AVP**
- Verbatim: "The three metrics you guys need to care about is Click Thru Rate (CTR), Average View Duration (AVD), and Average View Percentage (AVP). Make sure you know those abbreviations because that's how most people will refer to them" — [repost of the document text (GitHub)](https://github.com/echore/blog/blob/efb053927828e5894e5d2935178cf56c839979f5/content/Main/Mrbeast%20production.md)
- CTR is described as the share of people who click after seeing the thumbnail — [Alexander Jarvis repost](https://www.alexanderjarvis.com/memo-how-to-succeed-in-mrbeast-production/) (search summary)
- AVP is tied to how well a video holds attention — [ProTunesOne](https://protunesone.com/blog/leaked-mrbeast-document-on-his-youtube-strategies/) (search summary)
- A summary says CTR is driven by thumbnails and titles "that create high expectations", which the video must then meet — [jyzblog (GitHub)](https://github.com/jyzblog/jyzblog.github.io/blob/88a14c341f39cc3254957eb7139d53426577a455/blog/posts/2024-09-19.md)
- Other summaries: [Medium](https://medium.com/@art02623i/mrbeast-production-doc-key-themes-and-insights-be95b024e63b); [Popsters](https://popsters.com/blog/post/secrets-of-success-in-vlogging-a-guide-from-mrbeast); [IndieHackers](https://www.indiehackers.com/post/creators/mrbeasts-leaked-company-doc-is-required-reading-for-content-creators-He40uWgzqPqiZZEYhLp2)

**The first minute and the minute-by-minute structure**
- The memo treats the first minute as the most important part of the video because that is where the most viewers are lost, so the team puts the most effort into it — [WebSeitz wiki notes on the memo, 15 Sep 2024](http://webseitz.fluxent.com/wiki/2024-09-15-LeakedMrBeastMemoOnProduction) (search summary)
- Minutes 1–3 are for moving "from hype to execution". Minutes 3–6 are for the most exciting content. — [Alexander Jarvis repost](https://www.alexanderjarvis.com/memo-how-to-succeed-in-mrbeast-production/) (search-summary paraphrase)

**"Wow factor"**
- The memo calls the wow factor the most subjective metric and describes it as doing something no other creator can do — [WebSeitz wiki](http://webseitz.fluxent.com/wiki/2024-09-15-LeakedMrBeastMemoOnProduction) (search summary)
- It is presented as a qualitative measure that cannot be tracked, alongside the three numeric metrics — [Energy Crystals newsletter](https://www.energycrystals.io/p/what-the-mr-beast-memo-can-teach) (search summary)

**Prioritising must-have elements (associated with "critical components")**
- The memo sets out a priority list whose first item is buying a Lamborghini for under $200k. It says that anything pulling an employee away from that task is the employee's fault. — [Alexander Jarvis repost](https://www.alexanderjarvis.com/memo-how-to-succeed-in-mrbeast-production/) (search-summary paraphrase). The search summary could not confirm the exact phrase "critical components"; see Gaps.

**"No does not mean no"**
- When dealing with outsiders, staff should not accept a refusal at face value. They should go around the first person who refused, to other employees or managers, and not stop until every conceivable option is exhausted. — [Alexander Jarvis repost](https://www.alexanderjarvis.com/memo-how-to-succeed-in-mrbeast-production/) (search-summary paraphrase)
- Critics including Rosanna Pansino cited the line as evidence of an authoritarian culture. Tubefilter notes that the memo also tells staff never to do anything that could make the company look bad from a PR perspective, and that the author was not applying the phrase to sexual politics. — [Tubefilter, 17 Sep 2024](https://www.tubefilter.com/2024/09/17/mrbeast-internal-production-guide-leaked-key-points/) (search summary)

**Consultants**
- A section titled "Use Consultants" calls consultants "cheat codes" and tells staff to check whether a consultant exists before starting any task they are assigned — [PDF copy](https://cdn.prod.website-files.com/6623b7720b009050313e701c/66ede69453b7bbadcd2f05a8_How-To-Succeed-At-MrBeast-Production%20(2).pdf) (search summary)

**People system**
- The memo sets an A/B/C-player hierarchy for staff — [Sherwood News](https://www.sherwood.news/culture/mrbeast-youtube-leaked-internal-success-document); [werd.io](https://werd.io/how-to-succeed-in-mrbeast-production-leaked-pdf/) (search summary)

**Jimmy Donaldson and his team, on the record (2022–2025)**
- **Thumbnail process.** In a YouTube-produced interview with MrBeast's thumbnail lead:
  - The team settles titles and thumbnails before shooting.
  - The lead pointed to YouTube's thumbnail A/B testing option as a way to try ideas.
  - A/B tests favoured closed-mouth images: the closed-mouth version led to higher watch time in all 30 videos tested, though by a small margin.
  - MrBeast separately posted that people "hate open mouth".
  - Source: [Social Media Today](https://www.socialmediatoday.com/news/youtube-shares-insights-mrbeasts-team-creates-compelling-thumbnail/709817/); the publication date was not shown in the search output.
- **Thumbnail spend.** Reported second-hand: about $10,000 per thumbnail, and up to 20 thumbnail variations per upload — [Social Media Today](https://www.socialmediatoday.com/news/youtube-shares-insights-mrbeasts-team-creates-compelling-thumbnail/709817/); [Nouns News](https://nouns-news.beehiiv.com/p/mrbeast). The original source of these numbers was not identified.
- **Story over pace.** MrBeast publicly argued for YouTube videos to focus "more on story", meaning better storytelling and character development, especially in unscripted shows. He said retention on newer videos where he tested this is much higher than on videos made with his old methods. Some viewers responded that "this one was boring". — [MEAWW](https://meaww.com/mr-beast-advocates-for-you-tube-videos-to-focus-more-on-story-internet-says-this-one-was-boring) (date not shown; probably 2024–25; entertainment outlet of moderate reliability)
- **Long-form interviews.** These exist but their content was not retrieved this session:
  - Lex Fridman Podcast #351, "MrBeast: Future of YouTube, Twitter, TikTok, and Instagram" (January 2023) — [Recall summary page](https://www.recall.it/summary/content-creation/mrbeast-future-of-youtube-twitter-tiktok-and-instagram-or-lex-fridman-podcast-351)
  - 2022 Rolling Stone cover profile, which Simon Willison links in his post — [Rolling Stone](https://www.rollingstone.com/culture/culture-features/mrbeast-youtube-cover-story-interview-1334604/); [link captured in linksfordevs (GitHub)](https://github.com/Buildstarted/linksfordevs/blob/fce0101cff17ef6100016e446fbb3b15eb0de0a2/2024/09/15/index.html)
- **Low-quality source, for completeness.** An AI-generated video summary claims MrBeast stresses setting the right expectation in the first 5 seconds — [Chaindesk AI summary](https://chaindesk.ai/ru/tools/youtube-summarizer/how-mr-beast-achieved-70-retention-k1pFu5VbAN4)

### Inferences
- The memo is a funnel:
  1. Packaging earns the click (CTR).
  2. The first minute pays off the promise made by the thumbnail and title, which minimises the steepest early drop-off (AVD).
  3. Planned escalation (hype, then execution, then the best material in minutes 3–6) sustains AVP.
  4. The wow factor creates a distinctiveness that the metrics cannot capture.

  This funnel works without MrBeast's budget.
- "Critical components", consultants and "no does not mean no" together form a production-risk system, not creative advice: identify single points of failure, hand them to an owner, bring in expertise, and persist on logistics. For a small creator this becomes a one-page pre-production risk list with owners and deadlines.
- The thumbnail evidence (30 tests, a small consistent margin) suggests the team compounds many marginal, data-validated gains rather than relying on intuition.
- The "more story" push in 2024–25 shows that even this system changes its style when retention or novelty decays. Treat the leaked memo as a September 2024 snapshot, not a fixed formula.
- Caution for replicators: the culture sections drew labour-practice criticism. Copy the persistence on logistics and suppliers, not the pressure on people.

### Gaps
- **Exact memo wording not retrieved.** The full PDF and reposts could not be read, so I could not verify the exact text of:
  - the "critical components" definition and its examples;
  - the full minute-by-minute section (re-engagement points, minute 6 to the end, the ending);
  - the A/B/C-player definitions;
  - the communication and check-in rules;
  - the ideation and creative process;
  - any internal numbers.
- **[UNVERIFIED] leads on the memo.** From background knowledge: the memo's A-player definition includes being obsessive, coachable, not making excuses and believing in YouTube; it describes a "crazy progression" early in videos and a re-engagement beat around minute 3. Check against the [PDF](https://cdn.prod.website-files.com/6623b7720b009050313e701c/66ede69453b7bbadcd2f05a8_How-To-Succeed-At-MrBeast-Production%20(2).pdf) or the [Tubefilter key points](https://www.tubefilter.com/2024/09/17/mrbeast-internal-production-guide-leaked-key-points/) before use.
- **Interview claims without sources.** None retrieved for Jimmy's statements on how many years he spent studying retention, his upload cadence, or how many ideas or videos get killed, scrapped or reshot. **[UNVERIFIED]** He is widely quoted as having spent about five years obsessively studying YouTube virality with a small group of friends, and Joe Rogan Experience #1788 (2022) is often cited for this.
- **[UNVERIFIED] interview pointers to check.** "Colin & Samir — Unfiltered Conversation with MrBeast" (date unknown, possibly before 2022); a possible early-2025 Diary of a CEO appearance; ViewStats, MrBeast's analytics and outlier tool.

## 2. Paddy Galloway — documented frameworks, case studies and public breakdowns

### Takeaway
As far as the evidence here shows, Paddy Galloway's method has four parts:
- **Packaging first.** He treats YouTube as a "click-and-watch" platform where the title and thumbnail are reportedly about 50% of success.
- **Outlier analysis.** Study videos that performed roughly 5–15x a channel's baseline and copy what drove them.
- **The CCN test.** An idea should appeal to Core, Casual and New viewers at once.
- **Heavy idea filtering.** Hundreds of concepts are cut down to a few.

He argues that any niche can reach viral scale. His own channel shows extreme selectivity: reportedly about 33 videos in a decade averaging about 1M views. Much of this evidence comes from podcast summaries and a tool vendor's blog, so treat the numbers as approximate.

### Cited Findings
- His second appearance on Jay Clouse's Creator Science podcast (judging by the URL slug) is titled "Paddy Galloway is the world's most sought-after YouTube strategist" — [Creator Science](https://podcast.creatorscience.com/paddy-galloway-2/)
- His "New Rules of YouTube" (2025) is published as a Colin and Samir resource, and an edited transcript exists on Substack. Only titles and snippets were seen. — [Colin and Samir](https://www.colinandsamir.com/resources/the-new-rules-of-youtube-from-paddy-galloway); [The Transcript Desk](https://thetranscriptdesk.substack.com/p/the-new-rules-of-youtube-2025-edited)
- **Outlier analysis.** Ignore average videos and find the anomalies performing about 5x–15x above a channel's baseline. Isolate what drove them (topic, title, thumbnail, format, timing) and build new videos on those variables. — [OutlierKit (tool vendor)](https://outlierkit.com/resources/paddy-galloway-growth-strategy/); [OutlierKit, YouTube strategist page](https://outlierkit.com/resources/youtube-strategist/). This is vendor marketing, so the framing is second-hand.
- **Packaging leverage.** Titles and thumbnails "constitute 50% of success". Small creators "often spend 95% of their time on filming and editing", but the real leverage is in packaging. — [Podwise episode summary (03 Sep 2024)](https://podwise.ai/episodes/1763187); [Podwise episode summary (14 Sep 2026)](https://podwise.ai/episodes/8899459). These are AI-generated summaries, not verbatim quotes.
- **CCN.** Growth means appealing to Core, Casual and New viewers at once. "With the right strategy, any niche can achieve viral reach." — podcast summaries surfaced by search ([Podwise](https://podwise.ai/episodes/1763187); [Colin and Samir](https://www.colinandsamir.com/resources/the-new-rules-of-youtube-from-paddy-galloway)); which page said what could not be separated.
- **Idea funnel.** Hundreds of concepts are filtered through strict elimination criteria to find the high-potential ideas — [OutlierKit](https://alpha.outlierkit.com/resources/paddy-galloway-growth-strategy/) or podcast summaries (search summary; attribution approximate)
- **Niche to broad example.** He cites a permaculture channel's desert/Sahara video. Sources conflict on its views: 15M+ in one, 12M in another. — [OutlierKit](https://alpha.outlierkit.com/resources/paddy-galloway-growth-strategy/); [Podwise](https://podwise.ai/episodes/8899459)
- **His own channel.** About 33 videos in a decade, averaging about 1.0M views each — [OutlierKit teardown](https://alpha.outlierkit.com/resources/paddy-galloway-growth-strategy/) (vendor; not independently verified)
- **Interview.** "Meet The Godfather of YouTube Strategy (Paddy Galloway Interview)" (YouTube ID UHhTKwclHCs); content not retrieved — [VideoHighlight](https://videohighlight.com/v/UHhTKwclHCs)

### Inferences
- Paddy's process can be read as a pipeline: idea bank, outlier validation, a CCN and broad-appeal filter, packaging drafted and tested, then production. It is the strategist's version of the MrBeast memo's "CTR first, then retention".
- The "95% of time on filming and editing" claim implies the cheapest gain for a small creator is moving hours from editing polish into ideation and packaging. For example, write 10–20 title options and mock 3+ thumbnails before scripting.
- CCN explains why some channels repeatedly break out. An idea that serves only core fans caps its reach; one that also hooks casual and new viewers can travel through recommendations.
- His own channel's low output and high average (if accurate) shows that selectivity is a viable system for small channels, not just volume.

### Gaps
- No verbatim Paddy quotes were retrieved, and his X threads were not reachable.
- His client case studies (MrBeast, Mark Rober, Ryan Trahan, Jesser, Sidemen and others) were not retrieved. I cannot confirm from sources which channels he has formally advised.
- "Total addressable market" wording was not confirmed in the retrieved text. **[UNVERIFIED]** He frequently discusses the broad appeal or addressable audience of an idea as a key filter.
- The dates and shows of the two Podwise episodes are not clear beyond the dates on the pages.

## 3. Other consistently viral creators — their repeatable mechanisms

### Takeaway
Within this session's limits only Ryan Trahan was partly documented. His system is a simple, instantly understood constraint (one penny; 50 states in 50 days), run as a serialized multi-part series, tied to a charity, with audience-participation mechanics such as donor-triggered "Wheel of Doom" twists. It has been repeated since 2017 with escalating stakes: $1.38M raised for Feeding America in 2022 and $11.5M for St. Jude in 2025. No sourced material was retrieved for the other 18 creators listed in the brief.

### Cited Findings
- **Penny series.** Trahan's best-known franchise: he has a set time to travel or progress starting with only a penny, and has run it several times since 2017. The franchise dates from 2017, before this brief's preferred window, but has recurred since. — [Wikipedia](https://en.wikipedia.org/wiki/Ryan_Trahan) (search summary)
- **2022 penny series.** He started in California with a single penny, aiming to travel to MrBeast's home in North Carolina and hand-deliver that penny. He raised over $1.38M for Feeding America. — [Wikipedia](https://en.wikipedia.org/wiki/Ryan_Trahan); [Dexerto](https://www.dexerto.com/entertainment/youtuber-ryan-trahan-completes-extreme-mrbeast-penny-challenge-on-final-day-1860308/) (search summary)
- **"50 States in 50 Days" (2025).** Trahan and his wife Haley Pham visited all 50 US states, staying in a different, unusual Airbnb in each, documented the trip online, and raised $11.5M for St. Jude Children's Research Hospital. — [Tubefilter, 30 Jul 2025](https://www.tubefilter.com/2025/07/30/ryan-trahan-haley-pham-50-states-st-jude-charity/). Mid-series coverage reported $5M–$5.5M — [Express Tribune](https://tribune.com.pk/story/2556660/ryan-trahan-raises-55m-in-viral-50-states-in-50-days-challenge); [Primetimer](https://www.primetimer.com/news/youtuber-ryan-trahan-raises-over-5-million-in-donations-for-his-50-states-in-50-days-challenge).
- **Audience lever.** Anyone who gave at least $50,000 bought an activation of the "Wheel of Doom", which forced Trahan and Pham into tricky situations — [Tubefilter](https://www.tubefilter.com/2025/07/30/ryan-trahan-haley-pham-50-states-st-jude-charity/) or [Primetimer](https://www.primetimer.com/news/youtuber-ryan-trahan-raises-over-5-million-in-donations-for-his-50-states-in-50-days-challenge) (search summary; attribution approximate)
- The search returned nothing on Trahan's planning or story process, or on a Colin and Samir interview with him — [search summary; see Wikipedia](https://en.wikipedia.org/wiki/Ryan_Trahan)

### Inferences
- Trahan's mechanism generalises well to small creators:
  - an instantly legible constraint that works as the title (for example, "$0.01 to…" or "50 states in 50 days");
  - daily episodes, each ending on an open question;
  - real stakes and a cause, which drive press, donations and sharing;
  - mechanics that let viewers change the story, such as donation-triggered twists.
- A serialized franchise turns one breakout into many, because each episode inherits the series' momentum and the format can be rerun with higher stakes. This is consistent with Paddy's focus on finding what already over-performs and repeating it.

### Gaps
**No sourced material retrieved.** The search budget ran out before any of these were researched:
- Mark Rober
- Veritasium (Derek Muller)
- Airrack
- Michelle Khare
- Yes Theory
- Dude Perfect
- Kurzgesagt
- Johnny Harris
- Cleo Abram
- Ludwig
- Jynxzi
- IShowSpeed
- Kai Cenat
- Sidemen
- Beta Squad
- Stokes Twins
- Zach King
- Marques Brownlee (MKBHD)

**[UNVERIFIED] leads from background knowledge, to check in a follow-up pass:**
- **Veritasium.** Derek Muller's 2023 video "Clickbait is Unreasonably Effective" argues that provocative packaging is needed to reach a mass audience and is legitimate if the video delivers on the promise. It also discusses changing titles and thumbnails.
- **Mark Rober.** Engineering builds told as stories, for example the recurring glitter-bomb package-thief sequels and the squirrel obstacle courses. He publishes about monthly, and the CrunchLabs subscription-box business launched around 2022.
- **Michelle Khare, "Challenge Accepted".** A fixed series format in which she trains for and attempts elite programmes, with a clear pass/fail stake in each episode.
- **Dude Perfect.** Recurring franchises (Overtime, Stereotypes, trick-shot Battles), and an outside investment of about $100M led by Highmount Capital in 2024.
- **Kurzgesagt.** An animation studio taking months per video, roughly a monthly cadence, and a public "sources" document for each video.
- **Sidemen.** A weekly "Sidemen Sundays" slot, recurring large-cast formats, Charity Match tentpole events, and a multi-channel ecosystem (MoreSidemen, Sides, reacts channels).
- **IShowSpeed.** Country-by-country IRL streaming tours (2024–25) whose clips spread through YouTube, Shorts and fan clip channels.
- **Kai Cenat.** "Mafiathon" subathons; Mafiathon 2 (November 2024) set a Twitch subscriber record.
- **Ludwig.** Moved his streaming to YouTube in late 2021 and runs separate VOD and clips channels.
- **Johnny Harris and Cleo Abram.** Both former Vox explainer journalists; Abram's show is "Huge If True", focused on optimistic technology.
- **Zach King.** Short-form "magic" illusions built with VFX; started on Vine.
- **MKBHD.** More than 15 years of consistent tech-review cadence with a studio team; 2024 backlash over the Panels app.
- **Jynxzi, Stokes Twins, Beta Squad, Airrack and Yes Theory.** No reliable process details recalled.

## 4. What growth consultants and strategists say separates repeat-viral channels from one-hit wonders

### Takeaway
The two sourced systems agree that repeat winners treat each video as a product designed for the platform. They validate ideas against outlier data, design and test the packaging before or alongside production, engineer retention from the first second, and aim for broad appeal (Core, Casual and New viewers) plus something only they can do (the wow factor). The sourced evidence comes only from Paddy Galloway and the MrBeast memo. Views from Creator Hooks (Jake Thomas), Film Booth and Colin and Samir's own commentary were not retrieved.

### Cited Findings
- Paddy Galloway (summaries):
  - packaging is about 50% of success;
  - small creators misallocate about 95% of their time to filming and editing;
  - outliers at 5–15x baseline are the source of repeatable patterns;
  - CCN appeal is the route to broad reach;
  - any niche can reach viral scale.

  Sources: [Podwise](https://podwise.ai/episodes/1763187); [OutlierKit](https://outlierkit.com/resources/paddy-galloway-growth-strategy/); [Colin and Samir](https://www.colinandsamir.com/resources/the-new-rules-of-youtube-from-paddy-galloway)
- Paddy's frameworks circulate through Jay Clouse's Creator Science podcast and Colin and Samir's resources. These are the main creator-economy channels named in the brief, but their own views were not retrieved. — [Creator Science](https://podcast.creatorscience.com/paddy-galloway-2/); [Colin and Samir](https://www.colinandsamir.com/resources/the-new-rules-of-youtube-from-paddy-galloway)
- The MrBeast memo's success definition is YouTube-specific: CTR, AVD and AVP, plus the unmeasurable wow factor, rather than production quality — [document text (GitHub)](https://github.com/echore/blog/blob/efb053927828e5894e5d2935178cf56c839979f5/content/Main/Mrbeast%20production.md); [Energy Crystals](https://www.energycrystals.io/p/what-the-mr-beast-memo-can-teach)
- MrBeast's statement that retention on his newer, story-focused videos is much higher than with his old methods shows that a top channel keeps changing its approach — [MEAWW](https://meaww.com/mr-beast-advocates-for-you-tube-videos-to-focus-more-on-story-internet-says-this-one-was-boring)

### Inferences
- **Repeat-viral channels:**
  1. Have a repeatable way to find ideas (outlier analysis, large idea banks that are filtered hard).
  2. Treat packaging as part of the idea and gate production on it.
  3. Engineer retention structurally (first minute, escalation).
  4. Build recurring formats or series that can be rerun, as Trahan's penny series and 50-states run show.
  5. Keep updating their style as audience tastes shift (MrBeast's move to story).
- **One-hit wonders** typically have a hit whose cause they never isolate. That is an inference: no source quantified it.
- For a small creator, the practical difference is a written, repeatable pipeline plus a review loop against their own baseline, not a bigger budget.

### Gaps
**Not retrieved, because search was exhausted:**
- Jake Thomas / Creator Hooks (title and hook formulas, outlier newsletters);
- Film Booth (idea and packaging frameworks);
- Jay Clouse's own framework (as opposed to hosting Paddy);
- Colin and Samir's interview-derived observations;
- Think Media and vidIQ interviews with top creators.

**[UNVERIFIED] leads:**
- Creator Hooks publishes recurring breakdowns of outlier titles and hooks.
- Film Booth emphasises validating an idea and its title and thumbnail before filming.
- Colin and Samir publish the "Publish Press" newsletter.

## 5. Professional pre-publish checklist and post-publish 48-hour playbook

### Takeaway
The only sourced, top-team practices are pre-publish:
- Settle the title and thumbnail before shooting.
- Produce many thumbnail variants (reportedly up to about 20 per upload at MrBeast).
- A/B test them with YouTube's built-in thumbnail testing.
- Make the first minute deliver on the promise set by the packaging.

No primary or credible secondary source was retrieved for a documented post-publish 48-hour playbook (monitoring against the channel baseline, thumbnail swaps, pinned comments, community posts, Shorts promos). The checklist under Inferences is a synthesis of the sourced practices, not a documented team procedure.

### Cited Findings
- MrBeast's team settles titles and thumbnails before shooting, and its thumbnail lead points to YouTube's thumbnail A/B testing option for trying ideas — [Social Media Today](https://www.socialmediatoday.com/news/youtube-shares-insights-mrbeasts-team-creates-compelling-thumbnail/709817/)
- A/B testing at scale: in 30 tests, closed-mouth thumbnails beat open-mouth ones on watch time, by a small margin — [Social Media Today](https://www.socialmediatoday.com/news/youtube-shares-insights-mrbeasts-team-creates-compelling-thumbnail/709817/)
- Up to about 20 thumbnail variations per upload, at a reported $10,000 per thumbnail — [Social Media Today](https://www.socialmediatoday.com/news/youtube-shares-insights-mrbeasts-team-creates-compelling-thumbnail/709817/); [Nouns News](https://nouns-news.beehiiv.com/p/mrbeast) (second-hand)
- The first minute is where the most viewers are lost, so the effort is concentrated there — [WebSeitz](http://webseitz.fluxent.com/wiki/2024-09-15-LeakedMrBeastMemoOnProduction)
- The three metrics used to judge a video are CTR, AVD and AVP — [document text (GitHub)](https://github.com/echore/blog/blob/efb053927828e5894e5d2935178cf56c839979f5/content/Main/Mrbeast%20production.md)

### Inferences
**Synthesized pre-publish checklist**, each item traced to a finding above:
1. The idea is validated against outliers at 5–15x baseline in the niche or adjacent niches (Paddy).
2. It passes the CCN test (Paddy).
3. The title is written and the thumbnail mocked up before filming (MrBeast team).
4. There are at least 3 thumbnail variants ready for an A/B test; MrBeast makes up to about 20 (MrBeast team).
5. The first minute visibly delivers what the thumbnail and title promise (memo).
6. Minutes 1–3 move from setup to action; the best material sits in minutes 3–6 (memo).
7. There is at least one wow moment the viewer can't get elsewhere (memo).
8. Critical items and owners are confirmed before the shoot (memo, Lamborghini priority example).

**Post-publish (inference only).** Run the built-in thumbnail test from launch. Judge CTR, AVD and AVP against your own channel baseline rather than absolute benchmarks. Treat small, consistent wins as real (the 30-test closed-mouth result).

### Gaps
- No sourced documentation of a professional 48-hour post-publish routine: when to swap thumbnails, CTR or AVD thresholds versus baseline, pinned-comment and community-post tactics, or Shorts teasers for long-form.
- **[UNVERIFIED] leads to verify:**
  - YouTube's "Test & Compare" tool (broad rollout around 2024) tests up to 3 thumbnails and picks the winner by watch-time share, not CTR.
  - YouTube announced title testing in 2025.
  - YouTube Studio's "typical performance" ranges are the usual baseline creators use in the first 24–48 hours.

  Official YouTube help and blog pages were blocked in this session (support.google.com and blog.youtube appear in the proxy's refusal log).

## 6. Hit rates even for top creators, and how they handle failure (idea kill rates, scrapped videos, reshoots)

### Takeaway
No reliable, sourced statistic was found for what fraction of uploads become outliers, for top creators or anyone else. The sourced evidence on handling failure is indirect:
- Very aggressive idea filtering: hundreds of concepts down to a few (Paddy).
- Extreme selectivity: about 33 videos in a decade (Paddy's own channel).
- Persistence on production blockers ("no does not mean no").
- Clear priority ownership of must-have elements (the Lamborghini example).
- Willingness to change a proven format when audience response shifts (MrBeast's move to story, despite "boring" criticism).

### Cited Findings
- Hundreds of concepts are filtered through strict elimination criteria to find the high-potential ideas — [OutlierKit](https://alpha.outlierkit.com/resources/paddy-galloway-growth-strategy/) / podcast summaries (search summary)
- Paddy's own channel: about 33 videos in a decade, averaging about 1.0M views (vendor figure) — [OutlierKit](https://alpha.outlierkit.com/resources/paddy-galloway-growth-strategy/)
- Outliers are defined as about 5–15x a channel's baseline, which implies most uploads are not outliers. No rate is given. — [OutlierKit](https://outlierkit.com/resources/paddy-galloway-growth-strategy/)
- Refusals from outsiders are not accepted at face value; staff exhaust every option first — [Alexander Jarvis repost](https://www.alexanderjarvis.com/memo-how-to-succeed-in-mrbeast-production/)
- In the priority example, anything that pulls an employee away from the #1 task (a Lamborghini under $200k) is the employee's fault — [Alexander Jarvis repost](https://www.alexanderjarvis.com/memo-how-to-succeed-in-mrbeast-production/)
- MrBeast changed his approach toward story and character, reporting higher retention, while some viewers called the new videos boring — [MEAWW](https://meaww.com/mr-beast-advocates-for-you-tube-videos-to-focus-more-on-story-internet-says-this-one-was-boring)

### Inferences
- If an outlier means at least 5x baseline, most videos even on strong channels will not be outliers by definition. A small creator should judge the system by its rolling average and its rate of outliers over many uploads, not by any single video.
- At top teams, most "failure" is absorbed before production, by killing ideas at the idea and packaging gate, which is far cheaper than scrapping finished videos. That fits Paddy's "hundreds of concepts" funnel and MrBeast's packaging-before-shooting rule.

### Gaps
- No sourced figures for:
  - the percentage of uploads that become outliers for MrBeast or any other top channel;
  - the number of ideas MrBeast's team kills, or videos it scraps or reshoots;
  - reshoot policies at Mark Rober, Dude Perfect, Sidemen and others.
- **[UNVERIFIED]** MrBeast has spoken in interviews about scrapping or re-filming expensive videos that did not meet his bar. Specific instances and costs were not verified.
- Follow-up suggestion: interviews by Colin and Samir and on Creator Science, plus Paddy Galloway's breakdowns, are the likeliest sources of numeric hit-rate statements. All were unreachable here.

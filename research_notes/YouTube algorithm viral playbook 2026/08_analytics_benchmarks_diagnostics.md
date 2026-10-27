# YouTube Analytics for Diagnosing, Predicting and Engineering Viral Performance (2026): Metrics, Benchmarks, Viral Trajectories, Diagnostics, Tools

> Method note for the report writer: in this session, direct page fetches were blocked for every external host (support.google.com, vidiq.com, 1of10.com, tubefilter.com, searchenginejournal.com, ppc.land all failed DNS under the sandbox allow-list). The Tavily API was over quota, and the shared WebSearch budget ran out before the last planned queries. Every finding below therefore comes from WebSearch result extracts of the cited pages. They are not full-page reads. Official YouTube statements (Help Center, YouTube Blog, YouTube staff) are tagged **[OFFICIAL]**. Vendor, blog and agency figures are tagged **[THIRD-PARTY]**. Items that rest on one source or on conflicting sources are marked **(unverified)**. Numbers in the Inferences sections that I calculated myself are labelled as my own calculations.

---

## 1. What the core metrics mean, how much each matters, and which ones best predict a breakout

### Takeaway
YouTube's own documentation frames the funnel as impressions, then impressions CTR, then watch behaviour (AVD/APV/retention). Each of these only means something relative to traffic source, audience segment and the channel's own "typical" baseline. YouTube judges packaging by **watch time** rather than CTR: Test & Compare picks winners on watch-time share. The strongest breakout signals are therefore relative velocity (views and impressions vs. the channel's typical video at the same age) together with retention that holds while the audience broadens. A falling CTR during that broadening is expected.

### Cited Findings

**Reach: impressions and impressions CTR**
- **[OFFICIAL]** An impression is logged only when a thumbnail is on screen for **more than one second with at least 50% visible**. Impressions are logged on YouTube search, the homepage, subscription and trending feeds, and "Up Next"/recommendations. They are **not** logged on external websites/embeds, the YouTube Kids or YouTube Music apps, email, or background tabs. Sources: [YouTube Help – Check your impressions and CTR](https://support.google.com/youtube/answer/9314486) and [YouTube Help – Impressions & CTR FAQ](https://support.google.com/youtube/answer/7628154).
- **[OFFICIAL]** YouTube's 2025 article "Decoding CTR & impressions in your Analytics" says that as a video reaches a wider audience and gains impressions, its CTR may fall, because it is expanding past the core audience to viewers "who might not be immediately drawn to click." Its worked example: a video at **10,000 impressions with 9% CTR** (mostly loyal fans) grew to **100,000 impressions and settled at 3.5% CTR**. YouTube says this drop "signals that the content is reaching a broader segment and resonating with new audiences." — [YouTube Help – Decoding CTR & impressions](https://support.google.com/youtube/answer/16767369)
- **[OFFICIAL]** CTR varies by content type, audience, and where on YouTube the impression appeared. Search traffic often shows fewer impressions but higher CTR because viewers have specific intent. High-impression surfaces like the Homepage typically show lower CTR because viewers are "in discovery mode." Sources: [Decoding CTR & impressions](https://support.google.com/youtube/answer/16767369) and [Impressions & CTR FAQ](https://support.google.com/youtube/answer/7628154).
- **[OFFICIAL]** YouTube gives a warning sign for clickbait: **high CTR but low average view duration, together with lower than expected impressions**. Sources: [Impressions & CTR FAQ](https://support.google.com/youtube/answer/7628154) and [Decoding CTR & impressions](https://support.google.com/youtube/answer/16767369).
- **[OFFICIAL, quoted by a third party]** On subscriber click behaviour, YouTube is quoted as saying "Probably all your videos have about maybe a 10% or less click-through rate. That means that even your best videos, 90% of the time your subscribed audience isn't deciding to watch." Sources: [OutlierKit – Does YouTube test videos on subscribers first?](https://outlierkit.com/resources/does-youtube-test-videos-on-subscribers/), with a matching headline at [PPC Land – "Subscribers skip 90% of uploads in their feed, YouTube director says"](https://ppc.land/subscribers-skip-90-of-uploads-in-their-feed-youtube-director-says/). (The speaker's name could not be verified from the extracts.)
- **[THIRD-PARTY]** Early impressions come mostly from existing subscribers, who click at higher rates. Suggested and home-feed placements reach colder viewers who click less often even when the packaging is unchanged. — [AIR Media-Tech glossary](https://air.io/en/youtube-glossary/what-are-youtube-impressions-and-ctr)

**Views, engaged views, unique viewers, realtime**
- **[OFFICIAL]** Shorts view counting changed on **March 31, 2025**. A Shorts view now counts as soon as the Short starts to play or replays, with **no minimum watch time**. The previous metric is kept as **"engaged views"** in Advanced Mode. YPP eligibility and earnings are still based on engaged views. Sources: [Social Samosa](https://www.socialsamosa.com/news-2/youtube-shorts-now-count-every-play-replay-view-8895256), [eMarketer](https://emarketer.com/content/youtube-shorts-changes-view-count-rules-match-tiktok--instagram), [MobileSyrup](https://mobilesyrup.com/2025/03/27/youtube-changes-how-it-counts-shorts-views/) and [Search Engine Journal](https://www.searchenginejournal.com/youtube-changes-shorts-view-counts-no-change-to-monetization/543005/).
- **[OFFICIAL]** YouTube defines engaged views as "how many times viewers stayed to watch past the initial seconds, not including any loops." For Shorts, "stayed to watch" is the percentage of views that get past those initial seconds. Sources: [YouTube Help – Understand your content performance](https://support.google.com/youtube/answer/12220281) and [YouTube Help – Understand your audience](https://support.google.com/youtube/answer/9314416).
- **[OFFICIAL]** Unique viewers is the "estimated number of viewers that watched your content within the selected date range." It is available for periods of up to **90 days**. A viewer who watches several of your videos counts as a unique viewer for each video but as one unique viewer for the channel. For Shorts, engaged views are used to estimate unique viewers. — [YouTube Help – Understand your unique viewers data](https://support.google.com/youtube/answer/7577916)
- **[OFFICIAL]** Realtime activity "only shows estimates of potential view activity" and may not match the watch-page count. It is one of the report views in the Overview tab. — [YouTube Help – Get started with YouTube Analytics](https://support.google.com/youtube/answer/9002587)

**Retention: audience retention, key moments, typical retention**
- **[OFFICIAL]** The Key Moments report has four parts:
  - **Intro**: the percentage of the audience still watching after the first 30 seconds. A strong intro suggests the opening matched what the title and thumbnail promised.
  - **Spikes**: moments that were rewatched or shared. A spike can mean interest, or that the content was confusing.
  - **Dips**: moments that were skipped or where viewers left.
  - **Gradual decline** is normal ("Videos on YouTube generally taper off during the playback period").

  Source: [YouTube Help – Measure key moments for audience retention](https://support.google.com/youtube/answer/9314415)
- **[OFFICIAL]** "Typical retention" is "the engagement that the **last 10 of your videos of a similar length** have maintained." This is the official comparison baseline. — [YouTube Help – Measure key moments](https://support.google.com/youtube/answer/9314415)
- **[OFFICIAL] (threshold wording unverified)** According to a search extract of the Help pages, videos with **50% or more** of the audience still watching at the 30-second mark appear in an "above typical intros" list. Sources: [Measure key moments](https://support.google.com/youtube/answer/9314415) and [Content tab analytics tips](https://support.google.com/youtube/answer/12942217).
- **[OFFICIAL]** Audience retention data typically takes **1–2 days** to process. If a video's best moments come late, YouTube suggests moving them earlier, because audience size usually shrinks over the length of a video. — [YouTube Help – Content tab analytics tips](https://support.google.com/youtube/answer/12942217)

**Audience segments (new / casual / regular)**
- **[OFFICIAL]** The three segments:
  - **New viewers** watched the channel for the first time in the selected period.
  - **Casual viewers** watched at least once a month for **1–5 of the trailing 12 months**.
  - **Regular viewers** watched at least once a month for **6+ months**. One source says 7 or more of the trailing 12 months, so this threshold is in conflict.

  Viewers browsing privately, with deleted watch history, or after a gap of more than a year count as new. Sources: [YouTube Help – New, casual & regular viewers tips](https://support.google.com/youtube/answer/13615784), [PPC Land](https://ppc.land/youtube-introduces-refined-viewer-analytics-with-casual-and-regular-metrics/) and [Search Engine Journal](https://www.searchenginejournal.com/youtube-adds-new-viewer-metrics-to-track-audience-loyalty/550289/).
- **[OFFICIAL]** These segments **replaced the old binary "returning viewers" metric** and are "not a direct equivalent" of it. They were announced **July 24, 2025** and apply to Shorts, long-form (VOD) and live. YouTube says regular viewers are "a high bar," so a small share is expected. Sources: [PPC Land](https://ppc.land/youtube-introduces-refined-viewer-analytics-with-casual-and-regular-metrics/), [SEJ](https://www.searchenginejournal.com/youtube-adds-new-viewer-metrics-to-track-audience-loyalty/550289/) and [YouTube Help 13615784](https://support.google.com/youtube/answer/13615784).

**Traffic sources (official definitions)**
- **[OFFICIAL]** YouTube's definitions:
  - **Browse features**: Home, subscriptions, Watch Later, Trending/Explore and other browsing features.
  - **Suggested videos**: suggestions next to or after other videos, plus links in video descriptions.
  - **Notifications**: split into notifications to belled subscribers (who turned on "All notifications" and device notifications) and other notifications such as email, inbox and digests.
  - **Playlists**: any playlist that includes your video, including viewers' "Liked videos" and "Favorite videos."
  - **Channel pages**: your channel or other channels.
  - **External**: websites and apps that embed or link to the video.
  - **Direct or unknown**: direct URL entry, bookmarks, signed-out viewers and unidentified apps.

  Further categories include YouTube search, Shorts feed, end screens, cards and product pages. Sources: [YouTube Help – Understand your video reach](https://support.google.com/youtube/answer/9314355) and [YouTube Help – Understand your content performance](https://support.google.com/youtube/answer/12220281).
- **[OFFICIAL]** Unchecking "notify subscribers" keeps an upload out of subscribers' feeds and notifications. OutlierKit reports that YouTube advises against doing this. Sources: [YouTube Help 7457584](https://support.google.com/youtube/answer/7457584) and [OutlierKit](https://outlierkit.com/resources/does-youtube-test-videos-on-subscribers/).

**"Typical performance" and ranking**
- **[OFFICIAL]** The Overview tab shows personalised comparisons against your usual results. At channel level, "typical performance" compares the channel with its usual performance. At video level, it compares a video with typical performance. — [YouTube Help – Get an overview of channel performance](https://support.google.com/youtube/answer/9314414)
- **[THIRD-PARTY]** One 2026 guide says the widget shows how your latest videos compare to your typical performance "within the first few hours or days after publishing." The specific guide among the search results could not be pinned down; see [Alan Spicer](https://alanspicer.com/youtube-analytics-explained/), [Improvado](https://improvado.io/blog/youtube-analytics-guide) and [FrameOS](https://frameos.studio/blog/how-to-read-youtube-analytics).

**What YouTube says it optimises for**
- **[OFFICIAL]** Test & Compare picks the winning title or thumbnail by **watch time share**, not CTR. YouTube says this "helps guide creators toward sustainable growth, rather than incentivizing clickbait-style approaches that fail to hold attention." One source describes the metric as "watch time per impression." Sources: [YouTube Help – A/B test titles & thumbnails](https://support.google.com/youtube/answer/16391400), [SEJ](https://www.searchenginejournal.com/youtube-title-a-b-testing-rolls-out-globally-to-creators/562571/) and [ThumbnailTest](https://thumbnailtest.com/news/youtube-releases-title-test-compare/).
- **[OFFICIAL, via press]** A YouTube spokesperson said metrics like CTR and AVD are "only one of dozens of signals" feeding search and discovery. — [Tubefilter](https://www.tubefilter.com/?p=148002)
- **[OFFICIAL, via press]** Todd Beaupré, YouTube's Senior Director of Growth & Discovery, describes recommendations as "pulled" per viewer when each user opens YouTube. He says the system learns separately for different audiences, so a video can underperform with subscribers while performing with people who have never watched the channel. Sources: [SEJ – YouTube Algorithm Myths Debunked](https://www.searchenginejournal.com/youtube-algorithm-myths-debunked-insights-from-the-growth-team/510091/) and [KDCC summary](https://blog.kdcc.social/youtubes-growth-director-just-debunked-6-algorithm-myths/).

**Metrics changed or renamed, 2025–2026**
- **[OFFICIAL]** Shorts views were redefined on March 31, 2025. The old definition became "engaged views" (sources above).
- **[OFFICIAL]** "Returning viewers" was replaced by casual and regular viewers in July 2025 (sources above).
- **[OFFICIAL]** Test & Compare was expanded from thumbnails (2024) to titles and title+thumbnail combinations (2025). See Q5.
- **[OFFICIAL/press]** A **Studio redesign test began July 16, 2026** for a limited group of creators. It renames the **Analytics tab to "Insights"**, groups related metrics, keeps an Advanced Mode for detailed charts, and adds **four AI insight cards: Channel Summary, Content Patterns, Audience Loyalty, Video Summary**. YouTube Help says an updated Studio experience is gradually rolling out from July 2026. Sources: [Net Influencer](https://www.netinfluencer.com/youtube-tests-redesigned-studio-analytics-with-ai-insight-cards/), [Social Samosa](https://www.socialsamosa.com/news-2/youtube-tests-redesigned-studio-ai-insights-research-tools-creators-12172699), [Social Media Today](https://www.socialmediatoday.com/news/youtube-refreshes-studio-and-updates-video-guidance/825496/) and [YouTube Help 9002587](https://support.google.com/youtube/answer/9002587).
- **[THIRD-PARTY] (unverified, single source)** The same test reportedly turns the Trends tab into an outlier-scored **"Research"** tab. It would show other channels' videos with subscriber counts, views, video age and an "outlier multiplier." Desktop Saved Keywords would be retired, with a three-month export window. — [MiraFlow](https://miraflow.ai/blog/youtube-studio-insights-redesign-explained-2026)
- **[PRESS]** Other late-2026 changes:
  - The Ask Studio AI assistant is expanding to iOS and Android ([TechCrunch, Sept 23, 2026](https://techcrunch.com/2026/09/23/youtube-releases-new-ai-features-for-creators-within-its-studio-app/)).
  - Studio now separates **paid vs. organic** analytics (views, engaged views, likes, comments, shares, watch time) and adds an estimated-revenue column ([SocialBee 2026 updates log](https://socialbee.com/blog/youtube-updates/)).
  - One extract says that at Made On YouTube (Sept 2026), YouTube promised analytics that explain *why* videos perform. A second search found no mention of this, so it is in conflict ([SocialBee](https://socialbee.com/blog/youtube-updates/)).
- **[THIRD-PARTY] (unverified, single source)** CineD reports that "from August 24 that ten-second requirement is gone, and every format behaves the way Shorts already does." That would mean view counting changed beyond Shorts. No second source was found. — [CineD](https://www.cined.com/?p=435859)

### Inferences
- **Recommended order for reading long-form metrics** (my synthesis of the official funnel and diagnostic guidance):
  1. **Impressions vs. the channel's typical video at the same age.** This is the system's verdict on demand and competition, and it caps everything else.
  2. **Impressions CTR, broken down by traffic source and read against impression volume.** An aggregate CTR mixes high-CTR Search and subscriber traffic with low-CTR Home traffic.
  3. **Retention:** intro (30-second) retention, then AVD/APV against "typical retention" (last 10 similar-length videos), then dips.
  4. **Watch time per impression ≈ CTR × AVD.** This is the composite closest to Test & Compare's watch-time-share criterion.
  5. **Audience expansion:** share of views from non-subscribers and new viewers, and growth of Browse/Suggested.
  6. **Loyalty and satisfaction:** moving viewers from casual to regular, subscribers gained, and engagement.
- **Standard definitions** (arithmetic, not taken from an extract):
  - AVD = watch time ÷ views.
  - APV = AVD ÷ video length.
  - Views from impressions = impressions × CTR.
  - Therefore watch time from impressions = impressions × CTR × AVD.
- **Most predictive breakout signals**, ranked by strength of evidence:
  - (a) velocity relative to the channel's own baseline (typical-performance comparison, VPH vs. channel norm; see Q3);
  - (b) impressions accelerating while intro retention and APV stay at or above typical;
  - (c) traffic shifting toward Browse/Suggested and new viewers;
  - (d) CTR falling gradually while absolute clicks keep rising (YouTube's official 9% → 3.5% example).
- **Shorts** need a separate funnel: shown in feed, then viewed vs. swiped (hook), then APV/loops, then engaged views, then subscribers. Classic impressions CTR barely applies to Shorts.

### Gaps
- No official methodology was found for the video-level "typical performance" ranking (e.g., "Ranking by views: 3 of 10"). It is unclear whether it uses the median, whether it compares at the same age, or whether the window is the last 10 uploads.
- The widely cited Realtime windows (last 48 hours / last 60 minutes) were not confirmed in retrieved text.
- No Creator Insider episode transcripts were retrieved.
- YouTube does not publish a weighting of metrics. "Only one of dozens of signals" is the only official framing found.
- The CineD all-format view-count claim and the "Research tab/outlier multiplier" claim each rest on one source.

---

## 2. Benchmark ranges for the key metrics (official vs. third-party, with sample sizes)

### Takeaway
The only large-sample **official** benchmark is that **half of all channels and videos have an impressions CTR between 2% and 10%**. YouTube's other "benchmark" is your own last 10 similar-length videos. Third-party retention data points to a platform average APV in the **low-to-mid 20s**: Retention Rabbit reports 23.7% average, with only 16.8% of videos above 50%. Niche-level CTR tables and Shorts "viewed vs. swiped" thresholds are mostly estimates without disclosed samples, and they contradict each other.

### Cited Findings

**Official anchors**
- **[OFFICIAL]** "Half of all channels and videos on YouTube" have an impressions CTR of **2%–10%**. New videos or channels, or videos with **fewer than 100 views**, can see an even wider range. Third-party guides stress that this describes the population and is not a target. Sources: [YouTube Help – Impressions & CTR FAQ](https://support.google.com/youtube/answer/7628154), relayed by [Umbrella Creators](https://umbrellacreators.com/tools/youtube-thumbnail-ctr-benchmark) and [vidIQ](https://vidiq.com/blog/post/6-tips-good-CTR-youtube/).
- **[OFFICIAL]** The retention baseline is "typical retention" from the last 10 videos of similar length. — [YouTube Help 9314415](https://support.google.com/youtube/answer/9314415)
- **[OFFICIAL] (threshold wording unverified)** 50% or more of viewers still watching at 30 seconds places a video in the "above typical intros" list. — [YouTube Help 9314415](https://support.google.com/youtube/answer/9314415) and [12942217](https://support.google.com/youtube/answer/12942217)
- **[OFFICIAL, quoted]** Subscriber CTR on uploads is "about maybe a 10% or less." — [OutlierKit](https://outlierkit.com/resources/does-youtube-test-videos-on-subscribers/)

**Third-party retention benchmarks**
- **[THIRD-PARTY] Retention Rabbit 2025 benchmark report:**
  - average retention **23.7%**;
  - only **16.8%** of videos exceed **50%** average retention;
  - **55%** of viewers lost by the 60-second mark;
  - channels in the top quartile for retention see **3.5x** higher subscriber growth;
  - intros holding **more than 65%** of viewers correlate with **58% higher AVD**.

  The sample is described inconsistently by secondary sources: "10,000+ videos across 1,000+ channels" in one, "75+ niches, 2024–2025" in another. The original was reachable only through a translation proxy, so it is **unverified**. Sources: [Retention Rabbit report](https://www.retentionrabbit.com/blog/2025-youtube-audience-retention-benchmark-report), [Stripo research summary](https://research.stripo.email/youtube-benchmarks) and [Gyre](https://gyre.pro/blog/how-to-improve-audience-retention-on-youtube-top-tips).
- **[THIRD-PARTY] (unverified)** Retention by length, attributed to the same report: **5–10 minute** videos average about **31.5%**, and **under-5-minute** videos about **25–30%**. — secondary summary in [Stripo](https://research.stripo.email/youtube-benchmarks); not checked against the original.
- **[THIRD-PARTY] vidIQ:** a realistic "good" target for a **6–9 minute** talking-head or education video is about **30% APV**. vidIQ says third-party studies of thousands of videos put the platform average in the **low-to-mid 20s**. — [vidIQ – Audience retention](https://vidiq.com/blog/post/increase-audience-retention-youtube/)
- **[THIRD-PARTY] 2026 vendor "good APV" targets** contradict each other and sit well above the measured averages. No samples are disclosed. Sources: [PrePublish](https://prepublish.ai/guides/youtube-retention-guide), [Humble&Brag](https://humbleandbrag.com/blog/youtube-audience-retention-benchmarks), [Retti](https://retti.ai/guides/what-is-a-good-retention-rate), [LenosTube](https://www.lenostube.com/en/youtube-audience-retention-average-good-and-best-benchmarks/) and [InstantViews](https://instantviews.net/youtube-benchmarks).

  | Video length | Low end of "good" claims | High end of "good" claims |
  |---|---|---|
  | Under 5 min | ~50–70% | ~70–90% |
  | 5–10 min | ~40–55% | ~50–70% |
  | 10–20 min | ~30–45% | ~40–60% |
  | 20+ min | ~20–35% | ~35–50% |

**Third-party CTR benchmarks**
- **[THIRD-PARTY]** No rigorous multi-channel study of CTR by niche was found. Stripo's 2025 report says it analysed **10,000+ videos from 1,000+ creators**, but its CTR section cites other blogs. Umbrella Creators states that its niche rows are "estimates, not measured from channel data." Sources: [Stripo](https://research.stripo.email/youtube-benchmarks) and [Umbrella Creators](https://umbrellacreators.com/tools/youtube-thumbnail-ctr-benchmark).
- **[THIRD-PARTY]** Niche ranges conflict:
  - Gaming: 7–10% vs. 4–7% vs. 8–15%.
  - Education: 3–6% vs. 2–5%.
  - Music: 1–3% (one source).

  Sources: [HookSnap](https://www.hooksnap.io/blog/youtube-average-ctr-by-niche-2026), [Click Studio](https://www.clickstudio.co/blog/youtube-ctr-benchmarks), [Artiphik](https://artiphik.com/blog/youtube-ctr-benchmarks-by-niche) and [LenosTube](https://www.lenostube.com/en/youtube-ctr-benchmark-average-good-best-practices/).
- **[THIRD-PARTY]** Channel size matters more than niche in one source: channels under 1,000 subscribers at **8–20%** CTR vs. channels over 1M at **1.5–4%**. Other small-channel ranges given are 4–10% and 6–10% for channels under 1K subscribers. One guide gives YouTube Search CTR as **8–15%**, with no attribution. Sources: same set as above, plus [TubeAnalytics – small channels](https://www.tubeanalytics.net/blog/good-ctr-small-channels-2026) and [Teleprompter](https://www.teleprompter.com/blog/whats-a-good-click-through-rate-on-youtube).

**Shorts benchmarks (all third-party; no official benchmark)**
- **[THIRD-PARTY]** "Viewed vs. swiped away" (the "How many chose to view" card) thresholds:
  - top creators about **75–80% viewed**;
  - "good" **70–90%**;
  - more than **70%** claimed to trigger viral distribution;
  - under **60%** claimed to stop distribution to new audiences.

  Creator Essentials says no universal benchmark exists, and one source notes the Help page describes what the card measures, not how ranking uses it. Sources: [Creator Essentials](https://www.creatoressentials.com/glossary/viewed-vs-swiped-away/), [1of10 Shorts analytics](https://1of10.com/blog/youtube-shorts-analytics/), [Shortimize](https://www.shortimize.com/blog/how-to-analyze-youtube-shorts-performance), [Buffer](https://buffer.com/resources/the-creators-guide-to-youtube-shorts-analytics/) and [Everpop](https://everpop.app/blog/how-to-read-youtube-shorts-analytics).

**Engagement-rate benchmarks (formulas differ by vendor)**
- **[THIRD-PARTY] HypeAuditor** compares a channel's engagement rate against creators in the same tier and labels it Low, Average, Good or Excellent. It publishes no numeric thresholds. ER is computed over the latest **30 videos**, with selectable 30/90/180/360-day windows. — [HypeAuditor Help](https://help.hypeauditor.com/en/articles/6227916-what-is-youtube-engagement-rate-and-how-do-you-calculate-it)
- **[THIRD-PARTY] Modash:** the "Average" band is about **0.36–0.51%** for 10K–50K channels and about **0.13–0.18%** for 1M+ channels. Modash also calls "0.73%–2.5%" standard. **Scrumball:** for channels under 1K and 1K–5K subscribers, "Good" is about **2–2.9%** and "Average" about 1.5–1.9%. A general rule of thumb puts YouTube ER at about **2%**. Sources: [Modash](https://modash.io/youtube-engagement-rate-calculator) and [Scrumball](https://scrumball.com/tools/youtube-engagement-rate-calculator).

**Velocity benchmark**
- **[THIRD-PARTY]** An analysis of **2,826 videos** concluded that "the better benchmark is a video's VPH relative to its channel's normal velocity" rather than an absolute VPH. The analysis was published by a tool vendor. — [OverseerOS – VPH](https://www.overseeros.com/blog/youtube-vph-views-per-hour) and [YTGrowth – VPH meaning](https://ytgrowth.io/blog/youtube-vph-meaning) (the extract did not pin down which of the two carried the study)

### Inferences
- **Working benchmark card** (my synthesis; always prefer the channel's own medians):

  | Metric | Normal band | "Good / outlier" signal | Evidence quality |
  |---|---|---|---|
  | Long-form impressions CTR (all sources) | 2–10% (official, half of channels) | Above your own median at a similar impression volume. Expect higher on Search and subscriber surfaces, lower on Home. | Official population stat; niche tables unreliable |
  | APV, 6–10 min videos | ~20–30% (RR average 23.7%; vidIQ "low-to-mid 20s") | ≥30% is good (vidIQ); ≥50% is roughly the top 17% (RR) | Third-party, unverified samples |
  | Intro retention (30 s) | — | ≥50% is "above typical" (Studio, if verified); ≥65% correlates with much higher AVD (RR) | Mixed |
  | Shorts viewed vs. swiped | ~60–70% | ≥70–80% | Third-party, no samples |
  | Engagement rate | ~0.1–0.5% for larger channels, up to ~2–3% for small channels (vendor-dependent) | Above your tier's band | Vendor formulas differ |
  | Subscriber CTR on uploads | ≤~10% (YouTube quote) | — | Official quote |

- Vendor "good APV" tables (50–90% for short videos) are far above measured averages (about 24%). The report should present them as aspirational marketing claims, not norms.

### Gaps
- **Subscriber conversion** (subscribers gained per 1,000 views): no reliable benchmark was retrieved.
- **Returning-viewer share** (and the new casual/regular shares): no benchmark was found. The only guidance is YouTube's statement that regular viewers are "a high bar."
- No CTR benchmarks by traffic source or impression level with disclosed samples were found from vidIQ, TubeBuddy, 1of10, Social Blade or Tubefilter.
- HypeAuditor's numeric tier thresholds are not public in the retrieved material.
- Retention Rabbit's methodology and length breakdown could not be verified against the original report.

---

## 3. What a video looks like in the data when it takes off, and which first 1–48 hour signals predict it

### Takeaway
YouTube's own worked example of a successful video shows **impressions growing about 10x while CTR falls from 9% to 3.5%**, which YouTube reads as the video reaching broader audiences. That broadening runs from subscribers to colder Home and Suggested viewers. YouTube's growth lead stresses that the first 24 hours do not decide a video's fate, and that many videos gain most of their audience much later. The best-documented early predictor is **relative velocity**: early views against the channel's own norm. Academic work shows early and later views are log-linearly related, but YouTube needed about 10 days of data, not hours, to forecast well.

### Cited Findings
- **[OFFICIAL]** A breakout shows impressions rising sharply while CTR falls: 10,000 impressions at 9% grew to 100,000 at 3.5%. This "signals that the content is reaching a broader segment and resonating with new audiences." — [YouTube Help 16767369](https://support.google.com/youtube/answer/16767369)
- **[THIRD-PARTY]** Early impressions skew to subscribers, who click more. Later Suggested and Home impressions reach colder viewers who click less with the same packaging. A falling CTR should be checked against retention: high CTR with fast abandonment signals a mismatch. — [AIR Media-Tech](https://air.io/en/youtube-glossary/what-are-youtube-impressions-and-ctr)
- **[OFFICIAL, via press]** Todd Beaupré says the first 24 hours don't decide a video's fate. Some videos peak on day one, and others "accumulate the bulk of their audience a month or more after publication." The system learns separately per audience. One video's poor performance won't irreversibly affect the channel. Sources: [SEJ](https://www.searchenginejournal.com/youtube-algorithm-myths-debunked-insights-from-the-growth-team/510091/) and [KDCC](https://blog.kdcc.social/youtubes-growth-director-just-debunked-6-algorithm-myths/). A secondhand source dates a similar statement to **September 2026** ("many videos get most of their views a month or more after upload"). — [AITuber](https://aituber.app/blog/youtube-algorithm-changes/) (unverified)
- **[OFFICIAL, quoted]** Even a channel's best videos convert about 10% or less of subscribers who see them, so day-one subscriber traffic is a small, biased sample. — [OutlierKit](https://outlierkit.com/resources/does-youtube-test-videos-on-subscribers/)
- **[THIRD-PARTY]** A YouTube liaison reportedly said the subscription feed "hasn't been updated in years" and that the homepage algorithm can deprioritise older subscriptions. One creator's subscription-feed impressions had declined over time. — [Lon.tv, July 10, 2024](https://blog.lon.tv/2024/07/10/youtube-acknowledges-that-subscriptions-dont-matter-as-much-anymore/)
- **[ACADEMIC]** Szabo & Huberman, "Predicting the Popularity of Online Content" (arXiv 2008; *Communications of the ACM* 2010, pp. 80–89):
  - They found a **log-linear relationship** between a video's early views and its later views.
  - The dataset was **7,146 YouTube videos** from the "recently added" section.
  - Digg stories could be forecast 30 days ahead from the first 2 hours of data. YouTube videos "need to be followed for **10 days** to reach the same performance."

  Note that this is 2008 data, before modern recommendations. Sources: [arXiv 0811.0405](https://arxiv.org/abs/0811.0405), [ar5iv HTML](https://ar5iv.labs.arxiv.org/html/0811.0405) and [MIT Technology Review](https://www.technologyreview.com/2008/12/04/217469/a-winning-web-formula).
- **[THIRD-PARTY] vidIQ VPH:** "Views Per Hour (VPH) aka view velocity is a great way to determine which videos are taking off to become viral. VPH updates over time so even if a video is older you can still see if viewership is heating up!" The metric was added to the Chrome extension as "Velocity" in **2014**. Users can set keyword alerts on a VPH threshold (e.g., more than 1k VPH). Sources: [vidIQ Support – What is VPH](https://support.vidiq.com/en/articles/108672-what-is-vph-views-per-hour), [vidIQ Velocity launch](https://vidiq.com/blog/post/vidiq-velocity/) and [Kripesh Adwani review](https://kripeshadwani.com/vidiq-review/).
- **[THIRD-PARTY]** Relative VPH, meaning a video's velocity against its channel's norm, beats absolute VPH as a benchmark (2,826-video analysis). VPH is not shown in Studio; tools compute it as views ÷ hours since publish. — [OverseerOS](https://www.overseeros.com/blog/youtube-vph-views-per-hour) and [YTGrowth](https://ytgrowth.io/blog/youtube-vph-meaning)
- **[OFFICIAL]** The clickbait pattern that **fails** to take off is high CTR, low AVD, and lower than expected impressions. — [YouTube Help 7628154](https://support.google.com/youtube/answer/7628154)
- **[PRESS]** Tubefilter reports that the most common case creators raise is a video that looks weak on views while its CTR and AVD look healthy. — [Tubefilter](https://www.tubefilter.com/?p=148002)

### Inferences
- **Viral-trajectory signature by phase** (a pattern I built from the mechanisms above; not a published YouTube model):

  | Window | What a breakout typically shows | False-positive or warning pattern |
  |---|---|---|
  | 0–2 h | Notification, subscription and Browse traffic dominate. CTR is often above the channel median because subscribers click more. Realtime/VPH is above the channel's typical early curve. | A high-CTR spike from loyal fans that does not translate into rising Home impressions. |
  | 2–24 h | Impressions accelerate, not just accumulate. The share of Browse (Home) and Suggested rises. CTR declines from its launch peak while total clicks keep climbing. Intro (30 s) retention is at or above typical. | CTR collapses *and* impressions plateau. Or high CTR with low AVD and lower-than-expected impressions (the official clickbait pattern). |
  | 24–72 h | The "typical performance" comparison is clearly above normal. New-viewer and non-subscriber shares rise. Suggested grows as the video is paired with other channels' videos. | Most views come from External (one-off spikes) or Search (capped by query demand). |
  | 7–30+ days | Long tail through Suggested and Search, or late resurfacing on Home. YouTube says many videos earn most of their views a month or more later. | Decay to near zero after the subscriber wave, which suggests the topic only fits the core audience. |

- **Early-prediction rule of thumb:** treat 24–72 hour velocity relative to the channel's median at the same age as the main early predictor. Confirm with traffic-source mix and retention. Szabo & Huberman's 10-day horizon and Beaupré's comments both argue against declaring failure on day one.
- A falling CTR is only "good" when impressions are growing faster than CTR is shrinking, so that views keep rising, and retention holds. In YouTube's example, clicks rose from about 900 to about 3,500, roughly 3.9x (my arithmetic).

### Gaps
- No public dataset or YouTube statement was found that quantifies which first 1–48 hour Studio metrics predict breakouts (for example, a CTR or retention threshold at hour 24).
- No case studies with screenshots and numbers (beyond YouTube's own worked example) were retrieved before the search budget ran out. Paddy Galloway, Film Booth and Creator Hooks breakdowns with real Studio numbers remain unretrieved.
- The Szabo–Huberman correlation coefficient was not captured, and the study is pre-2010.

---

## 4. Diagnostic frameworks and a decision tree for underperforming videos and channels

### Takeaway
YouTube's official guidance and creator-tool frameworks agree on the core rules:
- Check impressions first. Low reach can reflect **competition or a narrow topic**, not just bad packaging.
- Diagnose CTR **per traffic source**.
- Read CTR and retention **together**:
  - high CTR + low retention means overpromise/delivery;
  - low CTR + high retention means packaging;
  - good metrics + low impressions means a small addressable audience or strong competition.
- Fix intro problems by aligning the opening with the title and thumbnail promise.

### Cited Findings
- **[OFFICIAL]** On low impressions:
  - "Beyond your channel's performance, high competition means your video is ranked against countless others. If other videos perform even better, your content may not reach as many viewers."
  - For narrow topics, high CTR and AVD can come from the whole small pool of interested viewers, which the system will eventually exhaust.
  - Metadata changes "are recommended when a video has a lower CTR and is receiving fewer impressions than usual. If these adjustments do not improve performance, it may indicate that the video's topic appeals to a smaller audience."

  Sources: [YouTube Help – Decoding CTR & impressions](https://support.google.com/youtube/answer/16767369), [Impressions & CTR FAQ](https://support.google.com/youtube/answer/7628154) and [Good to know about recommendations](https://support.google.com/youtube/answer/16559651).
- **[OFFICIAL]** On low CTR:
  - Small CTR variations are common and "aren't cause for immediate action." Improvements might be helpful "if a change in CTR is statistically significant."
  - Avoid manually A/B testing titles or thumbnails on the same video, because CTR differences "might be due to traffic sources, rather than the title or thumbnail."
  - Avoid clickbait, whose signature is high CTR, low AVD and lower-than-expected impressions.

  Sources: [Impressions & CTR FAQ](https://support.google.com/youtube/answer/7628154) and [Decoding CTR & impressions](https://support.google.com/youtube/answer/16767369).
- **[OFFICIAL]** On retention:
  - For a weak intro, make the thumbnail and title better reflect the content, and edit the opening to "experiment with different styles."
  - Move top moments earlier.
  - Review dips for why viewers left.

  Source: [YouTube Help – Content tab analytics tips](https://support.google.com/youtube/answer/12942217).
- **[THIRD-PARTY] OutlierKit diagnostic examples:** **2.1% CTR with 55% AVD** indicates a title/thumbnail problem. **6.5% CTR with 28% AVD** indicates a hook problem. Compare against the channel's own average. — [OutlierKit – How to get more views](https://outlierkit.com/resources/how-to-get-more-views-on-youtube/)
- **[THIRD-PARTY] Crepal sequence:** check impressions first (low means distribution), then CTR (high impressions with low CTR means packaging). Split CTR by source: low Browse CTR points to the thumbnail, low Search CTR points to a title/intent mismatch. — [Crepal](https://crepal.ai/blog/aivideo/youtube-video-analysis-tool-guide/)
- **[THIRD-PARTY] Subscribr:** the biggest drop in the first 30 seconds usually means a hook problem. Drops later in the video usually point to pacing or structure. Sources: [Subscribr – Reach tab explained](https://subscribr.ai/p/youtube-analytics-reach-tab-explained) and [Subscribr – Continuous improvement](https://subscribr.ai/p/youtube-analytics-continuously-improve-content).
- **[THIRD-PARTY] Paddy Galloway** (consultant to MrBeast, Ryan Trahan and others), per podcast summaries:
  - Titles and thumbnails are about **50%** of a video's success.
  - He prioritises **retention curves over CTR**, which he treats as a vanity metric.
  - His **CCN framework** says a video should serve **Core, Casual and New** viewers while keeping a through-line for existing fans.

  Sources: [Colin & Samir](https://www.colinandsamir.com/resources/the-new-rules-of-youtube-from-paddy-galloway), [Creator Science podcast](https://podcast.creatorscience.com/paddy-galloway/) and [Transcript Desk](https://thetranscriptdesk.substack.com/p/the-new-rules-of-youtube-2025-edited). Related: [Spotter Studio – The three audiences every YouTube video should serve](https://www.spotterstudio.com/blog/the-three-audiences-every-youtube-video-should-serve).
- **[THIRD-PARTY]** A newsletter cites a December 2022 Galloway thread on when to watch CTR, AVD, returning vs. new viewers and traffic sources. The full thread text was not retrieved. — [The Viral Post](https://theviralpost.beehiiv.com/p/youtube-is-rigged)
- **[OFFICIAL, via press]** The system learns per audience: a video can fail with subscribers and succeed with non-viewers. One weak video doesn't irreversibly hurt a channel. — [SEJ](https://www.searchenginejournal.com/youtube-algorithm-myths-debunked-insights-from-the-growth-team/510091/)
- **[THIRD-PARTY]** Use the **median** CTR and AVD of your last **10–15 videos of similar length and topic** as the baseline. One expert advises waiting for **at least 1,000 views and two weeks** before interpreting a video. These come from a 2026 search-result set; the exact page could not be pinned down. See [Alan Spicer](https://alanspicer.com/youtube-analytics-explained/), [Gyre](https://gyre.pro/blog/why-your-youtube-metrics-are-decreasing-and-what-you-can-do-about-it) and [TubeAnalytics](https://www.tubeanalytics.net/blog/youtube-analytics-complete-guide).

### Inferences
- **Diagnostic decision tree** (my synthesis; each branch notes its evidence):

```
STEP 0 – Is the data mature and comparable?
  • Compare at a fixed age (24 h / 72 h / 7 d / 28 d) against the MEDIAN of your last ~10 similar videos
    (same format, similar length and topic)                              [official "typical" uses last 10]
  • Long-form CTR: wait for ~1,000–2,000+ impressions                    [third-party rule of thumb; see Q7]
  • Retention: wait 1–2 days for processing                              [official]
  • Not mature -> wait. Don't react to day-to-day wiggles                [official]
  • Shorts? -> use the Shorts branch (shown in feed -> viewed vs swiped -> APV/loops); skip the CTR branches

STEP 1 – Impressions vs typical (Reach)
  1a  Impressions LOW, CTR and retention at/above typical
      -> Demand ceiling or competition: narrow topic, crowded topic, or limited audience     [official]
      -> Don't rework the video; give it time (late growth is common)                       [Beaupré]
      -> Next video: a broader idea, a bigger addressable audience, or a CCN bridge         [Galloway]
  1b  Impressions LOW and CTR LOW
      -> Packaging is losing the test -> Test & Compare titles/thumbnails                   [official]
      -> If still flat after changes -> topic appeals to a smaller audience                 [official]
  1c  Impressions LOW, CTR HIGH, AVD LOW
      -> Clickbait/expectation mismatch -> align the packaging with the content,
         or fix the intro so it pays off the promise in the first 30 s                      [official]
  1d  Impressions HIGH or growing, views lagging -> go to STEP 2

STEP 2 – CTR by traffic source (long-form only)
  • Low Browse/Home CTR  -> visual concept or thumbnail                                     [third-party]
  • Low Search CTR       -> title/intent mismatch                                           [third-party]
  • Low Suggested CTR    -> not competitive next to the videos it's paired with             [inference]
  • Expected: Search > subscriber surfaces > Home; CTR falls as impressions grow            [official]
    -> a falling CTR with rising clicks is HEALTHY

STEP 3 – Retention (Delivery)
  • Intro (30 s) below typical -> opening doesn't match the promise, or slow hook           [official]
  • Steep steady decay        -> pacing/structure                                          [third-party]
  • Isolated dips             -> cut or tighten that segment; move best moments earlier    [official]
  • Always benchmark against same-length videos (APV naturally falls with length)          [official]

STEP 4 – CTR x Retention matrix (vs your own medians)
                 Retention HIGH                           Retention LOW
  CTR HIGH   Breakout candidate: don't touch; make       Overpromise: fix intro/packaging alignment;
             follow-ups/series                           the system will throttle impressions
  CTR LOW    "Hidden gem": packaging problem ->          Idea/execution miss: log it, move on
             Test & Compare

STEP 5 – Audience layer
  • Subscribers watch, non-subscribers don't -> core-only topic; system learns per audience [Beaupré]
  • Many new viewers, few casual/regular gains -> one-off topic; build series that bridge
    new -> core                                                                              [CCN]

STEP 6 – Video-level vs channel-level
  • A single video down -> video-level (idea or packaging); no lasting channel penalty      [Beaupré]
  • Many videos down across topics over 28–90 days -> channel-level: check
    - seasonality
    - competition and topic saturation
    - audience fatigue (falling casual/regular share)
    - format drift
    - traffic-source mix shift (e.g., lost Browse)
```

- **Channel-level signs:** Browse share falling across uploads, subscriber CTR falling, the new casual/regular metrics trending down, and typical-performance comparisons below normal for most recent uploads. These point to idea, format or audience fit rather than a single bad thumbnail.

### Gaps
- The specific decision frameworks of **Film Booth, Creator Hooks** and **Creator Insider** were not retrieved, because WebFetch was blocked and the search budget ran out.
- No official YouTube "decision tree" exists in the retrieved material. The tree above is a synthesis.
- The date of the Tubefilter "compare with similar channels" test was not captured, and neither was whether that feature shipped.

---

## 5. How professionals optimise after publishing and iterate over the long term

### Takeaway
YouTube's native **Test & Compare** now covers **thumbnails (2024) and titles or title+thumbnail combinations (2025)**. It picks winners by **watch-time share**, and YouTube explicitly discourages manual same-video A/B swaps because traffic-source mix confounds CTR. Over the long term, professionals benchmark every video against the **channel median**, which is how outlier tools compute scores. In 2026, Studio itself is moving toward AI pattern-finding cards and possibly a native outlier metric.

### Cited Findings
- **[OFFICIAL] Thumbnail Test & Compare history:**
  - Announced **June 2023**. Limited access began in 2023 or 2024 (sources conflict).
  - Rolled out widely around **June–July 2024**.
  - Desktop Studio only. Requires **Advanced Features** (phone verification).
  - Works on public long-form videos, archived livestreams and podcast episodes. Not available for private, Made for Kids or mature videos.
  - Up to **3 thumbnails**, shown evenly; the winner is measured on **watch-time share**.
  - Tests take "a few days or up to two weeks," depending on impressions and how different the thumbnails are.
  - Outcomes reported at launch were Winner, a "Preferred" label for a slight edge, or no clear winner (the first thumbnail is kept).

  Sources: [TechCrunch, June 12, 2024](https://techcrunch.com/2024/06/12/youtube-creators-can-test-multiple-video-thumbnails), [Gigazine](https://gigazine.net/gsc_news/en/20240613-youtube-thumbnail-test-and-compare), [Social Media Today](https://www.socialmediatoday.com/news/youtube-announces-roll-out-plan-for-thumbnail-ab-testing/718647/), [ThumbnailTest](https://thumbnailtest.com/news/youtube-test-and-compare/) and [YouTube Blog – René's top five, June 14, 2024](https://blog.youtube/creator-and-artist-stories/renes-top-five-june-14-2024/).
- **[OFFICIAL] Title/combination testing** (current Help article "A/B test titles & thumbnails"):
  - Test up to **three titles, three thumbnails, or combinations**, for up to **two weeks**.
  - Outcomes are **Winner / Performed the same / Inconclusive**. For ties or inconclusive results, the first uploaded version is shown. "Higher view counts increase the likelihood of a decisive result."
  - Desktop only. Not available for Shorts, scheduled lives, Premieres, Made for Kids, age-restricted or private videos.
  - Creators can change titles or thumbnails manually after the test ends.

  Sources: [YouTube Help 16391400](https://support.google.com/youtube/answer/16391400), [SEJ – global rollout](https://www.searchenginejournal.com/youtube-title-a-b-testing-rolls-out-globally-to-creators/562571/), [RouteNote](https://routenote.com/blog/youtube-expands-a-b-title-testing/) and [ThumbnailTest](https://thumbnailtest.com/news/youtube-releases-title-test-compare/).
- **[OFFICIAL]** Do not manually swap titles or thumbnails as an A/B test, because CTR differences might come from traffic sources. Judge CTR and impressions together over the long term. — [YouTube Help 7628154](https://support.google.com/youtube/answer/7628154)
- **[OFFICIAL]** If CTR is lower *and* impressions are fewer than usual, metadata changes are recommended. If they don't help, the topic may appeal to a smaller audience. — [YouTube Help 16767369](https://support.google.com/youtube/answer/16767369)
- **[OFFICIAL]** Retention fixes: align the packaging with the content, experiment with openings, move the best moments earlier. — [YouTube Help 12942217](https://support.google.com/youtube/answer/12942217)
- **[OFFICIAL]** The retention benchmark is "typical retention" from the last 10 similar-length videos (a built-in cohort comparison). — [YouTube Help 9314415](https://support.google.com/youtube/answer/9314415)
- **[THIRD-PARTY]** Outlier-score methods used by tools:
  - Median views of recent uploads, excluding the video being scored ([Apify Outlier Finder](https://apify.com/datascoutlab/youtube-outlier-finder)).
  - Score against the median of the **last 25 videos** ([Vamos – The outlier score](https://intercom.help/getvamos/en/articles/16934858-the-outlier-score)).
  - The median is preferred over the mean because "a single viral hit can inflate the average" ([SocialCrawl](https://www.socialcrawl.dev/blog/how-many-views-is-viral)).
  - ViewStats's free outlier score is measured against the creator's **last nine uploads** ([OutlierKit's ViewStats review](https://outlierkit.com/blog/viewstats-review-features-alternatives), a competitor).
  - 1of10 reportedly defines outliers as about **10x the average**; window and statistic are unknown ([OverseerOS roundup](https://www.overseeros.com/blog/best-youtube-outlier-tools); unverified).
- **[OFFICIAL/press] 2026 in-Studio iteration aids:**
  - AI insight cards "Content Patterns," "Audience Loyalty," "Channel Summary" and "Video Summary," in the Insights redesign test from July 16, 2026 ([Net Influencer](https://www.netinfluencer.com/youtube-tests-redesigned-studio-analytics-with-ai-insight-cards/)).
  - Ask Studio AI Q&A coming to mobile ([TechCrunch, Sept 23, 2026](https://techcrunch.com/2026/09/23/youtube-releases-new-ai-features-for-creators-within-its-studio-app/)).
  - A reported Research tab with an outlier multiplier ([MiraFlow](https://miraflow.ai/blog/youtube-studio-insights-redesign-explained-2026); unverified).
- **[THIRD-PARTY] Paddy Galloway's ideation process:** a "100-to-1" (or "110-1") funnel that filters hundreds of concepts down to one. His packaging patterns include the "contradiction click" and "everything ideas." Sources: [Creator Science](https://podcast.creatorscience.com/paddy-galloway/) and [Thread Reader – PaddyG96](https://threadreaderapp.com/user/PaddyG96). The naming differs between sources.

### Inferences
- **Post-publish runbook** (my synthesis):
  - **Before publishing:** prepare 2–3 thumbnails and 2–3 titles that are genuinely different, and load them into Test & Compare at publish time. Small variations rarely give decisive results, because decisiveness depends on view volume and how different the variants are. Leave "notify subscribers" on.
  - **T+0–2 h:** watch Realtime and velocity against your typical early curve. Change nothing, since CTR here reflects subscribers.
  - **T+24 h:** check the typical-performance comparison, CTR by traffic source (only once there are about 1–2k+ impressions), and Browse/Suggested growth.
  - **T+48–72 h:** once retention has processed, check intro retention vs. typical and the dips. If CTR is low *and* impressions are low and no test is running, start Test & Compare. If CTR is high and AVD is low, fix the packaging/content mismatch.
  - **T+7 d:** log the video in an **outlier tracker**: views at day 7 ÷ median day-7 views of the last 10–25 uploads. Tag topic, format, length, packaging style and traffic mix.
  - **T+28 d and later:** check for late growth through Suggested, Search or Home resurfacing. Refresh packaging on evergreen videos using Test & Compare, never manual swaps.
- **Long-term iteration loop:**
  - Monthly or quarterly, group uploads into cohorts by topic, format and length.
  - Compare medians of: impressions per video at day 7, CTR by source, APV vs. length, watch time per impression, new-viewer share, and casual/regular trend.
  - Double down on clusters that keep producing outliers of 2x, 5x or 10x or more.
  - Use Galloway's CCN check so that bets on new viewers still bridge to the core audience.

### Gaps
- No evidence was retrieved on the measured impact of **pinned comments** or **chapters** on performance, or on official guidance for them.
- The exact global rollout date of title A/B testing was not captured. It is believed to be 2025, around the Made on YouTube announcements, but this is unverified.
- YouTube's statistical method for declaring a Test & Compare winner is not disclosed in the retrieved text.
- No retrieved study quantifies the uplift from post-publish title or thumbnail changes.

---

## 6. Third-party tools and dashboards, and what each actually measures

### Takeaway
Third-party tools see **public data only**: views over time, upload history, subscriber counts and thumbnails. They cannot see impressions, CTR or retention for channels you don't own. Their main analytical value is **velocity (VPH)** and **outlier scoring**: a video's views against its channel's recent median or average. Studio remains the only source of impressions, CTR, retention and audience segments, and YouTube itself is now testing native outlier-style research tools.

### Cited Findings
- **[THIRD-PARTY] vidIQ:**
  - **VPH / "Velocity"** (views per hour) since 2014, shown under video titles.
  - Pro identifies the highest-VPH videos and offers keyword alerts on VPH thresholds.
  - Its retention and CTR guidance blogs are quoted in Q2.

  Sources: [vidIQ Support](https://support.vidiq.com/en/articles/108672-what-is-vph-views-per-hour), [vidIQ Velocity](https://vidiq.com/blog/post/vidiq-velocity/) and [Kripesh Adwani review](https://kripeshadwani.com/vidiq-review/).
- **[THIRD-PARTY] ViewStats** (co-founded by MrBeast):
  - **Pro costs $49.99/month or $479.88/year.** One comparison lists a Business tier from $249/month.
  - Pro tools are **Outliers** (explains why some videos get many more views), **Thumbnail search** (finds similar thumbnails), **A/B thumbnail test data** (marketed as "every A/B thumbnail test ever conducted on YouTube"), **video-idea alerts** and **collections**.
  - The free tier reportedly includes a views-over-time graph, an outlier score against the last nine uploads, and thumbnail history.
  - Reliability complaints appear in competitor reviews.

  Sources: [Tubefilter](https://www.tubefilter.com/?p=180350), [Creator Handbook](https://www.creatorhandbook.net/mrbeast-launches-pro-version-of-viewstats/) and [OutlierKit review](https://outlierkit.com/blog/viewstats-review-features-alternatives) (competitor; treat criticism with caution).
- **[THIRD-PARTY] 1of10:**
  - An outlier-discovery tool, reportedly defining outliers as about 10x a channel's average. The exact formula was not verified ([OverseerOS roundup](https://www.overseeros.com/blog/best-youtube-outlier-tools)).
  - Publishes Shorts analytics guidance on viewed vs. swiped, engaged views and related metrics ([1of10 blog](https://1of10.com/blog/youtube-shorts-analytics/)).
- **[THIRD-PARTY] OutlierKit:**
  - Outlier finder ([OutlierKit tool page](https://outlierkit.com/resources/outlier-finder-tool/)).
  - Diagnostic guides, including the CTR/AVD example in Q4.
  - Competitor comparisons, written by an interested party.
- **[THIRD-PARTY] Other outlier scorers:** Apify actors use the median of recent uploads excluding the candidate video, Vamos uses the median of the last 25 videos, and TubeRecon is a Chrome extension. Sources: [Apify](https://apify.com/datascoutlab/youtube-outlier-finder), [Vamos](https://intercom.help/getvamos/en/articles/16934858-the-outlier-score) and [Chrome Web Store – TubeRecon](https://chromewebstore.google.com/detail/hbgdjglflbmbbnnobocoogjefelkgflb).
- **[THIRD-PARTY] HypeAuditor:** engagement rate over the latest 30 videos, rated against same-tier creators (Low/Average/Good/Excellent), with 30/90/180/360-day windows. Mainly an influencer-marketing and brand tool. — [HypeAuditor Help](https://help.hypeauditor.com/en/articles/6227916-what-is-youtube-engagement-rate-and-how-do-you-calculate-it)
- **[THIRD-PARTY] Modash and Scrumball:** engagement-rate calculators with tier benchmarks (Q2). Sources: [Modash](https://modash.io/youtube-engagement-rate-calculator) and [Scrumball](https://scrumball.com/tools/youtube-engagement-rate-calculator).
- **[THIRD-PARTY] Retention Rabbit:** a retention-analytics vendor that publishes the 2025 retention benchmark report (Q2). — [Retention Rabbit](https://www.retentionrabbit.com/blog/2025-youtube-audience-retention-benchmark-report)
- **[OFFICIAL/press] YouTube's own tools:** Test & Compare (Q5), the Insights AI cards, Ask Studio, and a possible Research tab with an outlier multiplier. Sources: [Net Influencer](https://www.netinfluencer.com/youtube-tests-redesigned-studio-analytics-with-ai-insight-cards/), [TechCrunch](https://techcrunch.com/2026/09/23/youtube-releases-new-ai-features-for-creators-within-its-studio-app/) and [MiraFlow](https://miraflow.ai/blog/youtube-studio-insights-redesign-explained-2026) (unverified).

### Inferences
- **Tools by job:**

  | Job | Best source | Why |
  |---|---|---|
  | Your own impressions, CTR, retention, audience segments | YouTube Studio (Analytics/Insights) | The only source of private funnel data |
  | Spotting a breakout early (yours or a competitor's) | vidIQ VPH, ViewStats views-over-time | Velocity against channel norm |
  | Idea and packaging research ("what's overperforming in my niche?") | 1of10, ViewStats Pro, OutlierKit, Spotter, possibly YouTube Research tab | Outlier scores = views ÷ channel baseline |
  | Packaging A/B | Native Test & Compare (watch-time share) | Avoids traffic-source confounding |
  | Sponsor/brand benchmarking | HypeAuditor, Modash | Engagement rate vs. tier |

- Because outlier tools differ in baseline (mean vs. median, last 9 vs. 25 uploads), outlier scores are **not comparable across tools**. The playbook should define one house formula: views at age *t* ÷ median views at age *t* of the last 10–25 uploads of the same format.

### Gaps
- What **Social Blade, Playboard, Google Trends (YouTube Search filter), TubeBuddy** and **Spotter Studio** measure and cost could not be verified this session (no successful searches or fetches). The report writer should describe them only in general terms or flag them as unverified.
- 1of10's exact outlier formula and data window could not be verified.

---

## 7. How a small channel should read low-volume data

### Takeaway
YouTube itself warns against acting on small samples or day-to-day wiggles, and says CTR is more extreme on new channels and videos with fewer than 100 views. Third-party guidance converges on waiting for about **1,000–2,000 impressions** before judging CTR, and on about **1,000 views and two weeks** before judging a video overall. Basic statistics agree: CTR measured on a few hundred impressions has error bars of several percentage points.

### Cited Findings
- **[OFFICIAL]** YouTube's guidance on small samples:
  - Avoid deciding without a substantial impression sample, and avoid reacting to small day-to-day wiggles.
  - Small CTR variations "aren't cause for immediate action." Improvements might be helpful "if a change in CTR is statistically significant."
  - New videos or channels, or videos with fewer than 100 views, can see an even wider CTR range.

  Sources: [YouTube Help – Impressions & CTR FAQ](https://support.google.com/youtube/answer/7628154) and [Decoding CTR & impressions](https://support.google.com/youtube/answer/16767369).
- **[OFFICIAL, per a third-party relay]** Videos with fewer impressions tend to show higher CTR because they reach a narrower, more loyal audience. — attributed to YouTube Help by [TubeAnalytics](https://www.tubeanalytics.net/blog/good-ctr-small-channels-2026)
- **[OFFICIAL]** Test & Compare: "Higher view counts increase the likelihood of a decisive result." Tests can run up to two weeks and end "Inconclusive." — [YouTube Help 16391400](https://support.google.com/youtube/answer/16391400)
- **[OFFICIAL]** Retention data takes 1–2 days to process ([YouTube Help 12942217](https://support.google.com/youtube/answer/12942217)). Unique viewers are available for periods up to 90 days ([YouTube Help 7577916](https://support.google.com/youtube/answer/7577916)).
- **[THIRD-PARTY]** Thresholds from 2026 guides:
  - Wait for "at least 1,000 to 2,000 impressions before reading much into a video's CTR."
  - A CTR based on 100 impressions is "noise."
  - Small-channel CTR norms are cited as 4–10% or 6–10% for channels under 1,000 subscribers.

  The search returned these from one result set, and the specific page for each could not be pinned down: [Teleprompter](https://www.teleprompter.com/blog/whats-a-good-click-through-rate-on-youtube), [vidIQ](https://vidiq.com/blog/post/6-tips-good-CTR-youtube/), [TubeBuddy – analytics for small channels](https://www.tubebuddy.com/blog/youtube-analytics-for-small-channels-which-ones-matter-and-what-they-mean/) and [TubeAnalytics](https://www.tubeanalytics.net/blog/good-ctr-small-channels-2026).
- **[THIRD-PARTY]** Wait for at least 1,000 views and two weeks before interpreting a video. Benchmark against the median of the last 10–15 similar videos. Same caveat on the specific page: see [Alan Spicer](https://alanspicer.com/youtube-analytics-explained/) and [Gyre](https://gyre.pro/blog/why-your-youtube-metrics-are-decreasing-and-what-you-can-do-about-it).
- **[OFFICIAL]** Regular viewers are "a high bar," so small regular-viewer shares are normal. — [YouTube Help 13615784](https://support.google.com/youtube/answer/13615784)

### Inferences
- **My own calculations (binomial, 95% normal approximation; not from a source).** Treat these as lower bounds on uncertainty: real impressions are not independent trials, and the traffic-source mix shifts over time. The approximation is rough when there are very few clicks (about 5 at 100 impressions × 5%).

  | Impressions | ± error if true CTR = 5% | ± error if true CTR = 10% |
  |---|---|---|
  | 100 | ±4.3 pts | ±5.9 pts |
  | 500 | ±1.9 pts | ±2.6 pts |
  | 1,000 | ±1.4 pts | ±1.9 pts |
  | 2,000 | ±1.0 pt | ±1.3 pts |
  | 10,000 | ±0.4 pt | ±0.6 pt |

- **Sample sizes needed for A/B tests (my calculation; 80% power, α = 0.05, two-sided):**
  - Telling a 4% CTR from a 5% CTR needs about **6,700 impressions per variant**.
  - Telling 5% from 7% needs about **2,200 per variant**.

  This explains why Test & Compare is often "Inconclusive" on small channels, and why small channels should test **big, conceptually different** variants rather than small tweaks.
- **Rules for small channels:**
  1. Judge medians across 5–10+ videos, not single videos.
  2. Compare videos at the same age and format.
  3. Prefer 28- or 90-day windows over daily views.
  4. Read retention (APV, intro) before CTR. Retention is measured on viewers, not impressions, and stabilises faster in relative terms.
  5. Don't change several variables at once.
  6. Expect CTR to look high early (subscriber skew) and to fall as reach grows.
  7. Treat a single unusual result as a hypothesis to retest with the next video.

### Gaps
- YouTube publishes no minimum impression count for a "reliable" CTR. The 1,000–2,000 figure is a third-party rule of thumb.
- No published analysis was found on how quickly retention metrics stabilise on low-view videos.
- YouTube's significance method for Test & Compare is not disclosed.

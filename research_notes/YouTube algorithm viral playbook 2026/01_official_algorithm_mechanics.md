# Official Mechanics of YouTube's Recommendation System (Home, Suggested/Up Next, Search, Subscriptions) — status as of Oct 2026

How this was researched, and the legend (read first). This session could not open any primary page directly. The network policy blocked youtube.com, blog.youtube, support.google.com, arxiv.org, dl.acm.org, research.google and most news sites. Tavily extract/search was over quota, and the shared WebSearch budget ran out after about 14 queries. Every claim therefore carries two tags:
- **Evidence type:** **[OFFICIAL]** is a YouTube/Google statement (Official Blog, Help Center, How YouTube Works, or YouTube staff on the record, including conference talks). **[PAPER]** is Google/YouTube-authored research (peer-reviewed or preprint). **[3P]** is third-party reporting, summary or inference.
- **Verification status:**
  - **[V]**: the content was confirmed this session from search-result excerpts of the cited page. Text in "double quotes" is as reproduced in those excerpts. **[V-2nd]** means it was confirmed only through a secondary page quoting the original.
  - **[PK]**: taken from my prior knowledge of the cited document's text. The URL is known, but the document was *not* re-opened this session, so treat the wording as approximate and re-verify before printing it as an exact quote.
  - **[HL]**: only the headline or title was seen.
- **"(older)"** marks a statement dated before 2022, with a note on whether it has been reaffirmed since.

## 1. Which signals does the system officially use, how are they weighted conceptually, and what does "the algorithm follows the audience" mean?

### Takeaway
YouTube's own named signal set is **clicks, watch time, survey responses, sharing, likes and dislikes**, interpreted through watch/search history and explicit feedback. These are combined by machine learning into a per-viewer prediction of *satisfaction* ("valued watchtime"), and the blend is tuned for viewers coming back over the long term. YouTube says no single metric is decisive. Recommendations are "pulled" for each viewer rather than "pushed" by creators; notifications are the one exception. In practice, "the algorithm follows the audience" means a video's reach is the sum of many per-viewer predictions about how *that viewer* will respond to it compared with their other options.

### Cited Findings
- **[OFFICIAL][V] (older: 15 Sep 2021; reaffirmed in substance in 2025, see Beaupré below).** Cristos Goodrow (VP of Engineering), "On YouTube's recommendation system", YouTube Official Blog. It lists the signals as clicks, watchtime, survey responses, sharing, likes and dislikes, and says they build on each other "to help inform our system about what you find satisfying." — [YouTube Blog](https://blog.youtube/inside-youtube/on-youtubes-recommendation-system/); excerpted by [recommender-systems.com](https://recommender-systems.com/news/2021/09/21/youtube-recommendation-system-case-study/) and [Ripple Room](https://rippleroomsocialclub.com/resources/how-youtube-recommendations-work)
- **[OFFICIAL][V-2nd] (older, 2021).** The same post explains why clicks were insufficient and watch time was added: "when we first incorporated watchtime into recommendations, we saw an immediate 20% drop in views". It then concludes that "not all watchtime is equal", which motivated the move to surveys. — [YouTube Blog](https://blog.youtube/inside-youtube/on-youtubes-recommendation-system/) via [Ripple Room](https://rippleroomsocialclub.com/resources/how-youtube-recommendations-work)
- **[OFFICIAL][V-2nd] (older, 2021). "Valued watchtime".** Viewers are surveyed to rate videos from one to five stars, and "only videos that you rate highly with four or five stars are counted as valued watchtime". Because most viewers never answer, YouTube trained a model to predict how each viewer *would* have answered. — [Ripple Room quoting the blog](https://rippleroomsocialclub.com/resources/how-youtube-recommendations-work); original: [YouTube Blog](https://blog.youtube/inside-youtube/on-youtubes-recommendation-system/)
- **[OFFICIAL][PK] (older, 2021).** The same post also says:
  - Likes and shares correlate with satisfaction on average, so the system predicts how likely you are to like or share further videos.
  - A dislike signals that you probably weren't satisfied.
  - "Recommendations drive a significant amount of the overall viewership on YouTube, even more than channel subscriptions or search."
  - It gives a collaborative-filtering example: if viewers who like the same tennis videos as you also enjoy jazz, you may be shown jazz.

  — [YouTube Blog](https://blog.youtube/inside-youtube/on-youtubes-recommendation-system/)
- **[3P][V]** Third-party guides repeat a claim that the system draws on "80 billion" signals. One search excerpt flagged this figure as coming from secondary sources. I recall it originates in the Goodrow post [PK], but could not verify that. — [subsub.io](https://www.subsub.io/blog/youtube-algorithm-explained-how-youtube-recommends-videos-in-2026); [vidIQ](https://vidiq.com/blog/post/understanding-youtube-algorithm/)
- **[OFFICIAL][V] (current Help Center page; its high answer ID suggests it was published around 2025, but no date was captured).** "YouTube's Recommendation System" says personalization primarily examines a viewer's **watch history** and their **interest affinity**. Only a snippet was seen. — [YouTube Help, answer 16533387](https://support.google.com/youtube/answer/16533387?hl=en)
- **[OFFICIAL][V] (2025; one source mentions a "September 2026" interview, which is unresolved).** Todd Beaupré (Senior Director, Growth & Discovery) spoke in Creator Insider interviews hosted by Rene Ritchie:
  - YouTube tries to understand "not just about the viewer's behavior and what they do, but how they feel about the time they're spending." It does this partly through direct feedback from surveys.
  - When those direct-feedback signals were added into ranking, it "actually leads to people coming back to YouTube more in the long run."
  - No metric on its own is a good indicator of value (paraphrase).

  — [Search Engine Journal, "How YouTube's Recommendation System Works In 2025"](https://www.searchenginejournal.com/how-youtubes-recommendation-system-works-in-2025/538379/); [AdOutreach summary](https://adoutreach.com/how-youtubes-algorithm-really-works-in-2025-straight-from-youtubes-director-of-growth/); [Creator Insider short, "satisfaction"](https://www.youtube.com/shorts/J9bQFujPhBE)
- **[OFFICIAL][V] (2025). Pull, not push.** Beaupré: "Most of the recommendations are more pulled for each viewer." The single exception is notifications, which go to viewers who opted in. — [Search Engine Journal](https://www.searchenginejournal.com/how-youtubes-recommendation-system-works-in-2025/538379/)
- **[OFFICIAL][V] (26 Aug 2024).** Rene Ritchie (YouTube Creator Liaison) frames the system as serving viewers rather than pushing content at them. His advice: "check your Audience tab in Analytics, see which videos are growing your audience. Make more videos like those." — [Tubefilter](https://www.tubefilter.com/2024/08/26/rene-ritchie-shorts-creator-faqs/)
- **[OFFICIAL][V] (date not captured).** Ritchie: each traffic source is important, "but it's crucial to know your viewers." — [MediaPost](https://www.mediapost.com/publications/article/401206/)
- **[3P][HL]** Headline framing of YouTube's position: "YouTube says the secret to success is not their algorithm, it's your audience." — [Yahoo](https://www.yahoo.com/entertainment/tv/articles/youtube-says-secret-success-not-230830752.html)
- **[PAPER][PK] (older, 2019). How the published ranker weights signals conceptually.** The model makes separate predictions for **engagement** tasks (clicks, time spent) and **satisfaction** tasks (likes, ratings). These are combined into one ranking score using weights tuned by hand for the best engagement plus satisfaction outcome. The result is a tuned weighted blend, not one metric. — [Zhao et al., RecSys 2019 (PDF)](https://daiwk.github.io/assets/youtube-multitask.pdf)
- **[3P][V]**
  - Third-party guides describe "Not interested" and "Don't recommend channel" as feedback that deprioritizes similar content.
  - Home leans on watch history, while Suggested centers on the video currently playing.
  - One guide says that with watch history off and no data, popular or trending content is shown. This conflicts with my unverified recollection that YouTube disables the Home feed in that case; see Gaps.

  — [subsub.io](https://www.subsub.io/blog/youtube-algorithm-explained-how-youtube-recommends-videos-in-2026); [vidIQ, Suggested](https://vidiq.com/blog/post/youtube-suggested-videos-algorithm/); [Hootsuite](https://blog.hootsuite.com/youtube-algorithm/)
- **Shorts (high level only).**
  - **[3P][V]** A third-party guide says a channel's long-form subscriber count does not carry over to how its Shorts are distributed. — [SocialPilot](https://www.socialpilot.co/youtube-marketing/youtube-algorithm)
  - **[3P][V, figure unverified]** A blog reports about a 5% click-through-rate (CTR) lift on Shorts after YouTube replaced embedding tables with Semantic IDs. — [Tullie](https://tullie.ai/blog/youtube-semantic-ids-ctr-lift)

### Inferences
- **The objective.** The officially described target is *predicted viewer satisfaction* (valued watch time). It is estimated from a chain of behaviours (impression → click → watch → like/share/dislike → predicted survey rating) and tuned against long-term return visits. Clicks, average view duration and likes are each necessary inputs, but none is "the algorithm".
- **"Follows the audience" in mechanical terms.** The system builds a model of each viewer and scores candidate videos for them. Distribution is the sum of those per-viewer decisions. The two creator levers are:
  - *who* the video appeals to, and
  - how *those* viewers respond compared with what else they could watch.
- **Comments.** Comments and replies are absent from the official 2021 signal list. This suggests they play at most a minor or indirect role. This is inferred from their absence; YouTube has not confirmed it.
- **Clickbait.** Explicit negative signals (dislikes, low predicted survey scores) and the move away from clicks put a "wins the click, loses the viewer" video at a structural disadvantage.
- **Engagement prompts.** Asking viewers to like or share fits the named signals, but the system models *satisfaction*. Engagement that doesn't reflect real satisfaction should not help over the long run.

### Gaps
- The Goodrow post, the How YouTube Works recommendations page (https://www.youtube.com/howyoutubeworks/product-features/recommendations/) and the full text of Help Center answer 16533387 could not be opened.
  - Whether these pages currently list "Not interested", "Don't recommend channel", search history, subscriptions and location as signals is recalled as yes, but unverified.
- YouTube publishes no numeric weights for any signal.
- No official statement was found on comments, replies or end screens as ranking signals.
- The date of the Beaupré interview (2025, or a later September 2026 interview) is unresolved. So is the content of a possible 2026 interview mentioned by [OutlierKit](https://outlierkit.com/resources/youtube-algorithm-updates/) (headline only).
- Recalled but unverified older Creator Academy wording: the system "pays attention to viewers", not videos. The exact phrase "the algorithm follows the audience" could not be sourced this session.
- Recalled but unverified (2023 Help Center): if watch history is off and there's no significant prior history, Home-feed recommendations are disabled.

## 2. How is a new video distributed? Core viewers first, then expansion? Relative vs absolute performance? The "first 24/48 hours", late bloomers and evergreen videos

### Takeaway
Officially there is no step where a new upload is sent to all subscribers and judged on their response. Recommendations are pulled per viewer, and only notifications push to opted-in viewers. YouTube has debunked the tactic of uploading privately and waiting 24–48 hours before publishing.

Published YouTube research shows dedicated machinery for new uploads:
- an "example age" freshness feature;
- a separate fresh-content pipeline that deliberately explores new videos with uncertainty-aware ranking to "bootstrap content with less exposure";
- models that update in near real time from early feedback.

Because ranking happens per viewer, a video is always judged against the other candidates for that viewer's attention, so performance is inherently relative. I could not verify a 2022-or-later official statement on the "first 24/48 hours" window or on videos taking off months later.

### Cited Findings
- **[OFFICIAL][V] (2025).** "Most of the recommendations are more pulled for each viewer"; notifications are the exception for viewers who opted in. — [Search Engine Journal](https://www.searchenginejournal.com/how-youtubes-recommendation-system-works-in-2025/538379/)
- **[OFFICIAL via 3P][HL] (2025/26).** "Subscribers skip 90% of uploads in their feed, YouTube director says." The article body was not retrieved. — [PPC Land](https://ppc.land/subscribers-skip-90-of-uploads-in-their-feed-youtube-director-says/)
- **[OFFICIAL via 3P][V] (date not captured).** Rene Ritchie rejected the advice to wait 24–48 hours after uploading before publishing. His reasoning (paraphrase): there is no audience behaviour to learn from until a video is public. A second write-up adds that the delay only postpones when engagement data can start accumulating. — [Search Engine Journal, "YouTube Debunks 24-48 Hour Upload Delay Recommendation"](https://www.searchenginejournal.com/youtube-debunks-24-48-hour-upload-delay-recommendation/560613/); [MyInternetMarketingTools](https://myinternetmarketingtools.com/youtubes-rene-ritchie-dispels-upload-delay-myth-for-creators/)
- **[PAPER][V] (older, 2016; the emphasis on freshness was reaffirmed by the 2023 paper below). Freshness is modelled explicitly.** "we feed the age of the training example as a feature during training. At serving time, this feature is set to zero (or slightly negative)." Without this, "the model would predict approximately the average likelihood over the training window." — [Covington et al., RecSys 2016 (PDF)](https://cseweb.ucsd.edu/classes/fa17/cse291-b/reading/p191-covington.pdf); [The Morning Paper summary](https://blog.acolyer.org/2016/09/19/deep-neural-networks-for-youtube-recommendations/)
- **[PAPER][PK] (older, 2016).** Two further lines from the same paper:
  - "We consistently observe that users prefer fresh content, though not at the expense of relevance."
  - Recommending fresh uploads has "a critical secondary phenomenon of bootstrapping and propagating viral content."

  — [Covington et al. (PDF)](https://cseweb.ucsd.edu/classes/fa17/cse291-b/reading/p191-covington.pdf)
- **[PAPER][V] (KDD 2023). A dedicated pipeline for new uploads.** "Fresh Content Needs More Attention: Multi-funnel Fresh Content Recommendation" (Jianling Wang et al.) describes:
  - a two-tower model for *coverage* paired with a sequence model that updates "in near real time" from user feedback for *relevance*;
  - "Nominated fresh candidates are then scored and ranked by systems considering prediction uncertainty to further bootstrap content with less exposure";
  - as motivation, the fact that "more than 500 hours of contents are uploaded to YouTube every minute";
  - "multiple rounds of live experiments on a commercial platform serving billion of users."

  — [arXiv 2306.01720](https://arxiv.org/pdf/2306.01720); [ACM KDD 2023](https://dl.acm.org/doi/10.1145/3580305.3599826)
- **[3P][V] (a third-party reading of the 2023 paper).** The pre-ranking stage includes a real-time Bernoulli multi-armed bandit that uses Thompson sampling to explore and exploit each fresh item and estimate its CTR. — [aman.ai](https://aman.ai/sysdes/sys-design/)
- **[PAPER][V] (WSDM 2024).** A follow-up titled "Fresh Content Recommendation at Scale: A Multi-funnel Solution and the Potential of LLMs." Its existence and title were confirmed; the content was not retrieved. — [ACM WSDM 2024](https://dl.acm.org/doi/10.1145/3616855.3635749)
- **[PAPER][V] (older, 2016). Each viewer has their own competition.** Candidate generation learns user embeddings "useful for discriminating among videos with a softmax classifier". At serving time, "choosing the N most likely classes (i.e, videos) to pass to the ranking stage can be reduced to a nearest neighbour search." The ranker then orders those candidates. — [Covington et al. (PDF)](https://cseweb.ucsd.edu/classes/fa17/cse291-b/reading/p191-covington.pdf)
- **[PAPER][PK] (older, 2016).** Further points from the Covington paper:
  - The ranking objective is "generally a simple function of expected watch time per impression."
  - "The most important signals are those that describe a user's previous interaction with the item itself and other similar items", e.g. "how many videos has the user watched from this channel? When was the last time the user watched a video on this topic?"
  - On churn: "if a user was recently recommended a video but did not watch it then the model will naturally demote this impression on the next page load."

  — [Covington et al. (PDF)](https://cseweb.ucsd.edu/classes/fa17/cse291-b/reading/p191-covington.pdf)
- **[PAPER][V] (older, 2019).** The ranker's separate "shallow tower" takes the display position (and device) to absorb position/selection bias. Its output is added to the main model's final logit, and position is set to missing at serving time. A video is therefore not credited simply for having been shown at the top. — [Zhao et al. (PDF)](https://daiwk.github.io/assets/youtube-multitask.pdf); [HackMD notes](https://hackmd.io/@nbswords/HJEGOKY7F)

### Inferences
- **Who sees a new upload first.** The first audience is likely viewers whose history predicts interest. These are disproportionately past viewers and subscribers, because "user × channel history" features are among the strongest. The fresh-content pipeline adds exploration slots on top. This is continuous, viewer-by-viewer allocation, not a fixed "test batch" that passes or fails.
- **Performance is relative by construction.** Every impression is a contest between your video and the other candidates for that viewer at that moment. The same CTR or retention can be strong for one audience and weak for another. *Implication:* benchmark against your own typical performance and against what your audience would otherwise watch, not against absolute view counts.
- **Early feedback matters but is not a cliff.** Near-real-time sequence models and bandits react quickly to early clicks and satisfaction. Even so, no source I found describes a hard 24/48-hour cutoff. Distribution continues as long as predicted per-viewer satisfaction stays competitive.
- **Impression churn.** Repeated unclicked impressions to the same viewer reduce future impressions to that viewer. Packaging that misses its audience "burns" those impressions; new packaging could change the outcome. This is inference: the official position on retitling could not be verified (see Q4 Gaps).
- **Evergreen and late-bloomer videos are architecturally plausible.** Retrieval is driven by viewer interests, and the freshness feature only *modulates* scores, so older videos can resurface whenever viewers' interests or search demand line up with them.
- **No reason to hold videos private for 24–48 hours.** Publish when ready.

### Gaps
- No verified 2022-or-later official statement on the "first 24/48 hours", videos taking off months or years later, or Analytics' "typical performance" comparisons. Creator Insider transcripts could not be reached.
- Recalled but unverified:
  - a cap on subscriber notifications per channel per 24 hours;
  - "Personalized" being the default bell setting;
  - Beaupré saying there is no fixed test audience.
- A real-time bandit paper for fresh content ("Online Matching", RecSys 2023) could not be confirmed by search.
- How the fresh-content pipeline divides impressions between brand-new and established channels is not public.

## 3. What do the Google/YouTube research papers reveal about architecture and objectives, and what do they mean for creators?

### Takeaway
Published YouTube research describes a funnel:
1. **Retrieval of candidates from a corpus of tens of millions of videos.** This has used neural two-tower retrieval, an RL (REINFORCE) candidate generator, a dedicated fresh-content pipeline and, since 2025, *generative retrieval* by Gemini-derived models over "Semantic IDs" computed from the video's content.
2. **Multi-objective ranking.** This predicts engagement *and* satisfaction separately and corrects for position bias.
3. **A tuned weighted final score.**

Over time the objective moved from CTR to expected watch time (2016), then to multi-objective engagement plus satisfaction (2019), then to survey-calibrated satisfaction and long-term return (2020 onward), and finally to LLM-based "large recommender models" (2025–26). These are research papers: apart from PLUM, which reportedly says so itself, the current production use of any of them is not confirmed.

### Cited Findings

#### Covington, Adams, Sargin — "Deep Neural Networks for YouTube Recommendations" (RecSys 2016) (older; superseded in parts)
- **[PAPER][V]** The system has two stages: candidate generation (user embeddings with a softmax over videos, served by nearest-neighbour search) and ranking. — [PDF](https://cseweb.ucsd.edu/classes/fa17/cse291-b/reading/p191-covington.pdf); [ResearchGate](https://www.researchgate.net/publication/307573656_Deep_Neural_Networks_for_YouTube_Recommendations)
- **[PAPER][V]** The ranker uses weighted logistic regression: "the positive (clicked) impressions are weighted by the observed watch time on the video. Negative (unclicked) impressions all receive unit weight." The learned odds therefore approximate expected watch time. — [PDF](https://cseweb.ucsd.edu/classes/fa17/cse291-b/reading/p191-covington.pdf); [The Morning Paper](https://blog.acolyer.org/2016/09/19/deep-neural-networks-for-youtube-recommendations/)
- **[PAPER][V]** The example-age freshness feature is described in Q2. — [PDF](https://cseweb.ucsd.edu/classes/fa17/cse291-b/reading/p191-covington.pdf)
- **[PAPER][PK]** "Ranking by click-through rate often promotes deceptive videos that the user does not complete ("clickbait") whereas watch time better captures engagement." — [PDF](https://cseweb.ucsd.edu/classes/fa17/cse291-b/reading/p191-covington.pdf)
- **[PAPER][PK]** Other details from the paper:
  - Candidate generation narrows millions of videos to hundreds.
  - The strongest ranking features are a user's past interactions with the channel or topic.
  - Unwatched recommendations are demoted ("churn").
  - "Search history is treated similarly to watch history - each query is tokenized into unigrams and bigrams and each token is embedded."
  - The model is trained to predict the user's *next* watch, because viewing is asymmetric: people typically start with broadly popular items in a genre before narrowing into niches.

  — [PDF](https://cseweb.ucsd.edu/classes/fa17/cse291-b/reading/p191-covington.pdf)

#### Zhao et al. — "Recommending What Video to Watch Next: A Multitask Ranking System" (RecSys 2019, pp. 43–51) (older; its engagement-plus-satisfaction framing matches Beaupré's 2025 statements)
- **[PAPER][V]** The paper extends Wide & Deep with a Multi-gate Mixture-of-Experts (MMoE). Each objective has its own gating network that decides which shared experts to use, which accommodates potentially conflicting objectives. — [PDF](https://daiwk.github.io/assets/youtube-multitask.pdf); [Speaker Deck](https://speakerdeck.com/alpicola/recommending-what-video-to-watch-next-a-multitask-ranking-system)
- **[PAPER][V]** A shallow tower for selection bias (e.g. position bias) takes position and device features. Its output is added to the final logit, and position is "missing" at serving time. Secondary notes report 10% dropout on position during training, and a slide deck says the tower applies to the engagement task. — [PDF](https://daiwk.github.io/assets/youtube-multitask.pdf); [HackMD](https://hackmd.io/@nbswords/HJEGOKY7F); [Speaker Deck](https://speakerdeck.com/alpicola/recommending-what-video-to-watch-next-a-multitask-ranking-system)
- **[PAPER][PK]** The objectives fall into two groups: **engagement** (clicks, degree of engagement such as watch time) and **satisfaction** (e.g. liking a video, leaving a rating). The final score is a weighted combination with manually tuned weights. The task setting is ranking "what video to watch next" given the video currently playing (Up Next/Suggested). — [PDF](https://daiwk.github.io/assets/youtube-multitask.pdf)

#### Chen et al. — "Top-K Off-Policy Correction for a REINFORCE Recommender System" (WSDM 2019, pp. 456–464; arXiv 1812.02353) (older)
- **[PAPER][V]** Results were demonstrated "through a series of simulations and multiple live experiments on YouTube." — [ResearchGate](https://www.researchgate.net/publication/329464919_Top-K_Off-Policy_Correction_for_a_REINFORCE_Recommender_System)
- **[PAPER][PK]** The paper treats candidate generation as reinforcement learning (a REINFORCE policy gradient) over an action space of millions of videos. It corrects for the bias of learning from logs produced by earlier recommenders (off-policy correction), with a "top-K" correction because K items are shown at once. The reward is based on user engagement. — [arXiv 1812.02353](https://arxiv.org/abs/1812.02353)
- **[3P][V, numbers unverified]** A seminar slide summary reports that the YouTube experiment used ViewTime as the metric:
  - no significant ViewTime difference overall, but video views +0.53%;
  - ViewTime −0.52% without weight capping;
  - +0.15% with K=8.

  Do not cite these numbers without checking the paper. — [SlideShare](https://www.slideshare.net/slideshow/topk-offpolicy-correction-for-a-reinforce-recommender-system/237136380)

#### Yi et al. — "Sampling-Bias-Corrected Neural Modeling for Large Corpus Item Recommendations" (RecSys 2019) (older)
- **[PAPER][V]** "We then apply the sampling-bias-corrected modeling approach to build a large scale retrieval system called Neural Deep Retrieval (NDR) for YouTube recommendations. The system is deployed to retrieve personalized suggestions from a corpus of tens of millions videos."
  - The paper addresses in-batch softmax bias, which "could severely restrict model performance, particularly in the case of power-law distribution."
  - It estimates item frequency from streaming data.
  - It reports improved recommendation quality in live A/B tests.

  — [Google Research](https://research.google/pubs/sampling-bias-corrected-neural-modeling-for-large-corpus-item-recommendations/)
- **[PAPER][V] (2025).** A later paper says this "logQ correction" has become standard practice in industrial two-tower retrieval, including at Google. — [arXiv 2507.09331](https://arxiv.org/html/2507.09331v2)
- **Author-order conflict.** One search excerpt said Google's page lists Ji Yang first. My recollection [PK] is that the RecSys listing has Xinyang Yi first. Verify before citing as "Yi et al."

#### Christakopoulou et al. — "Deconfounding User Satisfaction Estimation from Response Rate Bias" (RecSys 2020) (older)
- **[PAPER][V]**
  - What users *do* (engagement) does not always match what they *say* in surveys (satisfaction).
  - Users "are more likely to respond to a survey when they will respond that they are more satisfied."
  - The authors train a response-propensity model and weight the satisfaction model by its inverse.
  - This improved satisfaction estimates for the slices of users least likely to respond, and held up in live A/B experiments.
  - The excerpts call the system "industrial" without naming YouTube. My recollection [PK] is that the authors are on Google's YouTube recommendations team.

  — [Google Research](https://research.google/pubs/deconfounding-user-satisfaction-estimation-from-response-rate-bias/); [ACM PDF](https://dl.acm.org/doi/pdf/10.1145/3383313.3412208)

#### Wang et al. — "Fresh Content Needs More Attention: Multi-funnel Fresh Content Recommendation" (KDD 2023), and the WSDM 2024 follow-up
- **[PAPER][V]** The coverage plus relevance pipelines and the uncertainty-aware bootstrapping of less-exposed content are covered in Q2. — [arXiv 2306.01720](https://arxiv.org/pdf/2306.01720); [ACM WSDM 2024](https://dl.acm.org/doi/10.1145/3616855.3635749)

#### PLUM — "Adapting Pre-trained Language Models for Industrial-scale Generative Recommendations" (preprint 2025; listed at the ACM Web Conference 2026, pp. 8093–8104)
- **[PAPER][V, from excerpts]**
  - **Three stages:** Semantic IDs for items; continued pre-training of a language model on user–item behaviour data; and fine-tuning for *generative retrieval*, in which the model predicts the Semantic IDs of the videos a user is likely to watch next.
  - **Results:** it reportedly outperformed "a heavily optimized production model" that relies on large embedding tables, and is described as in production for YouTube recommendations.
  - **Scale:** up to a Mixture-of-Experts model with more than 900M activated parameters (about 4.2B total).

  — [ResearchGate](https://www.researchgate.net/publication/396373037_PLUM_Adapting_Pre-trained_Language_Models_for_Industrial-scale_Generative_Recommendations)
- **[PAPER][V, from excerpts] (June 2026).** "Token Factory: Efficiently Integrating Diverse Signals into Large Recommendation Models" describes a PLUM model derived from a 210M-parameter MoE variant of a Gemini decoder. This may be a different variant from the one above; the sources don't reconcile them. — [arXiv 2606.19635](https://arxiv.org/pdf/2606.19635)

#### "Teaching Gemini to Speak YouTube: Adapting LLMs for Video Recommendations to 2B+ DAU" — Devansh Tandon (YouTube), AI Engineer conference talk (2025, 23 min)
- **[OFFICIAL talk][V via 3P summaries]**
  - The talk covers Semantic ID creation, model adaptation (continued pre-training of Gemini) and generative video retrieval using prompts.
  - A third-party report says video features (title, description, transcript, audio, frames) are combined into embeddings, then quantized into hierarchical tokens running from broad (e.g. music, gaming, sports) to specific.

  — [Class Central listing](https://www.classcentral.com/course/youtube-teaching-gemini-to-speak-youtube-adapting-llms-for-video-recommendations-to-2b-dau-devansh-tandon-468391); [ZenML LLMOps summary](https://www.zenml.io/llmops-database/large-recommender-models-adapting-gemini-for-youtube-video-recommendations); [Dev.to (contains speculative claims, so use cautiously)](https://dev.to/claudiuspapirus/how-google-taught-gemini-to-speak-youtube-the-rise-of-semantic-ids-1518)
- **[3P][V, unverified figure]** About a 5% CTR lift on Shorts from replacing embedding tables with Semantic IDs. — [Tullie](https://tullie.ai/blog/youtube-semantic-ids-ctr-lift)
- **[3P][V]** A creator blog makes claims about a "2026 Gemini update", such as every video getting a "vibe" summary. These are speculative and should not be relied on. — [Masculine Synergy](https://masculinesynergy.com/youtube-algorithm-2026-gemini-update-guide/)

### Inferences (plain-English creator implications, paper by paper)
- **Covington 2016.**
  - Packaging that earns clicks but not watch time loses in a ranker built on expected watch time *per impression*.
  - Impressions that a given viewer repeatedly ignores are demoted for that viewer.
  - A viewer's history with *your channel* is one of the strongest reasons your next video is shown to them, so returning viewers compound.
  - New uploads get a freshness lift, "not at the expense of relevance".
  - Viewers move from broad, popular entry points to niches, so a broad "gateway" video can feed deeper niche videos.
  - What people *search* also shapes their Home recommendations.
- **Zhao 2019.**
  - Satisfaction (likes, ratings and, by extension, predicted survey scores) is a separate prediction target from clicks and watch time. A video that is watched but disliked or poorly rated is penalised.
  - Position-bias correction means YouTube tries to learn a video's *intrinsic* appeal rather than crediting placement.
- **Chen 2019 (REINFORCE).** Candidate generation was optimised as long-horizon reinforcement learning, correcting for earlier systems' biases. Conceptually, it can recommend items that previous systems under-exposed [PK]. This counts against the idea that "only already-popular videos get recommended".
- **Yi 2019 (two-tower retrieval with logQ correction).** Correcting for popularity is built in, so niche videos can still be retrieved for well-matched viewers. Being the most popular is not a prerequisite for entering a viewer's candidate pool.
- **Christakopoulou 2020 (survey debiasing).**
  - Survey-based satisfaction is a measured, statistically debiased quantity.
  - Satisfaction is estimated for viewers who never answer surveys, so it can't be gamed by getting fans to answer them.
  - The aim is to predict how *typical* viewers would rate the experience.
- **Wang 2023 (fresh pipeline).** New uploads get deliberate, uncertainty-aware exploration, and early viewer feedback updates the models in near real time. A new video's earliest viewers matter, and the system is built to give low-exposure content a chance.
- **PLUM, Semantic IDs and Gemini (2025–26).**
  - The video's *content itself* (title, description, transcript, audio, frames) determines which "semantic neighbourhood" it sits in. That placement starts before any engagement data exists.
  - Clear, consistent topical signals in what is *said and shown*, not just in metadata, should help the system place a new upload near the right audience.
  - A sharp change of niche moves new uploads into a different neighbourhood, so the existing audience may not be matched to them.

### Gaps
- None of the papers could be opened, so [PK] details need verification against the PDFs.
- Relevant YouTube papers I believe exist but could not confirm this session (search either didn't find them or the budget ran out):
  - "Values of User Exploration in Recommender Systems" (RecSys 2021)
  - "Surrogate for Long-Term User Experience in Recommender Systems" (KDD 2022; one search did **not** find it)
  - "Reward Shaping for User Satisfaction in a REINFORCE Recommender" (2022)
  - "Online Matching: A Real-time Bandit System for Large-scale Recommendations" (RecSys 2023)
  - "Learning from Negative User Feedback and Measuring Responsiveness for Sequential Recommenders" (RecSys 2023)
  - "Better Generalization with Semantic IDs" (RecSys 2024)
  - "Long-Term Value of Exploration" (WSDM 2024)
- Production status: YouTube does not confirm which research systems run today. The only exception is PLUM, which reportedly says so itself according to excerpts.
- The commonly repeated claim that REINFORCE was "YouTube's most successful launch in two years" was not verified.

## 4. What has YouTube officially said about common creator beliefs? (Myth vs. fact)

### Takeaway
Within this session's limits I could verify YouTube's position on these beliefs:
- there is no push of every upload to all subscribers;
- "wait 24–48 hours before publishing" is wrong;
- CTR or raw watch time is not the whole story;
- tags matter little (PK);
- excessive hashtags are ignored (PK);
- borderline content is *demoted*, not boosted;
- "make more of what grows your audience" is the official advice;
- most "shadowban" complaints are audience shifts (low-authority source).

Published research also supports deliberate exploration for new and low-exposure content. Many other popular topics could **not** be verified this session: upload time, frequency, breaks, video length, deleting videos, unlisted-then-public, dead subscribers, sub-to-view ratio, small channels/Hype, niche changes, retitling/Test & Compare, end screens, comments and Premieres. They are listed in Gaps with my unverified recollection of YouTube's position.

### Cited Findings

Myth-vs-fact table (only rows with a source; status shown):

| # | Popular belief | YouTube's position | Who / where | Date | Evidence | Status |
|---|---|---|---|---|---|---|
| 1 | "YouTube sends a new upload to all subscribers first and judges it by their reaction" | Recommendations are "more pulled for each viewer"; only notifications push, and only to viewers who opted in. **Busted.** | Todd Beaupré, via [SEJ](https://www.searchenginejournal.com/how-youtubes-recommendation-system-works-in-2025/538379/) | 2025 | OFFICIAL (reported) | V |
| 2 | "Upload private/unlisted and wait 24–48 h before publishing" | Rejected: nothing to learn until the video is public, so the delay only postpones data. **Busted.** | Rene Ritchie, via [SEJ](https://www.searchenginejournal.com/youtube-debunks-24-48-hour-upload-delay-recommendation/560613/) | date not captured | OFFICIAL (reported) | V |
| 3 | "CTR is the algorithm" | Clicks are one of six named signals. Adding watch time caused "an immediate 20% drop in views". Reaffirmed in 2025: no single metric indicates value. **Busted.** | Goodrow, [YouTube Blog](https://blog.youtube/inside-youtube/on-youtubes-recommendation-system/); Beaupré, [SEJ](https://www.searchenginejournal.com/how-youtubes-recommendation-system-works-in-2025/538379/) | 2021 (older); reaffirmed 2025 | OFFICIAL | V / V-2nd |
| 4 | "Maximise raw watch time at any cost" | "not all watchtime is equal": only watch time rated 4–5★ in surveys counts as "valued watchtime", with ratings predicted for non-respondents. **Nuanced / busted.** | Goodrow, [YouTube Blog](https://blog.youtube/inside-youtube/on-youtubes-recommendation-system/) via [Ripple Room](https://rippleroomsocialclub.com/resources/how-youtube-recommendations-work) | 2021 (older); satisfaction focus reaffirmed 2025 | OFFICIAL | V-2nd |
| 5 | "Tags are key to ranking" | Tags "play a minimal role" except for commonly misspelled terms; title, thumbnail and description matter more. Search does use tags as one relevance input, alongside title, description and video content. **Mostly busted.** | [Help: tags](https://support.google.com/youtube/answer/146402); [Help: how search works](https://support.google.com/youtube/answer/16090438?hl=en) | Help pages undated (evergreen) | OFFICIAL | PK (tags page) / V (search page) |
| 6 | "More hashtags = more reach" | More than 60 hashtags means YouTube ignores *all* hashtags on the video; misleading hashtags can lead to removal. **Busted.** | [Help: hashtags](https://support.google.com/youtube/answer/6390658) | undated (evergreen) | OFFICIAL | PK |
| 7 | "Subscribers guarantee views" | A YouTube director says subscribers skip about 90% of uploads in their feed; distribution is pulled per viewer. **Busted.** | [PPC Land](https://ppc.land/subscribers-skip-90-of-uploads-in-their-feed-youtube-director-says/) | 2025/26 | OFFICIAL (reported) | HL (+V for pull) |
| 8 | "YouTube shadowbans channels" | Ritchie says most drops reflect audience shifts, not hidden penalties. A separate view-count issue linked to ad-blocking software was "largely resolved". **No confirmation of shadowbans; low-authority source.** | Ritchie, via [SigmaStory](https://sigmastory.in/youtube-liaison-rene-ritchie-reveals-truth-behind-shadowbans-and-ai-rules/) | c. 2025 | OFFICIAL via low-authority 3P | V (low confidence) |
| 9 | "YouTube boosts sensational/borderline content because it's engaging" | Reported a 70% drop in watch time of borderline content from non-subscribed recommendations (US, 2019) and set a goal of keeping such views below 0.5%. **Busted per YouTube**, but not independently verified ([arXiv 2204.10921](https://arxiv.org/pdf/2204.10921)). | [Four Rs blog](https://blog.youtube/inside-youtube/the-four-rs-of-responsibility-raise-and-reduce/); [How YouTube Works](https://www.youtube.com/intl/en_us/howyoutubeworks/our-commitments/managing-harmful-content/) | 3 Dec 2019 (older); restated on How YouTube Works | OFFICIAL | V |
| 10 | "You have to make content for the algorithm" | "check your Audience tab in Analytics, see which videos are growing your audience. Make more videos like those." | Ritchie, via [Tubefilter](https://www.tubefilter.com/2024/08/26/rene-ritchie-shorts-creator-faqs/) | 26 Aug 2024 | OFFICIAL (reported) | V |
| 11 | "New or low-exposure videos never get a chance" | YouTube research describes a fresh-content pipeline that ranks "considering prediction uncertainty to further bootstrap content with less exposure". **Contradicted by research; not an official policy statement.** | [Wang et al., KDD 2023](https://arxiv.org/pdf/2306.01720) | 2023 | PAPER | V |

Supporting detail:
- **[OFFICIAL][PK]** The tags Help page says: "Your video's title, thumbnail, and description are more important pieces of metadata for your video's discovery. Tags can be useful if content in your video is commonly misspelled. Otherwise, tags play a minimal role in helping viewers find your video." — [YouTube Help](https://support.google.com/youtube/answer/146402)
- **[3P][HL]** A Search Engine Journal myth-busting article based on YouTube's Growth team exists; its contents were not retrieved. — [SEJ, "YouTube Algorithm Myths Debunked: Insights From The Growth Team"](https://www.searchenginejournal.com/youtube-algorithm-myths-debunked-insights-from-the-growth-team/510091/)
- **[3P][HL]** A Ritchie explainer video exists but was not retrieved. — ["All About the YouTube Algorithm – with Rene Ritchie"](https://www.youtube.com/watch?v=Ng2miYe_oDI)

### Inferences (consolidated creator action list, strongest evidence first)
1. **Package honestly for the viewer you want.** A click that doesn't turn into satisfying viewing is explicitly discounted (Covington's clickbait note; Goodrow's 20% view drop; valued watchtime). *Strong: official plus paper.*
2. **Engineer a "4–5 star" experience.** Deliver the packaging's promise early, cut filler and end strong. Satisfaction is predicted for *every* viewer, not just those who answer surveys. *Strong.*
3. **Build returning viewers.** A viewer's history with your channel is among the strongest ranking features [PK], and YouTube tunes for long-term return. *Strong-moderate.*
4. **Don't count on subscribers.** Recommendations are pulled per viewer, notifications reach only opted-in viewers, and subscribers reportedly skip about 90% of uploads. *Moderate.*
5. **Publish when ready.** Holding a video private for 24–48 hours buys nothing. *Official.*
6. **Judge performance relatively.** Compare against your own typical performance and your audience's alternatives, not absolute views. *Inference from architecture.*
7. **Make the topic legible in the content itself.** Semantic IDs built from title, description, transcript, audio and frames place a new video before any engagement data exists, so consistent topics help cold-start. *Inference from 2025–26 papers and talk.*
8. **For search,** put the query's words and meaning in the title, description and spoken content. Tags are minor; there's no point stuffing hashtags. *Official.*
9. **Avoid borderline or sensational treatments** if you want reach from non-subscribers through recommendations. *Official.*
10. **Use the Audience tab** to find the videos that grow your audience, then make more like them. *Official.*
11. **Re-package underperforming videos.** If an impression is ignored, it is demoted for that viewer, so changing packaging is a rational experiment. *Inference; YouTube's stance is unverified.*

### Gaps
The following official positions could not be verified this session. Each line is my recollection of YouTube's stance. Do **not** publish any of it as fact without a source.
- **Upload time:** no algorithmic "best time"; publishing when your audience is active mainly affects early notification and subscription-feed views.
- **Upload frequency or consistency:** no direct algorithmic reward for uploading more; quality and viewer satisfaction matter more.
- **Taking breaks:** YouTube says there's no algorithmic penalty, but audiences may need to be re-engaged. I believe there was a Creator Insider analysis on this.
- **Video length:** no preferred length; the system optimises for satisfaction.
- **Deleting videos:** doesn't "hurt the channel", though you lose that video's future views. Re-uploading duplicates can conflict with YouTube's reused/repetitive-content and spam policies.
- **Unlisted or private, then public:** not penalised; the video is treated as published when it goes public. This is consistent with verified row 2.
- **"Dead" or inactive subscribers, and sub-to-view ratio:** not ranking inputs, and they don't hurt.
- **Small or new channels:** can be recommended. The Hype feature (channels under about 500K subscribers) is an added discovery surface; no details were retrieved.
- **Changing niche:** possible; the system finds the new audience, but there may be a dip.
- **Re-titling or re-thumbnailing old videos:** allowed and can help. Test & Compare reportedly picks winners by **watch-time share** rather than CTR; title testing may have been added around 2025. All unverified.
- **End screens and cards:** drive viewers to your other videos; no recalled statement that they boost ranking.
- **Comments, replies and likes:** likes are a named signal (V). Comments are not in the 2021 list; I recall no official claim that replying boosts ranking.
- **Premieres:** no recalled statement of a ranking advantage.
- **Notification rules:** a per-channel cap per 24 hours, and "Personalized" vs "All" bell settings. Unverified.
- **Shorts vs long-form:** YouTube has reportedly said Shorts and long-form are recommended separately, so posting Shorts doesn't hurt long-form. Shorts view counting reportedly changed on 31 March 2025. Both unverified here, and left to the Shorts researcher.

## 5. How does YouTube define and measure "satisfaction", how does it handle clickbait, and what is "authoritative" ranking and demotion?

### Takeaway
YouTube defines satisfaction as **"valued watchtime"**: watch time that viewers rate 4–5★ in on-platform surveys, predicted by a model for everyone who doesn't answer. It is combined with likes, dislikes and shares, and validated by whether viewers come back over the long run. YouTube's research corrects survey data for response bias, and its rankers predict satisfaction separately from engagement.

Clickbait is counteracted by design: ranking moved from CTR to expected watch time per impression, and later to satisfaction. For news and information-sensitive topics, YouTube "raises" authoritative sources and "reduces" borderline content and harmful misinformation, specifically in **non-subscribed recommendations**. It reports a 70% drop in watch time for that content and a target of below 0.5% of views (YouTube's own, unaudited figures).

### Cited Findings
- **[OFFICIAL][V-2nd] (older, 2021).** Surveys rate videos 1–5★; "only videos that you rate highly with four or five stars are counted as valued watchtime"; a model predicts survey responses for all viewers. — [YouTube Blog](https://blog.youtube/inside-youtube/on-youtubes-recommendation-system/) via [Ripple Room](https://rippleroomsocialclub.com/resources/how-youtube-recommendations-work)
- **[OFFICIAL][V] (2025).** YouTube aims to understand "how they feel about the time they're spending" through surveys. Adding those signals to ranking "leads to people coming back to YouTube more in the long run." — [Search Engine Journal](https://www.searchenginejournal.com/how-youtubes-recommendation-system-works-in-2025/538379/)
- **[PAPER][V] (older, 2020).** Engagement doesn't always match survey satisfaction. Satisfied users are more likely to respond, so YouTube's researchers correct with inverse-propensity weighting and validated the result in live A/B tests. — [Google Research](https://research.google/pubs/deconfounding-user-satisfaction-estimation-from-response-rate-bias/)
- **[PAPER][PK] (older, 2019).** The ranker has separate satisfaction objectives (e.g. likes, ratings) alongside engagement objectives. — [Zhao et al. (PDF)](https://daiwk.github.io/assets/youtube-multitask.pdf)
- **[PAPER][PK] (older, 2016). Clickbait:** "Ranking by click-through rate often promotes deceptive videos that the user does not complete ("clickbait") whereas watch time better captures engagement." — [Covington et al. (PDF)](https://cseweb.ucsd.edu/classes/fa17/cse291-b/reading/p191-covington.pdf)
- **[OFFICIAL][V-2nd] (older, 2021). Clickbait history:** moving from clicks to watch time caused "an immediate 20% drop in views". — [YouTube Blog](https://blog.youtube/inside-youtube/on-youtubes-recommendation-system/) via [Ripple Room](https://rippleroomsocialclub.com/resources/how-youtube-recommendations-work)
- **[OFFICIAL][V] (older: 3 Dec 2019; restated on How YouTube Works).** "The Four Rs of Responsibility, Part 2: Raising authoritative content and reducing borderline content and harmful misinformation" reports:
  - a 70% average drop in watch time of borderline content "coming from non-subscribed recommendations" in the US;
  - methodology: "Based on the 28-day average from 9/17/19 - 10/14/19, compared to when we first started taking action on this type of content in January 2019";
  - borderline content is "a fraction of 1%" of what's watched.

  The framework is the "Four Rs": remove, raise, reward and reduce. — [YouTube Blog](https://blog.youtube/inside-youtube/the-four-rs-of-responsibility-raise-and-reduce/); [Tubefilter](https://www.tubefilter.com/2019/12/03/youtube-borderline-content-watch-time-drop/)
- **[OFFICIAL][V] (How YouTube Works; page date unknown).** Restates the 70% figure and sets a goal of keeping views of borderline content from non-subscribed recommendations **below 0.5%**. — [How YouTube Works: managing harmful content](https://www.youtube.com/intl/en_us/howyoutubeworks/our-commitments/managing-harmful-content/)
- **[OFFICIAL][PK] (older: 25 Jan 2019).** YouTube began reducing recommendations of borderline content and harmful misinformation. Its examples were a phony miracle cure for a serious illness, flat-earth claims, and blatantly false claims about historic events like 9/11, affecting under 1% of content. The change affects *recommendations*, not availability: such videos may still appear for subscribers and in search. — [YouTube Blog (URL recalled)](https://blog.youtube/news-and-events/continuing-our-work-to-improve/)
- **[OFFICIAL][PK] (older, 2021).** Goodrow: borderline consumption that comes from recommendations is significantly below 1%. Demoting "salacious or tabloid-type" content *increased* watch time by about 0.5% over about 2.5 months. — [YouTube Blog](https://blog.youtube/inside-youtube/on-youtubes-recommendation-system/)
- **[OFFICIAL via 3P][V].** Search "quality" signals identify "which channels demonstrate expertise, authoritativeness, and trustworthiness on a given topic." — [SEO Sherpa](https://seosherpa.com/youtube-search-features/), summarising [YouTube Help](https://support.google.com/youtube/answer/16090438?hl=en)
- **[3P][V] Independent scrutiny:**
  - The 70% claim "has not been independently evaluated using behavioral data". — [arXiv 2204.10921](https://arxiv.org/pdf/2204.10921)
  - Because YouTube defines the category itself, such claims are nearly impossible to confirm. — [UPenn essay](https://amc.sas.upenn.edu/essay-do-not-recommend-reduction)
  - A 50% figure from the same period is unverified (search excerpt).

### Inferences
- **Satisfaction is three-layered:**
  1. explicit feedback (survey stars, likes, dislikes, shares, "not interested");
  2. model-predicted feedback for everyone else;
  3. long-term return.

  A video can win short-term engagement and still lose if it predicts low ratings.
- **Misleading packaging is self-defeating** under these objectives. Satisfaction tasks, dislikes and impression churn compound against it.
- **Borderline demotion targets non-subscribed recommendations,** which is exactly the growth surface. Creators in news, health or contentious niches should expect authoritative channels to be favoured on information-sensitive queries and shelves.
- **Sensationalism doesn't pay.** YouTube claims that demoting tabloid-style content *raised* total watch time, so it has little incentive to reward sensational treatments.

### Gaps
- The current Help Center text on "authoritative" sources, news shelves (e.g. Top news / Breaking news) and which topics count as information-sensitive was not retrieved.
- Recalled but unverified:
  - YouTube's December 2024 announcement (India first) on enforcing against "egregious clickbait" titles and thumbnails;
  - Test & Compare choosing thumbnail or title winners by watch-time share.
- No 2022-or-later updated borderline-content metrics were found.
- The extent of "limited" distribution for age-restricted or limited-features content was not retrieved.

## 6. How does Search ranking differ from Browse (Home) and Suggested (Up Next)?

### Takeaway
YouTube's own Help page says Search ranks on three elements: **relevance** (how well the title, tags, description and video content match the query), **engagement** (signals such as watch time *for that query*) and **quality** (channels showing expertise, authoritativeness and trustworthiness on the topic). Their weights vary by search type and are unpublished.

Browse (Home) is viewer-centric personalization driven by watch history and "interest affinity". Suggested/Up Next is conditioned on the video currently playing. Both optimize predicted satisfaction rather than matching a query.

### Cited Findings
- **[OFFICIAL][V] (current Help page; date not captured).** "How YouTube search works" covers three elements:
  - **relevance:** "how well the title, tags, description, and video content fit the query";
  - **engagement:** "the watch time of a particular video for a particular query", used to judge whether other users find the video relevant to that query;
  - **quality:** the importance of each element varies by search type.

  — [YouTube Help, answer 16090438](https://support.google.com/youtube/answer/16090438?hl=en)
- **[OFFICIAL via 3P][V].** Quality is described as signals identifying "which channels demonstrate expertise, authoritativeness, and trustworthiness on a given topic." — [SEO Sherpa](https://seosherpa.com/youtube-search-features/)
- **[3P][V].**
  - YouTube hasn't published how much weight each element carries, so exact percentages "should be viewed with suspicion."
  - One guide says links from other websites are not among the ranking elements.

  — [Search Engine Journal, YouTube SEO](https://www.searchenginejournal.com/youtube-seo-video-optimization/260757/); [Digitizer](https://digitizer.rs/en/news-stories/how-does-youtube-search-work/)
- **[OFFICIAL][V].** Home personalization "primarily" examines watch history and interest affinity. — [YouTube Help, answer 16533387](https://support.google.com/youtube/answer/16533387?hl=en)
- **[3P][V].** Home leans on watch history, while Suggested centers on the currently playing video. — [vidIQ](https://vidiq.com/blog/post/youtube-suggested-videos-algorithm/); [subsub.io](https://www.subsub.io/blog/youtube-algorithm-explained-how-youtube-recommends-videos-in-2026)
- **[PAPER][PK].**
  - Zhao 2019 ranks "what video to watch next" given the video being watched, i.e. Suggested. — [PDF](https://daiwk.github.io/assets/youtube-multitask.pdf)
  - Covington 2016 feeds *search tokens* into recommendation models, so search behaviour shapes Home. — [PDF](https://cseweb.ucsd.edu/classes/fa17/cse291-b/reading/p191-covington.pdf)

### Inferences
- **To win Search:**
  1. Match the query's wording and meaning in the title, description and *spoken content*. Tags are minor.
  2. Satisfy *that query's* intent, because watch time is judged per query.
  3. Build consistent topical depth, which plausibly feeds "quality/authority".
- **To win Browse/Home:** be the best predicted 4–5★ choice for viewers whose watch history resembles your audience's.
- **To win Suggested:** be the natural *next* watch after popular videos in your niche, through follow-ups, series, responses and complementary angles.
- **Search builds Browse.** Search demand feeds recommendation, because search tokens are personalization features, so search-optimized videos can seed later Home and Suggested traffic.

### Gaps
- The full Help page could not be opened, so the following were not retrieved:
  - how personalised search results are (recalled: personalised by search and watch history);
  - the statement on paid placement (recalled: payment does not buy organic search ranking);
  - news and authoritative handling in search;
  - differences for logged-out users.
- The How YouTube Works search page (https://www.youtube.com/howyoutubeworks/product-features/search/) could not be retrieved.

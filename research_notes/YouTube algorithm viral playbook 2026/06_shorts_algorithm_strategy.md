# YouTube Shorts: Recommendation System, Virality Tactics and Shorts-to-Long-Form Conversion (state as of 27 Oct 2026)

Source tags: **[OFFICIAL]** = YouTube/Google statement, YouTube Blog, Help Center, or YouTube staff (Rene Ritchie, Todd Sherman, Neal Mohan). **[NEWS]** = press/trade coverage of an official announcement. **[DATA]** = third-party dataset or study (methods usually unaudited). **[CREATOR]** = a creator's own account. **[ANALYST]** = strategist or SEO-blog claim. Dates are publication or effective dates. Pre-2025 items are marked "(older)".

**How this was researched:** This session's network policy blocked direct page fetches from blog.youtube, support.google.com, youtube.com, techcrunch.com, socialmediatoday.com and creaticalc.com. Tavily was over quota. The shared web-search budget ran out partway through the research. So every finding below comes from search-engine extracts of the linked pages, not from reading the pages themselves. Short quotes are given as the extracts returned them. Spot-check them before quoting verbatim.

Items labelled "Lead (unverified)" in the Gaps sections are background knowledge given to the writer as pointers for follow-up. They are not findings and should not be published without verification.

---

## Q1. How does the Shorts feed rank and test content? Why do Shorts surge weeks or months later? How is Shorts ranking separated from long-form?

### Takeaway
- **Official ranking signal.** The only Shorts ranking input YouTube describes concretely is the viewer's choice to watch or swipe away. In Studio this metric is now called "Stayed to watch"; it launched as "Viewed (vs. swiped away)".
- **Seed-and-expand.** The popular "small test audience, then expand" model is a secondhand paraphrase of a Todd Sherman Q&A from 23 Aug 2023. YouTube publishes no Shorts signal weights or thresholds.
- **Separation from long-form.** Two official lines are verifiable:
  - Recommendations rely mainly on data from the same traffic source (Apr 2024).
  - YouTube has "not seen evidence" that Shorts hurt long-form.
- **Newest change.** Since 1 Oct 2026, Shorts recommendations explicitly favour original content over re-uploads.

### Cited Findings
- **[OFFICIAL] Definition of the swipe metric.** YouTube Help defines "Stayed to watch" as "the percentage of times that viewers viewed your Shorts versus swiped away." A Shorts-specific Help page describes it as the share of times viewers "stayed to watch past the initial seconds of a Short." The search extraction noted that the wording differs slightly between pages. — [YouTube Help: Content tab analytics tips (Shorts)](https://support.google.com/youtube/answer/12942217?hl=en&co=YOUTUBE._YTVideoType%3Dshorts); [YouTube Help: Understand your content performance](https://support.google.com/youtube/answer/12220281?hl=en-ie&ref_topic=12221641&co=GENIE.Platform%3DDesktop)
- **[OFFICIAL] How the metric launched.** YouTube introduced it as "Viewed (vs. swiped away)" together with "Shown in feed", in Advanced Analytics and content-level analytics.
  - Before that, creators saw only a "thumbnail impression" figure. It did not show whether a Short appeared in the feed or was swiped away.
  - The launch date was not in the extract. It was likely 2023 (older).
  - Source: [YouTube Help Community video: "New YouTube Shorts Metric – Viewed vs Swiped Away"](https://support.google.com/youtube/community-video/273390203/new-youtube-shorts-metric-viewed-vs-swiped-away?hl=en)
- **[OFFICIAL] Engaged views and retention metrics.**
  - "Engaged views" count viewers who stayed past the initial seconds, not including loops.
  - Average view duration and average percentage viewed (APV) for Shorts are calculated only among viewers who stayed to watch. APV therefore describes the body of the Short, not the hook.
  - Source: [YouTube Help: Content tab analytics tips (Shorts)](https://support.google.com/youtube/answer/12942217?hl=en&co=YOUTUBE._YTVideoType%3Dshorts)
- **[OFFICIAL, secondhand] Sherman's 2023 Q&A.** Todd Sherman, then Shorts product lead, answered creator questions in a Creator Insider Q&A published 23 Aug 2023 (older).
  - One summary says most Shorts views come from the feed itself, where "the element of a conscious choice on the part of the viewer is missing". In other words, there is no click.
  - Sources: [vidIQ: How does the Shorts algorithm work in 2026](https://vidiq.com/blog/post/youtube-shorts-algorithm/); [OutlierKit: Shorts algorithm in YouTube's words](https://outlierkit.com/resources/youtube-shorts-algorithm/); [Shortimize](https://www.shortimize.com/blog/how-does-youtube-shorts-algorithm-work). Exact per-site attribution was not verified.
- **[ANALYST, attributed to Sherman] "Explore and exploit".**
  - New Shorts are first shown to a small test audience.
  - If early signals are strong, distribution widens. One summary specifies viewers staying past the first ~5 seconds.
  - A high swipe-away rate stops further distribution.
  - No primary transcript was found. Specific thresholds cited by blogs (for example a "70% completion" trigger) appear to be third-party heuristics, not YouTube statements.
  - Sources: [OutlierKit](https://outlierkit.com/resources/youtube-shorts-algorithm/); [Social Champ](https://www.socialchamp.com/blog/youtube-shorts-algorithm/); [Shortimize](https://www.shortimize.com/blog/how-does-youtube-shorts-algorithm-work)
- **[ANALYST compiling YouTube statements] What the Shorts lead said.** Per OutlierKit's compilation:
  - The system finds a small group of people likely to enjoy a Short, shows it to them, and decides what to do next from their response.
  - YouTube "has not published the signals or any weights for Shorts."
  - There is no ideal length, no benefit to a particular posting time, and no reward for hitting a daily upload count.
  - Mass re-uploads and deleting and reposting a Short can be read as spam.
  - Source: [OutlierKit](https://outlierkit.com/resources/youtube-shorts-algorithm/)
- **[OFFICIAL] Topics covered in Sherman Q&As (2023–2024, older).** YouTube Blog "Rene's Top Five" roundups list these topics:
  - "whether the Shorts algorithm matches long-form"
  - "what exactly counts as a view on the Shorts feed"
  - "why some Shorts flatline"
  - whether hashtags still matter
  - "why you shouldn't delete and repost"

  One 2024 roundup says the algorithm is "constantly evolving to better follow the audience" and that sudden drops in performance usually have other causes. The extracts did not include the actual answers. — [Rene's Top Five, 24 Aug 2023](https://blog.youtube/culture-and-trends/renes-top-five-august-24-2023-edition/); [Rene's Top Five, 4 Apr 2024](https://blog.youtube/creator-and-artist-stories/renes-top-five-march-4-2024/); [Rene's Top Five, 18 Apr 2024](https://blog.youtube/culture-and-trends/renes-top-five-on-youtube-april-18-2024-edition/)
- **[OFFICIAL] Separation by surface (18 Apr 2024, older).**
  - Question put to Rene Ritchie: would unticking subscription-feed publishing or notifications for long-form uploads protect long-form performance?
  - His answer was no. Homepage recommendations primarily use data from the same traffic source, meaning how other viewers on the homepage react. They do not depend on whether someone ignored a notification or skipped a video in the Subscriptions feed.
  - Source: [YouTube Blog: Rene's Top Five, 18 Apr 2024](https://blog.youtube/culture-and-trends/renes-top-five-on-youtube-april-18-2024-edition/)
- **[OFFICIAL] No evidence of harm.** YouTube says it hasn't "seen evidence of Shorts negatively impacting long-form performance." — [YouTube Blog: Shorts truths – debunking common myths](https://blog.youtube/creator-and-artist-stories/debunking-common-myths-about-youtube-shorts/); repeated in [YouTube Blog: How to convert YouTube Shorts views into long-form channel growth](https://blog.youtube/creator-and-artist-stories/youtube-related-videos-traffic-guide/)
- **[ANALYST, attributed to Ritchie] Video-level evaluation.** YouTube evaluates at the level of each individual video and topic, "not the channel"; it "doesn't look at channel or creator for those sorts of things." — [The Leap](https://www.theleap.co/blog/youtube-shorts-algorithm/); [Panda Video](https://www.pandavideo.com/blog/shorts-and-long-form-videos-same-channel)
- **[ANALYST] Caution on popular "Shorts are harmless" quotes.**
  - One analysis reports it "chased all three" of the most-cited quotes and found "0 traceable sources" behind them.
  - It identifies a dated May 2025 YouTube statement as the verifiable primary source. That statement's content could not be retrieved here.
  - Another site presents a 2026 Ritchie quote as settled fact, and its wording varies across sites.
  - Sources: [Creaticalc](https://creaticalc.com/blog/do-youtube-shorts-hurt-long-form); [Market Maker](https://marketmakermgmt.com/blog-list2/do-youtube-shorts-hurt-your-channel)
- **[OFFICIAL] Thumbnails.** YouTube Blog published a conversation between Todd Sherman and creator Jenny Hoyos; the date was not in the extract, probably 2025. Both treat thumbnails as less important for the Shorts feed than for long-form. Custom thumbnails still help channel-page branding and brand deals. — [YouTube Blog: Shorts deep dive (Sherman and Hoyos)](https://blog.youtube/creator-and-artist-stories/youtube-shorts-deep-dive/)
- **[OFFICIAL] Trends versus evergreen.** In the same conversation, Sherman advised against relying only on trends; non-trend videos "will last a lot longer". The same piece reportedly frames the newer view counting as giving creators faster feedback. — [YouTube Blog: Shorts deep dive](https://blog.youtube/creator-and-artist-stories/youtube-shorts-deep-dive/)
- **[NEWS of OFFICIAL] 1 Oct 2026 ranking change.**
  - Announced in a TeamYouTube community post plus a Creator Insider video with Rene Ritchie.
  - YouTube said it is "updating our recommendation systems to further prioritize original content and reduce the reach of content re-uploaded from other creators" in Shorts.
  - It affects recommendations only; monetization stays under the reused-content policy.
  - If a channel that previously aggregated or re-uploaded shifts to original content, the system "will re-evaluate reach".
  - No start date, re-evaluation timescale or reach dashboard was given.
  - Sources: [PPC Land](https://ppc.land/re-uploaded-shorts-lose-reach-as-youtube-favours-original-clips/); [Relevant Audience](https://www.relevantaudience.com/youtube/youtube-shorts-original-content-reach-update/); [OutlierKit](https://outlierkit.com/resources/youtube-shorts-original-content-update/)
- **[ANALYST] Why Shorts surge late.** No official YouTube explanation was found. Third-party explanations:
  - Periodic re-tests with new audiences. This is unverified.
  - Evergreen discovery, because people "search, browse, and discover videos weeks, months, or even years after they're published."
  - A creator observed that one view spike coincided with YouTube changing its view-count mechanism that week, which may be a counting artifact.
  - Sources: [Socialinsider](https://www.socialinsider.io/blog/how-long-does-it-take-for-yt-shorts-to-get-views/); [Miraflow](https://miraflow.ai/blog/what-happens-youtube-shorts-after-30-days-old-content-views)
- **[ANALYST] Conflicting claim on recency.** One post claims that in late 2025, analysts saw YouTube prioritise Shorts newer than about 28–30 days. This is a single unverified source. — [Medium (A. Ershov)](https://medium.com/@AlexanderErshov/youtube-shorts-getting-0-views-heres-exactly-why-and-how-to-fix-it-84202c3eb6b3)

### Inferences
- **The first second does the job of a title and thumbnail.** Feed viewers make no click decision, so the first frame and first second are what earns the view. "Stayed to watch" acts as Shorts' equivalent of click-through rate. APV and average view duration (computed only among stayers) measure the body of the Short.
  - Low stayed-to-watch means the hook is the problem.
  - High stayed-to-watch with low APV means the middle or ending is the problem.
- **A weak Short should not drag down long-form.** Evaluation is per video, per topic and per traffic source, so a weak Short should not depress long-form homepage ranking. Deleting and reposting is the riskier move because of spam handling.
- **Late surges have no published cause.** They fit an audience-matching system with no published expiry; Sherman's comment that non-trend videos "will last a lot longer" points the same way. Since 31 Mar 2025, public view counts include every start and replay, so check any apparent spike against engaged views before treating it as real redistribution.

### Gaps
- The primary transcript of the 23 Aug 2023 Creator Insider Q&A could not be read (youtube.com blocked). "Explore/exploit" and the "5 seconds" detail are secondhand.
- The official answers to "Is the Shorts algorithm the same as long-form?" and the "May 2025" statement cited by Creaticalc were not retrieved.
- Found no official explanation of surges weeks or months later.
- Found no statement on whether Shorts use viewer satisfaction surveys the way long-form does.
- **Lead (unverified):** YouTube staff have described Shorts and long-form recommendations as evaluated separately ("decoupled"), so Shorts viewers' behaviour doesn't affect long-form recommendations. Find the exact Creator Insider or Ritchie wording and date before citing.

---

## Q2. What changed for Shorts in 2024–2026?

### Takeaway
Between Oct 2024 and Oct 2026, Shorts changed in six directions:
- **Longer:** up to 3 minutes.
- **Counted more generously:** every start or replay since 31 Mar 2025, with "engaged views" kept for analytics and YPP.
- **More AI-driven:** Veo 3 Fast, Reimagine, Gemini Omni in Remix, a Gemini editing assistant, and promised likeness Shorts.
- **More episodic:** "Shorts series" (Sept 2026).
- **Stricter on originality:** "inauthentic content" (Jul 2025) and re-upload reach cuts (Oct 2026).
- **Harder to monetize for small Shorts channels:** from 1 Feb 2027.

### Cited Findings
Chronological:

- **3 Oct 2024 announcement, effective 15 Oct 2024 (older): 3-minute Shorts.**
  - Square or vertical uploads of up to 3 minutes count as Shorts. YouTube framed this as a top creator request.
  - Templates arrived, reached through the Remix button.
  - Viewers got a "show fewer Shorts" option.
  - Sources: [YouTube Help: Understand three-minute YouTube Shorts](https://support.google.com/youtube/answer/15424877?hl=en); [AlternativeTo](https://alternativeto.net/news/2024/10/youtube-shorts-extends-limit-to-3-minutes-adds-templates-and-show-fewer-shorts-option); [TechCrunch, 3 Oct 2024](https://techcrunch.com/2024/10/03/youtube-takes-on-tiktok-with-longer-shorts-templates-trends-and-more); [YouTube Blog: Tall updates coming to Shorts](https://blog.youtube/news-and-events/tall-updates-coming-to-shorts/)
- **[OFFICIAL] Content ID rule for Shorts over 1 minute.**
  - A Short longer than one minute with an active Content ID claim of any type is blocked globally. It cannot be played, recommended or monetized, though the channel is not penalized.
  - Fixes: remove the claimed audio or dispute the claim. Shorts under one minute are unaffected.
  - Most Shorts Audio Library songs can run up to 90 seconds in a 3-minute Short; some are capped at 60 or 30 seconds. YouTube Audio Library royalty-free tracks don't receive Content ID claims.
  - Source: [YouTube Help: Understand three-minute YouTube Shorts](https://support.google.com/youtube/answer/15424877?hl=en)
- **[OFFICIAL] Later rule for music channels.** Square or vertical videos over one minute uploaded on or after 8 Dec 2025 by Official Artist Channels and linked music-owner channels are classified as Shorts. This is per the search extract of the Help page; verify the exact wording. — [YouTube Help: Understand three-minute YouTube Shorts](https://support.google.com/youtube/answer/15424877?hl=en)
- **Late 2024 to early 2025 (older): Veo in Dream Screen.** YouTube Blog posts exist on Veo coming to Shorts: "A future full of opportunities, Made On YouTube" (2024) and "Imagine it, create it: Veo 2 is coming to YouTube Shorts". Their content and dates were not retrieved. — [YouTube Blog: Made on YouTube 2024](https://blog.youtube/news-and-events/made-on-youtube-2024/); [YouTube Blog: Veo 2 is coming to Shorts](https://blog.youtube/news-and-events/veo-2-shorts/)
- **31 Mar 2025: view-counting change.**
  - A Shorts view now counts every time a Short starts to play or replays, with no minimum watch time. This aligns with TikTok and Instagram.
  - The old metric is kept as "engaged views", available in Advanced Mode.
  - YPP eligibility and earnings remain based on engaged views.
  - YouTube said "views may be higher moving forward" and advised using engaged views to compare against content published before 31 Mar.
  - Sources: [PPC Land](https://ppc.land/youtube-changes-how-shorts-views-are-counted-from-march-31/); [vidIQ](https://vidiq.com/blog/post/youtube-view-count-update/); [Digital Music News, 27 Mar 2025](https://www.digitalmusicnews.com/2025/03/27/how-does-youtube-shorts-count-views-2025/); [Entrepreneur](https://www.entrepreneur.com/business-news/youtube-shorts-will-see-more-view-counts-earnings/489190); [Sprout Social](https://support.sproutsocial.com/hc/en-us/articles/35874991211533-YouTube-Shorts-View-Count-Update-March-2025)
  - **Conflicting definition:** vidIQ describes engaged views as including meaningful interaction such as likes or comments. The Help Center definition is staying past the initial seconds, excluding loops.
- **[OFFICIAL] Related-video link (the official Shorts-to-long-form bridge).** Launched c. late 2023 (older).
  - Setup: YouTube Studio > Content > choose the Short > Related video.
  - Requires advanced-features access. The target must be public or unlisted and follow the Community Guidelines.
  - The link appears as a clickable link below the channel handle.
  - Shorts made with the Studio "Clips & Shorts" tool automatically get the source video as their related video, unless the Short is private, unlisted or Made for Kids.
  - Shorts made via Remix from a watch page link back to the original. This only works for your own public long-form uploads.
  - Sources: [YouTube Help: Add a related video to your Shorts](https://support.google.com/youtube/answer/14075157?hl=en); [YouTube Help: Video clips & Shorts in Studio](https://support.google.com/youtube/answer/15824265?hl=en); [YouTube Help: Create Shorts from your videos](https://support.google.com/youtube/answer/12836917?hl=en&co=GENIE.Platform%3DAndroid)
- **15 Jul 2025: "inauthentic content" rule.** YPP's "repetitious content" rule was renamed "inauthentic content" and broadened to mass-produced or repetitive uploads. Details are in Q8. — [TechCrunch, 9 Jul 2025](https://techcrunch.com/2025/07/09/youtube-prepares-crackdown-on-mass-produced-and-repetitive-videos-as-concern-over-ai-slop-grows); [Digiday](https://digiday.com/media/youtubes-ai-slop-crackdown-has-creators-concerned-marketers-cheering/)
- **[OFFICIAL] Sept 2025, Made on YouTube 2025.**
  - "We've started integrating Google DeepMind's Veo 3 Fast into YouTube Shorts so you can easily create video backgrounds or clips with sound, for free."
  - Also: apply motion, restyle videos, add props.
  - Likeness detection, which lets creators detect and manage AI videos using their face, expanded to all YPP creators in open beta.
  - Sources: [YouTube Blog: Made on YouTube 2025](https://blog.youtube/news-and-events/made-on-youtube-2025/); [YouTube Blog: new creative tools](https://blog.youtube/news-and-events/generative-ai-creation-tools-made-on-youtube-2025/)
- **[OFFICIAL via NEWS] 21 Jan 2026: Neal Mohan's annual letter.**
  - Shorts now average 200 billion daily views.
  - "This year you'll be able to create a Short using your own likeness, produce games with a simple text prompt, and experiment with music."
  - More than 1 million channels used YouTube's AI creation tools daily in Dec 2025.
  - To reduce low-quality AI content, YouTube is "actively building on our established systems that have been very successful in combatting spam and clickbait."
  - Press summaries also mention images coming to Shorts and AI editing tools.
  - Sources: [YouTube Blog: Mohan's 2026 letter](https://blog.youtube/inside-youtube/the-future-of-youtube-2026/); [TechCrunch, 21 Jan 2026](https://techcrunch.com/2026/01/21/youtube-will-soon-let-creators-make-shorts-with-their-own-ai-likeness); [Variety](https://au.variety.com/2026/digital/news/youtube-channels-using-ai-tools-reduce-slop-neal-mohan-letter-32190/); [eWeek](https://www.eweek.com/de/news/youtube-ai-slop-crackdown-creators/); [Free Press Journal](https://www.freepressjournal.in/amp/tech/youtube-ceo-neal-mohan-unveils-upcoming-features-in-2026-images-coming-to-shorts-new-shopping-upgrade-ai-editing-tools)
- **[OFFICIAL] Mar 2026: "Reimagine".** A Veo-powered Remix tool that turns a single frame of an existing Short into a new 8-second clip. — [YouTube Blog: Reimagine](https://blog.youtube/news-and-events/reimagine-new-ai-powered-remix-tool-youtube-shorts/)
- **[NEWS] Apr 2026: viewers can effectively switch off the Shorts feed.**
  - Path: You > Settings > Time management > Shorts feed limit > 0 minutes. It was reportedly not yet rolled out to all users.
  - Shorts can still appear in Subscriptions, search, channel pages, notifications, playlists and shared links.
  - Sources: [TechRadar](https://www.techradar.com/computing/software/youtube-watchers-praise-awesome-new-option-to-disable-annoying-shorts-heres-how-to-do-it); [Android Police](https://www.androidpolice.com/youtube-shorts-kill-switch/); [HelloPartner, 21 Apr 2026](https://hellopartner.com/2026/04/21/youtube-just-gave-users-the-option-to-fully-disable-shorts-what-do-the-experts-say)
- **[OFFICIAL] Google I/O 2026.**
  - "You can now expand your creativity with Gemini Omni in YouTube Shorts Remix and the YouTube Create app."
  - Likeness detection expanded to all creators aged 18 and over.
  - Trade coverage also reports a new "Unique Reach" metric and an AI "Extend" feature in Shorts Remix; details were not retrieved.
  - Sources: [YouTube Blog: Google I/O 2026](https://blog.youtube/news-and-events/youtube-news-google-io-2026/); [PPC Land: Unique Reach + Gemini Omni](https://ppc.land/youtube-adds-unique-reach-metric-and-gemini-omni-to-shorts-for-creators/); [PPC Land: Remix Extend](https://ppc.land/youtube-shorts-remix-gains-ai-powered-extend-feature-for-creators/)
- **[OFFICIAL] Announced c. Aug 2026, effective 1 Feb 2027: YPP changes.**
  - **Earning from Shorts:** creators will need 10M qualified Shorts views in the last 90 days to earn from the "Shorts Creator Pool" each month. Missing the threshold does not remove a channel from YPP or affect long-form earnings.
  - **New applicants:** 1,000 subscribers plus either 8,000 qualified watch hours in the last 365 days or 20M qualified Shorts views in the last 90 days. Existing YPP members are unaffected by the entry change.
  - **"Active" channel definition:** 1,000 qualified watch hours in 365 days, or 1M qualified Shorts views in 90 days, or 2 long-form videos or 5 Shorts every 90 days.
  - **Deadline:** updated terms must be accepted in Studio by 31 Jan 2027.
  - The announcement date is inferred from the Business Standard URL (11 Aug 2026).
  - Sources: [YouTube Blog: YPP changes 2027](https://blog.youtube/news-and-events/youtube-partner-program-updates-2027-new-opportunities-earn/); [YouTube Help: Changes to the YPP](https://support.google.com/youtube/answer/12843009?hl=en); [PPC Land](https://ppc.land/youtube-cuts-shorts-pay-for-channels-under-10m-views-from-february-2027/); [Business Standard](https://www.business-standard.com/technology/tech-news/technology-tech-news-youtube-partner-program-monetisation-rules-2027-watch-hours-shorts-views-126081100708_1.html)
- **[NEWS, unverified detail] Premium split.** Premium is reported to allocate 30% of net subscription revenue to creators and Premium Lite 60%. This is a secondary report; check before use. — [Social Samosa](https://www.socialsamosa.com/news-2/youtube-changes-ypp-rules-shorts-premium-ad-revenue-sharing-2027-12249534)
- **[OFFICIAL] Current Shorts revenue share (since 1 Feb 2023, older).** Creators keep 45% of the Shorts ad revenue allocated to them, after a music-licensing deduction. This is the reverse of the 55% creator share on long-form. — [YouTube Help: Shorts monetization policies](https://support.google.com/youtube/answer/12504220?hl=en) (figure not re-verified in this session; consistent with long-standing Help text)
- **[OFFICIAL] Current YPP entry routes (before Feb 2027).**
  - Full YPP: 1,000 subscribers plus either 4,000 public watch hours in 12 months or 10M valid public Shorts views in 90 days.
  - Lower fan-funding tier: 500 subscribers plus 3 uploads in 90 days plus either 3,000 watch hours or 3M Shorts views.
  - Sources: [YouTube Help: YPP overview & eligibility](https://support.google.com/youtube/answer/72851?hl=en&co=GENIE.Platform%3DAndroid); [YouTube Help: Expanded YPP](https://support.google.com/youtube/answer/13429240?hl=en&co=GENIE.Platform%3DAndroid) (page text not retrieved; figures from long-standing Help text, should be verified)
- **[NEWS] 23 Sept 2026: Made on YouTube 2026.**
  - **"Shorts series":** creators can group Shorts into seasons and episodes, with custom thumbnails and series playback. TechCrunch frames this as competition with microdrama apps.
  - **Gemini editing assistant** in Shorts and the YouTube Create app: describe edits in words, for example reorder frames, trim pauses or sync music.
  - **Expanded image carousels** in the Shorts feed.
  - **"Ask YouTube" shopping** inside playback.
  - **Custom feeds** built by describing what you want to watch, for all US users "this fall".
  - The official YouTube recap could not be retrieved.
  - Sources: [TechCrunch, 23 Sept 2026](https://techcrunch.com/2026/09/23/youtubes-new-short-series-feature-brings-episodic-viewing-to-shorts/); [Social Media Today](https://www.socialmediatoday.com/news/youtube-presents-new-ai-and-engagement-features-at-made-on-2026/831216/); [TheWrap](https://www.thewrap.com/industry-news/tech/made-on-youtube-updates-2026/); [Analytics Insight](https://www.analyticsinsight.net/news/youtube-2026-update-ai-editing-ask-youtube-shopping-shorts-series-announced)
- **1 Oct 2026: originality-first Shorts recommendations.** See Q1 and Q8. — [PPC Land](https://ppc.land/re-uploaded-shorts-lose-reach-as-youtube-favours-original-clips/)

### Inferences
- **Benchmark on engaged views.** Since 31 Mar 2025 the public view count overstates attention. Judge Shorts on engaged views and stayed-to-watch, and only compare pre- and post-March 2025 Shorts using engaged views.
- **Watch music claims above one minute.** A Short over 1:00 with any Content ID claim is invisible: not played, not recommended. Keep Shorts that use commercial music at 60 seconds or less, or use YouTube Audio Library tracks.
- **2027 monetization pushes small channels toward the funnel model.** The 10M qualified views per 90 days requirement means most small and mid-size Shorts channels will earn little or nothing from the Shorts pool. Shorts become mainly a discovery and conversion tool, which raises the importance of the related-video funnel in Q6.
- **Series are a new retention lever.** "Shorts series" (Sept 2026) and the earlier success of episodic Shorts suggest structured multi-part storytelling may get native support, such as series playback. Watch for how series are surfaced in the feed; no data yet.
- **AI tools are cheap but carry policy risk.** Veo 3 Fast, Reimagine and Gemini Omni lower production cost, but the inauthentic-content rule and the 2026 anti-slop and originality changes make templated AI output a reach and monetization risk unless creative input is substantive.

### Gaps
- Found no 2024–2026 data on **Shorts on TV**: share of Shorts views on connected TVs, or TV-specific ranking.
- Details of YouTube's "Sharing your passion on YouTube pays off: An update on Shorts revenue share" were not retrieved ([YouTube Blog](https://blog.youtube/inside-youtube/shorts-revenue-sharing-update/)).
- The definition of "qualified Shorts views" in the 2027 YPP terms was not retrieved. Is it the same as engaged views?
- Exact dates and features for Dream Screen with Veo (2024), Veo 2 (2025) and "YouTube Shorts introduces new creation tools" (2025) were not retrieved ([YouTube Blog](https://blog.youtube/news-and-events/new-shorts-creation-tools-2025/)).
- Found no 2026 change to the 3-minute maximum.
- **Lead (unverified):** clickable links in Shorts descriptions and comments were disabled around 31 Aug 2023 for spam reasons, and the related-video link replaced them. Verify the date.

---

## Q3. Which benchmarks matter?

### Takeaway
- **No official thresholds.** YouTube publishes no "good" stayed-to-watch percentage or APV.
- **Third-party targets** cluster at 70–80% stayed-to-watch.
- **A top Shorts creator's numbers:** Jenny Hoyos reportedly runs about 85% stayed and about 90–95% retention.
- **Length data splits by measure:**
  - 45–60 s Shorts win on average views (higher ceiling).
  - 11–20 s Shorts win on median views (more consistent).
  - Over 90 s underperforms on medians.
- **Posting time and frequency:** YouTube says length, posting time and daily upload counts carry no built-in bonus. Found no rigorous posting-frequency study.

### Cited Findings
- **[OFFICIAL] No official threshold.** YouTube publishes no universal stayed-to-watch threshold. Extracts note the more defensible approach is to compare a Short against your own similar Shorts. — [OutlierKit](https://outlierkit.com/resources/youtube-shorts-algorithm/); [Subscribr](https://subscribr.ai/youtube-strategy/youtube-shorts-analytics-metrics-growth)
- **[ANALYST] Third-party targets.**
  - Guides commonly cite 70% or 75% "viewed" as trigger points, or "at least 75–80%" as a target.
  - At least one source in the same result set argues these cut-offs are SEO-blog inventions, not YouTube numbers.
  - Sources: [Subscribr](https://subscribr.ai/youtube-strategy/youtube-shorts-analytics-metrics-growth); [ContentStudio](https://contentstudio.io/blog/youtube-shorts-analytics-guide); [Bytecap retention benchmarks](https://www.bytecap.io/research/youtube-shorts-retention-benchmarks); [Frameos: what's known vs folklore](https://frameos.studio/blog/how-the-youtube-shorts-algorithm-works); [Everpop](https://everpop.app/blog/youtube-shorts-algorithm-2026-what-actually-matters). Exact per-site attribution was not verified.
- **[OFFICIAL] APV only counts stayers.** APV and average view duration are computed only among viewers who stayed to watch, and engaged views exclude loops. A loop-heavy Short can therefore show APV above 100%, because looped watch time counts toward duration. This mechanism is inferred from the definitions; I found no explicit Help statement about APV above 100%. — [YouTube Help: Content tab analytics tips (Shorts)](https://support.google.com/youtube/answer/12942217?hl=en&co=YOUTUBE._YTVideoType%3Dshorts)
- **[CREATOR] Jenny Hoyos's reported numbers.**
  - From AI-generated summaries of her video interview (YouTube ID As7abwNhG7Y): average "scroll-through" (stayed) rate of about 85% and retention up to about 95%. Another summary says she targets about 90% or more.
  - In the same interview she reportedly said retention "doesn't matter as much as people think."
  - Her numbers vary across summaries.
  - Sources: [VideoHighlight summary](https://videohighlight.com/v/As7abwNhG7Y); [Summarize.ing](https://summarize.ing/video-69997-Meet-the-Girl-Who-Cracked-YouTube-Shorts-Jenny-Hoyos-Interview-); [YouTubeSummary](https://youtubesummary.com/summary/As7abwNhG7Y)
- **[DATA] quso.ai length study (~108K–113K Shorts; the page title says 113K).**
  - 11–20 s Shorts have the highest median views (901).
  - Under 10 s: median 514.
  - Over 90 s: median 51.
  - Uses medians so viral outliers don't distort the result.
  - Source: [quso.ai](https://quso.ai/research/youtube-shorts-length)
- **[DATA] Vidhalo (331M Shorts, 90-day window).**
  - 45–59 s had the highest average views.
  - 15–29 s is the most common band (about 37% of Shorts) and had the lowest average views.
  - Source: [Vidhalo](https://vidhalo.com/tools/youtube-shorts-length)
- **[DATA, 2023, older] Inflow Network (5,400 Shorts).** 50–60 s Shorts averaged about 1.7M views, nearly 22× more than Shorts under 10 s. This predates 3-minute Shorts. — reported in length roundups such as [Piktochart](https://piktochart.com/blog/how-long-youtube-shorts/) and [Hooked](https://www.hooked.so/blog/how-long-are-youtube-shorts) (exact page attribution not verified)
- **[ANALYST] Retention by length.** 15–30 s Shorts "consistently achieve the highest retention rates (often 80%+)". — [Virvid](https://virvid.ai/blog/best-shorts-length-retention-2026) (methodology unknown)
- **[OFFICIAL, secondhand] No built-in bonuses.** YouTube's Shorts lead said there is no ideal length, no benefit to a particular posting time, and no reward for hitting a daily upload count. — [OutlierKit](https://outlierkit.com/resources/youtube-shorts-algorithm/)
- **[OFFICIAL] Hoyos's length in practice.** In the YouTube Blog conversation, Sherman mentions creators making 15-second "moments" that capture a vibe or scene. Hoyos works in story "bits"; her Shorts are reportedly about 34 seconds. — [YouTube Blog: Shorts deep dive](https://blog.youtube/creator-and-artist-stories/youtube-shorts-deep-dive/); [Summarize.ing](https://summarize.ing/video-69997-Meet-the-Girl-Who-Cracked-YouTube-Shorts-Jenny-Hoyos-Interview-)
- **[ANALYST, unverified] Posting frequency.** Figures circulating, such as "67% increase for 3–5 Shorts per week plus 1–2 long-form" attributed to "AM World Group", have no traceable methodology. — [search-result cluster incl. Touhfa](https://touhfa.art/blog/growth/youtube-shorts-vs-long-form-subscribers/), [InfluenceFlow](https://influenceflow.io/resources/youtube-shorts-and-long-form-video-strategy-the-complete-2026-creators-guide-1/) (attribution not pinned)
- **[OFFICIAL] Upload minimum for an "active" channel (from 1 Feb 2027).** 5 Shorts or 2 long-form videos every 90 days, or the watch-hour or Shorts-view equivalents. This is a monetization rule, not a ranking signal. — [YouTube Blog: YPP changes 2027](https://blog.youtube/news-and-events/youtube-partner-program-updates-2027-new-opportunities-earn/)

### Inferences
- **Length by goal.** Combining the medians (quso) and averages (Vidhalo and Inflow):
  - **For reliable reach per post:** about 11–30 s. Easier to finish and loop, and higher median views.
  - **For maximum upside, watch time and story payoff:** about 45–60 s. Higher averages, driven by outliers.
  - **Over 90 s:** rarely wins on reach. Over 60 s also triggers the Content ID blocking risk.
- **Monetization favours watch time and loops.** The pool is allocated by engaged views, so shorter, loopable Shorts that rack up many engaged views are likely more efficient. This is inferred; there is no official per-length revenue data.
- **Use your own baseline.** Benchmark stayed-to-watch and APV against your own channel's median, not fixed numbers. A Short beating your median on both metrics is a candidate for remakes and follow-ups.

### Gaps
- Found no YouTube-published distribution of stayed-to-watch or APV, and no large audited dataset on stayed-to-watch rates.
- Found no rigorous study on posting frequency for Shorts.
- Found no data on optimal length for revenue specifically (RPM by length).
- The "viewed vs swiped" benchmarks from vidIQ, TubeBuddy and Social Blade could not be retrieved; the search budget was exhausted.

---

## Q4. Which hook and structure techniques work for Shorts?

### Takeaway
The best-documented method is Jenny Hoyos's, discussed with YouTube's Shorts lead:
- Hook in the first second ("one second to hook someone").
- Structure as hook, then a quick foreshadow, then escalating "but/therefore" beats, then a payoff or twist in the final second.
- Use the retention graph to trim the exact seconds where viewers leave.

When a Short promotes a long-form video, YouTube's own guide adds a verbal plus visual CTA in the final ~5 seconds and an immediate payoff at the start of the long-form. Evidence on loop engineering, captions and trending versus original audio could not be verified this session.

### Cited Findings
- **[CREATOR via OFFICIAL] The first second.** "I really do think you have one second to hook someone, especially on Shorts." Hoyos describes a three-step hook formula: **shock, intrigue, satisfy**. — [YouTube Blog: Shorts deep dive (Sherman and Hoyos)](https://blog.youtube/creator-and-artist-stories/youtube-shorts-deep-dive/)
- **[CREATOR] The long-form test for hooks.** A good Short has a hook strong enough that it "could be used as a title and thumbnail on a long form and still get clicks." — [YouTube Blog: Shorts deep dive](https://blog.youtube/creator-and-artist-stories/youtube-shorts-deep-dive/); [Leaderonomics: Lessons from Jenny Hoyos](https://www.leaderonomics.com/videos/box-of-chocolates/how-to-make-great-youtube-shorts-lessons-from-jenny-hoyos)
- **[ANALYST summarizing Hoyos] Structure.** Hook, then a foreshadow of no more than 3 seconds hinting where it's going, then a narrative driven by "but" and "therefore" turns, then a twist ending. This comes from a blog summary, not verified against the interview. — [MonitorYT: hooks](https://monitoryt.com/blog/youtube-video-hooks); [Leaderonomics](https://www.leaderonomics.com/videos/box-of-chocolates/how-to-make-great-youtube-shorts-lessons-from-jenny-hoyos)
- **[CREATOR] The ending.** In a ~34-second Short, Hoyos treats the last second as crucial because it is where the payoff lands. — [Summarize.ing](https://summarize.ing/video-69997-Meet-the-Girl-Who-Cracked-YouTube-Shorts-Jenny-Hoyos-Interview-); [YouTubeSummary](https://youtubesummary.com/summary/As7abwNhG7Y)
- **[CREATOR] Second-by-second editing.** Hoyos gives an example where changing a single one-second segment, based on the retention graph, significantly improved a Short's performance. — [VideoHighlight](https://videohighlight.com/v/As7abwNhG7Y); [Aishorty summary](https://aishorty.com/articles/957e83b1-3e45-4192-8e1f-d768b3974f47)
- **[OFFICIAL] Story units.** Hoyos builds Shorts from short "bits" that each tell a mini-story. Sherman points to creators who make 15-second "moments" capturing a specific vibe or scene. — [YouTube Blog: Shorts deep dive](https://blog.youtube/creator-and-artist-stories/youtube-shorts-deep-dive/)
- **[OFFICIAL] Trends.** Don't rely only on trends; evergreen ideas "will last a lot longer." — [YouTube Blog: Shorts deep dive](https://blog.youtube/creator-and-artist-stories/youtube-shorts-deep-dive/)
- **[OFFICIAL] CTA for conversion Shorts.**
  - Add verbal and visual cues in the final 5 seconds, such as pointing at the related-video link or flashing the long video's thumbnail.
  - A pinned comment also works.
  - The first 5–10 seconds of the long-form must directly address the hook the Short promised: no slow intros or logos.
  - Match the link to viewer intent, for example a quick hack linked to an in-depth tutorial.
  - Source: [YouTube Blog: How to convert Shorts views into long-form growth](https://blog.youtube/creator-and-artist-stories/youtube-related-videos-traffic-guide/)
- **[OFFICIAL] Hashtags.** YouTube's getting-started guide says to "use relevant hashtags to increase discoverability". Sherman's Q&A asked "do hashtags still matter?", but the answer was not in the extracts. — [YouTube Blog: Getting started with Shorts](https://blog.youtube/creator-and-artist-stories/your-guide-to-getting-started-with-youtube-shorts/); [Rene's Top Five, 4 Apr 2024](https://blog.youtube/creator-and-artist-stories/renes-top-five-march-4-2024/)
- **[OFFICIAL] Formats.** Shorts are not just dance challenges or Gen Z content; tutorials, comedy skits and behind-the-scenes all work. — [YouTube Blog: Shorts truths](https://blog.youtube/creator-and-artist-stories/debunking-common-myths-about-youtube-shorts/)
- **[NEWS] Sept 2026 editing tools.** The Gemini editing assistant can "trim pauses" and "sync music" from a text prompt, automating pacing work. — [Analytics Insight](https://www.analyticsinsight.net/news/youtube-2026-update-ai-editing-ask-youtube-shopping-shorts-series-announced)

### Inferences
- **A practical template** consistent with the cited material:
  1. Frame 1 shows the most striking visual or claim, in shock or intrigue form.
  2. Within about 3 seconds, foreshadow the payoff.
  3. Escalate with "but/therefore" beats.
  4. Deliver the payoff or twist at the very end. Ending on the payoff, with no outro, also makes the Short more likely to be replayed.
  5. For funnel Shorts, put the CTA in the last ~5 seconds and link the related video.
- **Edit to the retention graph.** Cut the specific seconds where viewers leave. Hoyos's one-second example suggests small edits can move results a lot.

### Gaps
- Found no verified sources this session on loop engineering (endings that flow into the beginning), on-screen captions or text hooks, pacing data, or trending sounds versus original audio. All were left unsearched once the budget ran out.
- YouTube's "Five tips to master Shorts" exists ([YouTube Blog](https://blog.youtube/creator-and-artist-stories/five-tips-to-master-shorts/)), but its content was not retrieved.
- **Lead (unverified):** common strategist advice is no intro, a visual and text hook in the first frame, burned-in captions because many viewers watch muted, and a loop where the last line completes the first. Verify with vidIQ, Film Booth or Paddy Galloway sources before publishing.

---

## Q5. What do top Shorts creators and strategists teach? Are there documented 0-to-millions case studies?

### Takeaway
Only Jenny Hoyos's methods could be verified this session. She appears in a YouTube Blog conversation with the Shorts product lead and on the Creator Science podcast (#167, "How she averages 10 million views per video"). Teachings from Zach King, Stokes Twins, Daniel LaBelle, Kallmekris, Brent Rivera, Ryan Trahan, MrBeast, Jesser and Alan Chikin Chow could not be researched before the search budget ran out.

### Cited Findings
- **[CREATOR] Hoyos on Creator Science.** Episode #167, about 41 minutes, titled "Jenny Hoyos – How she averages 10 million views per video (YouTube Shorts)". — [Creator Science podcast](https://podcast.creatorscience.com/jenny-hoyos/); [Creator Science](https://creatorscience.com/podcast/jenny-hoyos/)
- **[CREATOR] Hoyos's method.** Hook in one second (shock, intrigue, satisfy), the long-form-title test for hooks, payoff in the last second, second-level edits from retention graphs, and about 34-second runtime. Details and sources are in Q3 and Q4. — [YouTube Blog: Shorts deep dive](https://blog.youtube/creator-and-artist-stories/youtube-shorts-deep-dive/)
- **[CREATOR, unconfirmed] Hoyos's 600M figure.** A "600 million views" figure appears in AI summaries of her "Shorts Genius" interview but is not confirmed by a primary source. — [VideoHighlight](https://videohighlight.com/v/As7abwNhG7Y)
- **[OFFICIAL] APAC case-study post.** YouTube Blog has "5 APAC creators paving their way to 10 million subscribers with YouTube Shorts"; its content was not retrieved. — [YouTube Blog](https://blog.youtube/creator-and-artist-stories/road-to-10-million-subscribers-apac/)
- **[ANALYST, unverified] Hybrid-channel growth claim.** A "2026 analysis by Paddy Galloway" of 500+ channels reportedly found hybrid (Shorts plus long-form) channels gaining subscribers 2.8× faster than long-form-only channels. This was surfaced via secondary blogs and not traced to Galloway's own publication. — [search-result cluster incl. Market Maker](https://marketmakermgmt.com/blog-list2/do-youtube-shorts-hurt-your-channel), [AutoFaceless](https://autofaceless.ai/blog/youtube-channel-growth-statistics-2026) (attribution not pinned)

### Inferences
- Hoyos's method lines up with what YouTube's product lead emphasized in the same conversation: the first second, story bits, evergreen over trend-only. That makes it the best-supported creator playbook here.

### Gaps
None of the following could be verified this session; all need follow-up searches.
- **Lead (unverified):**
  - Zach King: illusion or "magic" edits built around a single reveal, carried over from Vine.
  - Daniel LaBelle: physical-comedy Shorts.
  - Alan Chikin Chow: episodic, Shorts-first storytelling ("Alan's Universe"), directly relevant to the Sept 2026 "Shorts series" feature.
  - Stokes Twins and Jesser: grew rapidly through Shorts-heavy challenge and prank formats.
  - Kallmekris: character comedy cross-posted from TikTok.
  - Brent Rivera: high-volume short-form from the Vine era.
- No documented "0 to millions in days" case studies with dated analytics were retrieved.
- The MrBeast and Ryan Trahan Shorts strategies were not researched.

---

## Q6. Do Shorts help or hurt long-form growth?

### Takeaway
- **YouTube's official position:**
  - It has seen no evidence that Shorts hurt long-form.
  - Official artist channels uploading both formats see better overall watch time and subscriber growth than long-form-only channels.
- **Recommended conversion mechanism:** the related-video link, plus a CTA in the last ~5 seconds, plus a long-form that pays off the Short's promise in its first 5–10 seconds.
- **Independent data is mixed and mostly unaudited.**
- **New 2026 risk:** viewers can cap the Shorts feed at 0 minutes, which hits channels that depend heavily on Shorts.

### Cited Findings
- **[OFFICIAL] No evidence of harm.** "We haven't seen evidence of Shorts negatively impacting long-form performance." — [YouTube Blog: Shorts truths](https://blog.youtube/creator-and-artist-stories/debunking-common-myths-about-youtube-shorts/); [YouTube Blog: related-videos traffic guide](https://blog.youtube/creator-and-artist-stories/youtube-related-videos-traffic-guide/)
- **[OFFICIAL, platform-reported] Artist channels.** "Official artist channels uploading both Shorts and long-form video are seeing better overall watch time and subscriber growth relative to those only uploading long-form." — [YouTube Blog: related-videos traffic guide](https://blog.youtube/creator-and-artist-stories/youtube-related-videos-traffic-guide/)
- **[OFFICIAL] Conversion playbook.**
  - Link the related video to the matching long-form; it can also point to a livestream or another Short.
  - Add a CTA in the last 5 seconds, verbal and visual, for example flashing the long-form thumbnail.
  - Use a pinned comment.
  - Pay off the promise in the long-form's first 5–10 seconds, with no slow intro or logo.
  - Optional: dual-stream live, sending 16:9 to desktop and vertical to the Shorts feed.
  - Source: [YouTube Blog: related-videos traffic guide](https://blog.youtube/creator-and-artist-stories/youtube-related-videos-traffic-guide/)
- **[OFFICIAL, Apr 2024, older] Subscribers who skip long-form.** Long-form homepage ranking relies on homepage audience reactions. Shorts-acquired subscribers ignoring a long-form notification or skipping it in Subscriptions doesn't drag down homepage performance. — [YouTube Blog: Rene's Top Five, 18 Apr 2024](https://blog.youtube/culture-and-trends/renes-top-five-on-youtube-april-18-2024-edition/)
- **[OFFICIAL] Automatic linking.** Studio's "Clips & Shorts" tool automatically links a Short back to its source long-form, and Remix from a watch page links back to the original. — [YouTube Help: Video clips & Shorts in Studio](https://support.google.com/youtube/answer/15824265?hl=en); [YouTube Help: Add a related video](https://support.google.com/youtube/answer/14075157?hl=en)
- **[DATA, mixed and unaudited] Independent studies.**
  - One write-up notes a 250-channel study that measured long-form declines.
  - An 18,000-channel dataset concluded that niche decides the outcome.
  - A 500-channel analysis reported zero measurable negative impact on long-form view counts.
  - Sources: [ytgrowth.io](https://ytgrowth.io/blog/shorts-vs-long-form); [Market Maker](https://marketmakermgmt.com/blog-list2/do-youtube-shorts-hurt-your-channel)
- **[ANALYST, unverified] Hybrid-growth multipliers.** Figures such as "41% faster", "2.8× faster" and "~3×" for hybrid channels circulate. None was traced to a YouTube publication or a published methodology. — [search-result cluster incl. Zebracat](https://www.zebracat.ai/post/youtube-shorts-statistics), [Market Maker](https://marketmakermgmt.com/blog-list2/do-youtube-shorts-hurt-your-channel)
- **[NEWS and ANALYST, Apr 2026] Shorts feed limit risk.**
  - Viewers can set the Shorts feed limit to 0 minutes.
  - One analysis argues channels that depend on Shorts for 80% or more of views "have no funnel" to capture viewers who opt out.
  - A filmmaker quoted by HelloPartner calls Shorts "one of the most powerful discovery tools for creators" and warns that growth could slow, especially for smaller creators, if more viewers opt out.
  - Sources: [OutlierKit](https://outlierkit.com/resources/youtube-disable-shorts-feature-creator-impact-2026/); [HelloPartner, 21 Apr 2026](https://hellopartner.com/2026/04/21/youtube-just-gave-users-the-option-to-fully-disable-shorts-what-do-the-experts-say)
- **[OFFICIAL] Feb 2027 monetization change.** Missing the 10M qualified Shorts views threshold does not affect long-form earnings or YPP membership. Shorts revenue and long-form revenue are explicitly separated. — [YouTube Blog: YPP changes 2027](https://blog.youtube/news-and-events/youtube-partner-program-updates-2027-new-opportunities-earn/)

### Inferences
- **Same channel or separate channel.** Evaluation is per video and topic ("not the channel") and surface-specific. So a Shorts-heavy channel is not penalized on long-form ranking.
  - The real trade-off is audience fit. Shorts subscribers drawn by an off-topic Short are unlikely to watch long-form. Keep Shorts on-topic with the long-form promise if conversion is the goal.
  - A separate channel makes sense only if the Shorts topic or audience differs materially. This is inferred; there is no official guidance.
- **Treat every funnel Short as an ad for a specific long-form.** One intent-matched related video, a CTA in the last 5 seconds, and a long-form cold open that pays off immediately. This is YouTube's own guidance.
- **Plan for less Shorts revenue.** Between the 2027 monetization rules and the feed-limit option, a long-form or community "home base" matters more.

### Gaps
- Found no official data on Shorts-to-long-form conversion rates, or on long-form watch behaviour of Shorts-acquired subscribers. The "Shorts audiences don't convert" debate could not be sourced from creator data this session.
- The "May 2025" official statement on Shorts versus long-form (per Creaticalc) was not retrieved.
- Found no official recommendation on same channel versus separate channel.

---

## Q7. Can Shorts serve as cheap tests for long-form ideas?

### Takeaway
Direct evidence is thin. The closest documented principle is Hoyos's: a good Short hook should work as a long-form title and thumbnail. YouTube's tooling (Clips & Shorts, Remix linking, the Gemini editing assistant) mostly supports the reverse direction, cutting long-form into Shorts. I found no data showing that Shorts performance predicts long-form performance.

### Cited Findings
- **[CREATOR] Hook-to-title test.** The hook should be strong enough to "be used as a title and thumbnail on a long form and still get clicks." — [YouTube Blog: Shorts deep dive](https://blog.youtube/creator-and-artist-stories/youtube-shorts-deep-dive/)
- **[OFFICIAL] Linking tools.** Long-form-to-Shorts tools (Studio Clips & Shorts, Remix) automatically create the related-video link back to the source. — [YouTube Help: Video clips & Shorts in Studio](https://support.google.com/youtube/answer/15824265?hl=en); [YouTube Help: Create Shorts from your videos](https://support.google.com/youtube/answer/12836917?hl=en&co=GENIE.Platform%3DAndroid)
- **[OFFICIAL] Different viewer decisions.** Shorts are judged on a watch-or-swipe decision with no click. Long-form is judged on a click from a title and thumbnail, then retention. These are different viewer decisions. — [YouTube Help: Content tab analytics tips (Shorts)](https://support.google.com/youtube/answer/12942217?hl=en&co=YOUTUBE._YTVideoType%3Dshorts); [vidIQ](https://vidiq.com/blog/post/youtube-shorts-algorithm/)

### Inferences
- **What a Short can and can't test.** A Short can test whether a premise or hook grabs attention, which is roughly a proxy for long-form packaging. It cannot test whether viewers will click a thumbnail or sit through 10 or more minutes.
- **How to read the result.** Treat a breakout Short as a signal to try the premise as long-form, keeping the same promise in the title and thumbnail. A flop is weaker evidence against the idea, because swipe behaviour depends heavily on execution.

### Gaps
- Found no documented, dated case studies this session of creators systematically validating long-form ideas with Shorts, such as MrBeast, Ryan Trahan or Paddy Galloway client examples. The search budget was exhausted.
- **Lead (unverified):** several strategists recommend "Shorts as concept tests"; find primary interviews with numbers.

---

## Q8. What gets Shorts suppressed? How does cross-posting from TikTok or Reels affect performance?

### Takeaway
Five documented suppression levers:
1. **Re-uploads (1 Oct 2026).** Recommendations cut reach for re-uploads of other creators' content. Crops, flips, speed changes, filters, transcribed captions, bulk template edits and narrating voiceovers don't count as transformation.
2. **Inauthentic content (15 Jul 2025).** A YPP rule against mass-produced or repetitive content, including AI slideshows and near-identical narrated stories.
3. **Spam handling.** Deleting and reposting, and mass re-uploading, can be treated as spam.
4. **Content ID.** Shorts over one minute with any Content ID claim are blocked globally.
5. **Low-quality AI.** YouTube's 2026 plan to apply its spam and clickbait systems to low-quality AI content.

No official YouTube statement on TikTok watermarks was retrieved.

### Cited Findings
- **[NEWS of OFFICIAL] 1 Oct 2026 originality change.**
  - Shorts recommendations now "further prioritize original content and reduce the reach of content re-uploaded from other creators".
  - The change relies on YouTube's existing nine-category spam policy, which already governs strikes, demonetization and terminations.
  - Ritchie said that voiceover narration describing what is on screen, minor technical edits and template-based bulk changes don't make a reused clip original. He pointed creators toward their own commentary, analysis and storytelling.
  - Reach "will" be re-evaluated if a channel shifts to original content.
  - Sources: [PPC Land](https://ppc.land/re-uploaded-shorts-lose-reach-as-youtube-favours-original-clips/); [Relevant Audience](https://www.relevantaudience.com/youtube/youtube-shorts-original-content-reach-update/); [OutlierKit](https://outlierkit.com/resources/youtube-shorts-original-content-update/)
- **[ANALYST] What doesn't count as original.** A list attributed to a non-official blog: crops, flips, speed changes, filters, transcribed captions, template-based bulk edits and narrating voiceovers. Sources disagree on whether Shorts cut from your own long-form are affected; YouTube hasn't addressed this. — [Mark Studios](https://www.markstudios.com/blog/youtube-shorts-original-content-update-2026); [Vidio](https://www.vidio.ai/blog/article/youtube-original-content-shorts-update-october-2026)
- **[OFFICIAL via NEWS] 15 Jul 2025 inauthentic-content rule.**
  - YPP's "repetitious content" rule was renamed "inauthentic content" to better identify mass-produced and repetitive content, for example repetitive slideshows with similar narration, or narrated stories with only small differences.
  - Ritchie called it a "minor update"; making money from mass-produced or repetitive videos "has not been eligible for monetization for some time."
  - AI-assisted videos remain monetizable if they enhance original content.
  - Reports say reaction and compilation channels are not the target.
  - Sources: [TechCrunch, 9 Jul 2025](https://techcrunch.com/2025/07/09/youtube-prepares-crackdown-on-mass-produced-and-repetitive-videos-as-concern-over-ai-slop-grows); [Digiday](https://digiday.com/media/youtubes-ai-slop-crackdown-has-creators-concerned-marketers-cheering/); [Betanews](https://betanews.com/2025/07/10/youtube-is-fighting-ai-slop-with-new-monetization-guidelines/); [CineD](https://cined.com/youtube-set-to-crack-down-on-ai-slop-with-monetization-policy-update); [PPC Land: YouTube clarifies inauthentic content](https://ppc.land/youtube-clarifies-inauthentic-content-policy-changes/)
- **[OFFICIAL] Reused content for monetization.** Monetization still falls under the reused-content policy, which requires borrowed material to be changed significantly to make it your own. — [PPC Land](https://ppc.land/re-uploaded-shorts-lose-reach-as-youtube-favours-original-clips/)
- **[OFFICIAL] Deleting and reposting.** Re-uploading a weak Short "can be considered as spam, and your channel could get flagged for spamming." — [YouTube Blog: Shorts truths](https://blog.youtube/creator-and-artist-stories/debunking-common-myths-about-youtube-shorts/); [Rene's Top Five, 4 Apr 2024](https://blog.youtube/creator-and-artist-stories/renes-top-five-march-4-2024/)
- **[OFFICIAL] Content ID on Shorts over one minute.** Any active Content ID claim means the Short is blocked globally: no playback, recommendations or monetization. Shorts under one minute are unaffected. — [YouTube Help: Understand three-minute Shorts](https://support.google.com/youtube/answer/15424877?hl=en)
- **[OFFICIAL via NEWS] Jan 2026 anti-slop plan.** YouTube will extend its spam and clickbait systems to "reduce the spread of low quality AI content". It is also upgrading likeness management in Content ID and supports the NO FAKES Act. — [TechCrunch, 21 Jan 2026](https://techcrunch.com/2026/01/21/youtube-will-soon-let-creators-make-shorts-with-their-own-ai-likeness); [Storyboard18](https://www.storyboard18.com/digital/youtube-ceo-neal-mohan-warns-against-ai-slop-outlines-safeguards-as-generative-tools-scale-in-2026-88165.htm)
- **[ANALYST, attributed to YouTube's Shorts lead] Mass re-uploads.** Mass re-uploads and deleting and reposting can be read as spam. — [OutlierKit](https://outlierkit.com/resources/youtube-shorts-algorithm/)
- **[NEWS] Creator concern.** Creators find the inauthentic-content wording open-ended. YouTuber Bennett Santora said it makes it harder for automated creators to know what's allowed. — [CineD](https://cined.com/youtube-set-to-crack-down-on-ai-slop-with-monetization-policy-update)

### Inferences
- **Cross-posting your own original work** is not "re-uploaded from other creators", so the Oct 2026 change does not target it on its face. The practical risks are the watermark or "foreign platform" look and platform-specific UI text, which may raise swipe-aways. That point is inferred, not official.
- **Clip and compilation channels and AI-template channels** face reduced reach (Oct 2026) and demonetization risk (Jul 2025). The safe path is adding real commentary, analysis or story, not cosmetic edits.
- **Never delete and repost an underperforming Short.** Make a new, materially different version instead.

### Gaps
- Found no official YouTube statement this session on **TikTok or Reels watermarks** in Shorts ranking, and no third-party data on cross-posted versus native Shorts performance.
- **Lead (unverified):** Instagram has publicly said it deprioritizes Reels with visible third-party watermarks. Check whether YouTube has an equivalent statement, possibly in a Sherman Q&A.
- **Lead (unverified):** a Kapwing study (late 2025) reported that a substantial share of Shorts shown to new accounts were "AI slop". Verify the figures and date before use.
- Found no data on how many channels lost reach after the 1 Oct 2026 change, and there is no official dashboard.

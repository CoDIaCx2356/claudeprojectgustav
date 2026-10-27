# YouTube Packaging: Evidence-Based Best Practices for Titles & Thumbnails (Max CTR Without Hurting Satisfaction)

> **Research-conditions note for the report writer (read first).** This session had badly restricted web access. Tavily returned "usage limit exceeded". WebFetch could not resolve any external host, including support.google.com, the MrBeast PDF CDN, etavrian.com and hitfactorapp.com. The HTTPS proxy returned policy 403s for vidiq.com and searchenginejournal.com, and its log showed 403s for youtube.com, blog.youtube, arxiv.org, reddit.com and archive.org. The shared WebSearch budget (200 calls per turn across all agents) ran out after about 19 of my queries.
>
> **Consequences:**
> - Every Cited Finding below comes from **search-engine summaries of the linked pages**, not from full-page reads. Numbers are reproduced exactly as the summaries gave them. Text in quotation marks appeared as quotes in those summaries.
> - Where a summary did not say which of several pages a claim came from, I cite the candidate pages and say so.
> - Anything from my background knowledge is kept in **Gaps**, labelled **UNVERIFIED**, with a suggested source to check.
> - View counts for examples could not be verified, so none are invented.
>
> Evidence types are tagged: **[DATA]** = quantitative study, **[OFFICIAL]** = YouTube statement, **[EXPERT]** = strategist or creator opinion, **[VENDOR]** = tool-company claim with a commercial interest.

## 1. What do large-scale data studies show about thumbnail and title features (faces/emotion, text amount, color/contrast, element count, title length, numbers, questions, capitalization, negativity, curiosity, brackets)?

### Takeaway
The newest large datasets (2025–2026) overturn several folk rules.
- **Faces:** they appear in most breakout thumbnails (69–80% in vidIQ's 500-breakout sample). Controlled comparisons, however, show no average lift (1of10 Media, 300k videos) or even a small within-channel penalty (HitFactor, 1.25M videos, about −6%).
- **Text:** most breakouts carry no text or only 1–3 words.
- **Cosmetic title tricks:** numbers, question marks, brackets, ALL CAPS and emoji show little or no reliable effect.
- **Title length:** the studies conflict, so shorter is the safer default.

The consistent signal is that the *substance* of the packaging (idea, stakes, emotion, curiosity) matters more than surface formatting.

### Cited Findings
**Thumbnails: faces (the most-studied variable; the evidence conflicts)**
- [DATA][VENDOR] **vidIQ, July 2026.**
  - Sample: 500 "breakout" long-form videos (far more views than the channel's own average) across 30 niches.
  - A human face appeared in **69%** of all 500 breakouts, **75%** of the top 100 and **80%** of the top 50.
  - High contrast **slightly declines** as breakouts get bigger.
  - vidIQ says the study **does not establish causation**: the thumbnail is one factor alongside topic, title, channel and timing.
  - [vidIQ Thumbnail Study 2026](https://vidiq.com/research/youtube-thumbnail-study/)
- [DATA] **1of10 Media (agency; analysis by Nate Curtiss, Head of Content).**
  - Sample: 300,000+ viral videos from 2025.
  - Faces performed **about the same as no faces on average**. A face helped **only for larger channels, and modestly**.
  - By niche: **Finance favored faces; Business did not.** **Multi-face thumbnails beat single-face ones.**
  - [etavrian summary](https://www.etavrian.com/news/youtube-thumbnail-faces-study-results); [Search Engine Journal: "Do Faces Help YouTube Thumbnails?"](https://www.searchenginejournal.com/do-faces-help-youtube-thumbnails-heres-what-the-data-says/563944/); [eCommerce Bridge: "The data says it's complicated"](https://www.ecommercebridge.com/do-faces-really-matter-in-youtube-thumbnails-the-data-says-its-complicated/)
- [DATA] **HitFactor Labs, 2026 (independent).** Sample: 1.25 million videos across 16,737 channels. Comparing videos within the same channel, thumbnails with faces were tied to **about 6% fewer views**. — [HitFactor Labs](https://docs.hitfactorapp.com/labs/2026-thumbnails-with-faces/)
- [VENDOR] **1of10 (the tool company).**
  - Claims face-forward thumbnails "dominate outlier data across most categories".
  - Claims a face **reacting to the subject** tends to win over showing the object alone.
  - Its faces post cites eye-tracking research without a source; treat this as marketing.
  - [1of10: Thumbnail Trends 2026](https://1of10.com/blog/youtube-thumbnail-trends-2026/); [1of10: Should you use your face?](https://1of10.com/blog/should-you-use-your-face-in-your-youtube-thumbnails/)

**Thumbnails: text, color/brightness, clutter**
- [DATA][VENDOR] **vidIQ 2026, text.** **No text** was the most common single pattern (**28%** of breakouts), followed by **1–3 words (24%)**. Among thumbnails that used text, the **median was 5 words**. — [vidIQ](https://vidiq.com/research/youtube-thumbnail-study/)
- [DATA][ACADEMIC] **Koh & Cui (2022), *Decision Support Systems*.**
  - Sample: 3,745 marketing videos from 38 top brands in 4 industries.
  - Thumbnail visual attributes were **significantly related to view-through**.
  - **Celebrity pictures** and particular **colorfulness × brightness combinations** were linked to stronger persuasion.
  - "Focusing on **too many objects** can hinder the processing of the information."
  - [ScienceDirect](https://www.sciencedirect.com/science/article/abs/pii/S0167923622000914)
- [DATA][ACADEMIC] **River Publishers (*Journal of Web Engineering*), study of visual expression elements.** Images and colors had a significant positive effect on viewer **satisfaction**; layout and typography did not. — [JWE PDF](https://journals.riverpublishers.com/index.php/JWE/article/download/18891/17877/67121)
- [ACADEMIC] **"Clickbait Aesthetics" (news thumbnails).**
  - A qualitative analysis of 100 Arabic thumbnails found three key clickbait elements: emotional imagery, emojis, and curiosity-inducing **visual–textual complementarity**.
  - The paper notes these strategies can work in the short term but can mislead viewers and harm credibility and trust.
  - Both points come from one search summary and may come from two related papers.
  - [Semantic Scholar PDF](https://pdfs.semanticscholar.org/c6ef/6cd28a85f864533800b6927aa082caa68dc6.pdf)
- [ACADEMIC] **Vitadhani et al. (2021).** OCR plus face recognition on 250 thumbnails; an SVM detected clickbait thumbnails with 0.968 accuracy. This shows embedded text and faces carry signal, but the sample is small and the labels are channel-level. — [IEEE](https://ieeexplore.ieee.org/abstract/document/9497811/)
- [EXPERT] **Paddy Galloway:** three or fewer focal points and fewer than five words of thumbnail text. — [Marketing Examined: Paddy Galloway guide](https://www.marketingexamined.com/blog/paddy-galloway-youtube-guide); [Paddy Galloway on X](https://x.com/PaddyG96/status/1811083499044044951)

**Titles: length (the studies conflict)**
- [DATA][VENDOR] **ViewsKit.** Sample: 61,838 long-form videos, Shorts excluded. Median views **fall monotonically as titles get longer**; titles **under 30 characters earned about 2× the median views** of 80–100-character titles. — [ViewsKit: Title Length Curve](https://viewskit.com/blog/youtube-title-length-curve)
- [DATA][VENDOR] **YTGrowth, 2026.** Sample: 28,947 videos. Found **no correlation with length**. Reported that numbers, brackets, colons, ALL CAPS and emoji make **"no measurable difference"**. The summary's phrase "every other pattern tested" implies one pattern did matter; it was not named. — [YTGrowth](https://ytgrowth.io/blog/youtube-title-length)
- [DATA][VENDOR] **OverseerOS.** Sample: 2,622 titles. At the character level, "the difference was effectively zero." — [OverseerOS: Title Length](https://www.overseeros.com/blog/best-youtube-title-length-study)
- [DATA][ACADEMIC] **Excel-tutorial preprint.** Studies YouTube videos about Microsoft Excel. One summary describes a **bell-shaped** relationship, with views peaking at specific lengths and word counts. Another says longer titles drew more views but outcomes spread more widely. The summaries conflict. — [ResearchGate](https://www.researchgate.net/publication/387126034_Effect_of_Title_Length_and_Word_Count_on_Views_Evidence_from_Microsoft_Excel_videos_on_YouTube)
- [EXPERT] **Paddy Galloway** favors titles of **about 50 characters, sometimes up to 60**, in **plain, universal words**. His X posts say under 60 characters. — [Creator Science podcast: Paddy Galloway](https://podcast.creatorscience.com/paddy-galloway-2/); [Marketing Examined](https://www.marketingexamined.com/blog/paddy-galloway-youtube-guide)

**Titles: numbers, questions, capitalization, brackets**
- [DATA][VENDOR] **Numbers.** Titles with digits had a somewhat higher raw breakout rate, **11.9% vs 9.9%**, but the difference was "not statistically strong enough to establish a reliable advantage". The summary did not say which of the vendor studies this came from; Subsub.io (120,703 titles; methodology unverified) is the likeliest. — [Subsub.io](https://www.subsub.io/blog/youtube-title-formulas-that-work)
- [VENDOR] **The "36% more clicks with numbers" figure** (attributed to Conductor) is only repeated secondhand. — [Humble & Brag](https://humbleandbrag.com/blog/youtube-title-best-practices)
- [DATA][VENDOR] **Questions.** Sample: 7,935 million-view titles. A question mark alone gave **"no measurable public-view advantage"**; in matched pairs, question and statement titles split almost evenly. — [OverseerOS: Should titles be questions?](https://www.overseeros.com/blog/should-youtube-titles-be-questions)
- [DATA][VENDOR] **Capitalization.** Sample: 6,878 million-view titles. Title Case–dominant styles were **83.3%** of recent titles. The authors stress this is descriptive and does not show that switching style causes more views. — [OverseerOS: Capitalization](https://www.overseeros.com/blog/youtube-title-capitalization)

**Titles: emotional triggers, curiosity, negativity, intensity**
- [DATA][EXPERT] **Jake Thomas (Creator Hooks).**
  - In his database of **408** titles, **61% used curiosity, 46% desire, and 40% fear or negativity**.
  - The strongest titles usually **pair curiosity with fear or desire**.
  - [vidIQ: 3 Secrets for Writing Click-Worthy Titles](https://vidiq.com/blog/post/write-click-worthy-youtube-titles/); [Net Influencer: Jake Thomas](https://www.netinfluencer.com/creator-hooks-jake-thomas-code-on-clickable-youtube-titles/). The summary did not separate these two sources.
- [EXPERT] **The leaked MrBeast production guide (2024)** advises intensifying the wording: **"I Survived" over "I Spent"**, and "In general the more extreme the better." The second line appears in the PDF itself, per the summary. — [MrBeast guide PDF](https://cdn.prod.website-files.com/6623b7720b009050313e701c/66ede69453b7bbadcd2f05a8_How-To-Succeed-At-MrBeast-Production%20(2).pdf); [Creator Handbook](https://www.creatorhandbook.net/leaked-document-allegedly-reveals-mrbeasts-secrets-to-youtube-success-the-key-takeaways/)

### Inferences
- **Faces are an "it depends" lever, not a rule.** They are common among breakouts but show no average causal lift and a slight within-channel penalty. A face is likely worth it when it shows a **strong, readable reaction to the subject** or a **group or relationship dynamic** (multi-face beat single-face), in face-friendly niches such as Finance. It should not just be a default talking head. This should be tested per channel.
- **Text in thumbnails should be zero to about 4 words.** It should add information the title doesn't carry. This rests on vidIQ's text distribution, Paddy's under-5-words rule, and Koh & Cui's clutter finding.
- **Cosmetic title tricks are weak.** Question marks, digits for their own sake, brackets, caps and emoji did not reliably move views in 2025–2026 vendor data. Effort is better spent on the concept, the stakes and the emotional trigger: curiosity plus fear or desire, and extreme-but-true wording.
- **Shorter titles are the safer default.** Some data favors short titles and none shows long titles winning outright. Short titles also survive mobile truncation. A practical target is **at most about 50–60 characters with the hook word up front**.
- **Clutter hurts.** At most three focal points, high subject-to-background separation, and bright/colorful palettes (Koh & Cui) are the evidence-aligned visual defaults. Note that vidIQ found extreme contrast is *not* more common among the very biggest breakouts.

### Gaps
- **Methods could not be checked.** I could not open the 1of10 Media, HitFactor, vidIQ, ViewsKit, YTGrowth, OverseerOS or Subsub.io studies to check controls (channel size, topic, upload date), outcome metrics (views vs CTR) or significance. All of these except HitFactor are vendor studies with commercial interests.
- **Variables with no YouTube-specific data retrieved:**
  - **arrows and circles**
  - overall **brightness** on YouTube (only Koh & Cui on branded video)
  - **number of elements**, beyond qualitative claims
  - **"I" vs "you"** in titles
  - **brackets/parentheses**, beyond YTGrowth's "no measurable difference"
  - **negativity on YouTube specifically**
- **Sources not reached:** I found nothing from **Spotter, Hootsuite, Buffer, ThumbnailTest or TubeBuddy** with aggregate feature-level data. The search budget ran out before I could target them.
- **UNVERIFIED (secondhand):** "A 2024 vidIQ study of 11,428 videos" reportedly found clear facial close-ups get about 2× the CTR of thumbnails without faces. This came from a blog summary surfaced alongside vidIQ's research page and was not verified. It conflicts with the 2025–2026 controlled studies.
- **UNVERIFIED background, negativity:** Robertson et al. (2023), *Nature Human Behaviour*, "Negativity drives online news consumption." Upworthy Research Archive, about 105k headline variants from about 22.7k A/B tests and about 370M impressions. **Each additional negative word raised CTR by about 2.3%**, and positive words lowered it. These are news headlines, not YouTube. Check at https://www.nature.com/articles/s41562-023-01538-4
- **UNVERIFIED background, older and non-YouTube:**
  - Netflix's 2016 "The Power of a Picture" research:
    - artwork reportedly accounted for over 82% of members' focus while browsing
    - about 1.8 seconds was spent per title
    - images with **expressive, complex facial emotion** performed well
    - groups of more than 3 people performed worse
  - Check at https://about.netflix.com/en/news/the-power-of-a-picture
- **UNVERIFIED background, older (2013–14), blog headlines not YouTube:** HubSpot and Outbrain reportedly found headlines with [brackets] performed about 38% better.
- **UNVERIFIED background, theory:** the "curiosity gap" rests on Loewenstein's (1994) information-gap theory of curiosity (*Psychological Bulletin* 116(1):75–98).

## 2. What does YouTube say about Test & Compare (thumbnail and title A/B tests), what does it optimize for, how often are there clear winners, and what have creators learned from running tests?

### Takeaway
Test & Compare lets creators test **up to 3 titles, thumbnails, or title+thumbnail combinations** on a long-form video. Title testing went global on **Dec 9, 2025**. It picks the winner by **watch time share, not CTR**, so a variant that wins clicks but loses viewers will not win.

YouTube publishes **no official rate** of conclusive results. Third-party guides agree that "Inconclusive" or "Performed Same" outcomes are common on low-traffic videos and for near-identical variants. Published creator learnings are thin and mostly anecdotal.

### Cited Findings
**Official mechanics**
- [OFFICIAL] Creators can **test and compare up to 3 different titles and thumbnails**. The test **should complete within two weeks**. **Changing the title or thumbnail during a test stops it automatically**, and the test must be restarted. When the test ends, **the option with the highest watch time is shown to all viewers**. — [YouTube Help: A/B test titles & thumbnails](https://support.google.com/youtube/answer/16391400?hl=en-GB)
- [OFFICIAL, via third-party explanation] **Watch time share** = "the portion of experiment watch time attributed to viewers who saw each package." YouTube also evaluates **statistical confidence**, so creators should rely on the Studio result label rather than read a winner from the percentages. — [ThumbnailPeak](https://thumbnailpeak.com/blog/youtube-thumbnail-ab-testing); [Tasty Edits](https://www.tastyedits.com/youtube-abc-testing-thumbnails/)
- **Result labels** are **Winner / Performed Same / Inconclusive**.
  - Per third parties: if a test is inconclusive, **the first-uploaded option stays live**.
  - Creators can **manually choose** which option stays, even after YouTube declares a winner.
  - Some guides say "Performed Same" means YouTube suggests picking the option you prefer.
  - Guides conflict on the exact behavior of Inconclusive vs Performed Same.
  - [gyre.pro](https://gyre.pro/blog/youtubes-new-title-ab-testing-tool-everything-creators-need-to-know); [Descript](https://www.descript.com/blog/article/how-to-ab-test-on-youtube-for-better-video-performance); [vidIQ](https://vidiq.com/blog/post/youtube-launches-new-thumbnail-testing-tool/)
- **Title testing launched globally on December 9, 2025**, alongside thumbnail testing.
  - **Requirements:** Advanced Features enabled and a verified account.
  - **Available on:** public long-form videos, livestream archives saved as videos, and podcast episodes.
  - **Not available on:** Made for Kids, age-restricted or private videos, and Shorts.
  - Per one source, **no CTR data is shown; Watch Time Share is the only metric.**
  - [Search Engine Journal](https://www.searchenginejournal.com/youtube-title-a-b-testing-rolls-out-globally-to-creators/562571/); [PPC Land](https://ppc.land/youtube-expands-a-b-testing-to-include-titles-alongside-thumbnails/); [RouteNote](https://routenote.com/blog/youtube-expands-a-b-title-testing/); [vidIQ](https://vidiq.com/blog/post/youtube-launches-new-title-testing-tool/); [ThumbnailTest](https://thumbnailtest.com/news/youtube-releases-title-test-compare/)
- **Also excluded, per one guide:** scheduled live streams and Premieres before they air. — [Descript](https://www.descript.com/blog/article/how-to-ab-test-on-youtube-for-better-video-performance)

**How long tests take and how often they are conclusive**
- **Third-party estimates of duration vary widely:**
  - "1 to 14 days depending on how quickly statistical significance is reached"
  - "1–2 weeks and thousands of impressions"
  - "a few hours to a few days"
  - **Inconclusive usually means too few impressions**, so retry on a higher-traffic video.
  - **Similar variants need more impressions** to separate than very different ones.
  - The summary did not attribute each claim to a specific guide among: [gyre.pro](https://gyre.pro/blog/youtubes-new-title-ab-testing-tool-everything-creators-need-to-know), [ThumbMagic](https://www.thumbmagic.co/blog/ab-test-youtube-thumbnails), [MonitorYT](https://monitoryt.com/blog/thumbnail-ab-testing), [Mocknex](https://www.mocknex.com/blog/how-to-ab-test-youtube-thumbnails), [Epidemic Sound](https://www.epidemicsound.com/blog/a-b-test-youtube-thumbnails/), [Autonolab](https://blog.autonolab.com/blog/2025-09-25-thumbnail-testing-a-b-testing-visual-packaging/)
- **No published figure exists for how often YouTube tests end with a Winner.** No official or independent rate was found.
- [DATA][VENDOR] **ThumbnailPeak's closest proxy.**
  - 1,696 comparisons, scored by its own model.
  - Where the two thumbnails' scores were **within 2 points (509 comparisons), 79%** ended as "a slight win or a tie".
  - At gaps of **11 or more points (269 comparisons), 10%** did.
  - This measures its own scoring model, not YouTube's winner rate, and does not separate Inconclusive from Performed Same.
  - [ThumbnailPeak](https://thumbnailpeak.com/blog/youtube-thumbnail-ab-testing)

**Pre-native third-party testing (TubeBuddy), for contrast**
- [VENDOR] TubeBuddy needs **95% statistical significance** before declaring a winner. Its Legend-plan test **rotates two thumbnails every 24 hours**. — [TubeBuddy Thumbnail A/B Test tool](https://www.tubebuddy.com/tools/youtube-thumbnail-test); [TubeBuddy blog](https://www.tubebuddy.com/blog/a-b-testing-youtube-ctr/)
- [VENDOR] **TubeBuddy reports relative lift.**
  - Its worked example: **4.38% → 5.2% CTR is reported as +18.8%**. The absolute gain of +0.82 points is "a number that we don't report."
  - A separate blog example showed a variation with "3.8% greater" CTR.
  - These are illustrations, not a dataset.
  - [TubeBuddy Support: A/B Testing Notes](https://support.tubebuddy.com/hc/en-us/articles/9324340751771-A-B-Testing-Notes); [TubeBuddy blog](https://www.tubebuddy.com/blog/a-b-testing-youtube-ctr/)

**What creators say they learned**
- [EXPERT] **Linus Tech Tips.** LTT released a video titled **"We Need to Change Our Thumbnails NOW"** about YouTube's **"new A/B/C thumbnail tester to figure out what makes YOU stick around and watch more of the video."** Viewers also noticed LTT thumbnails changing within about an hour of upload, which forum users attributed to testing; this was not confirmed. — [LTT forum thread](https://linustechtips.com/topic/1575263-we-need-to-change-our-thumbnails-now/); [TheTVDB episode listing](https://thetvdb.com/series/linus-tech-tips/episodes/10569350)
- [EXPERT] **Veritasium.**
  - Derek Muller says YouTube's analytics, "a lot of his own experimentation and research", made him much better at titles and thumbnails after he started out poor at them. — [Third Law Reaction review](https://www.thirdlawreaction.com/shocking-secret-behind-clickbait/)
  - A Hacker News commenter says Veritasium tests which thumbnails and titles work. This is anecdotal. — [Hacker News](https://news.ycombinator.com/item?id=28265912)
- [EXPERT] **MrBeast.** His team's analytics platform, **ViewStats**, prioritizes CTR, average view duration and average view percentage, the same three metrics the leaked guide centers on. — [Tubefilter](https://www.tubefilter.com/2024/09/17/mrbeast-internal-production-guide-leaked-key-points/)

### Inferences
- **Optimize for "qualified clicks", not raw CTR.** YouTube's own testing judges watch time share, so a lower-CTR variant that attracts better-matched viewers can and should win. Packaging that overpromises will tend to lose in YouTube's own A/B system.
- **Test concepts, not tweaks.** Near-identical variants (font color, a single word) mostly end Inconclusive or Performed Same. Test meaningfully different *angles*: a different subject, emotion, stakes, or title promise. Use all 3 slots, and don't edit mid-test because that kills it.
- **Treat an Inconclusive result as information.** It means the variants were interchangeable at that traffic level. Pick the one that best matches the content and move on.
- **Prefer native testing over manual rotation.** Manual "swap every 24h" testing (the TubeBuddy model, or creators swapping by hand) is confounded by time-of-day, video age and traffic-source mix. The native tool splits impressions at the same time.
- **Report lifts in absolute points as well as relative percentages.** A "+18.8%" CTR lift can be just +0.8 percentage points.

### Gaps
- **No official statistic** on how often Test & Compare produces a Winner, and **no Creator Insider or YouTube Liaison commentary** was retrievable; YouTube-owned domains were blocked.
- **No published Test & Compare learnings** were found from **MrBeast, Ryan Trahan, Mark Rober, Dude Perfect, Ali Abdaal** or **Veritasium**, beyond the anecdotes above. These likely exist in podcasts and videos (Colin and Samir, Creator Science) that I could not search further.
- **UNVERIFIED background, history:** Test & Compare was announced around VidCon in June 2023 as a limited thumbnail test and rolled out widely to eligible desktop Studio users during 2024. Check at YouTube Help or Creator Insider.

## 3. What packaging principles do top strategists teach (packaging-first ideation, title–thumbnail synergy, "the click is a promise", mobile/TV readability, branding vs novelty)?

### Takeaway
The leading strategists (MrBeast's guide, Paddy Galloway, Ed Lawrence/Film Booth, Jake Thomas/Creator Hooks) converge on a small set of rules:
- **Package before you produce.** An idea that can't be packaged isn't an idea yet.
- **Make the thumbnail pass a split-second glance test**: at most 3 focal points and fewer than 5 words.
- **Make the title and thumbnail complement each other**, never repeat or contradict.
- **Open a curiosity loop**, with extreme-but-true stakes and curiosity paired with desire or fear.
- **Deliver the promised image or payoff immediately.**

### Cited Findings
**Packaging-first ideation**
- [EXPERT] **Paddy Galloway, X post:** "22. Always plan your title and thumbnail before recording, everyone knows this, few do this." — [Paddy Galloway on X](https://x.com/PaddyG96/status/1788967959882346991)
- [EXPERT] **Paddy Galloway, podcast:** if an idea can't be summed up in a title and thumbnail, it isn't yet a viable idea and should be dropped. — [Creator Science podcast](https://podcast.creatorscience.com/paddy-galloway-2/)
- [EXPERT] **Ed Lawrence (Film Booth):** "There's no point wasting my time on a video until I have packaged it."
  - He works on packaging first and doesn't continue until the title is settled.
  - He argues competition is now less about making videos and more about who has the most interesting **idea, thumbnail and title**.
  - [Creator Science: Ed Lawrence](https://podcast.creatorscience.com/ed-lawrence/); [Passionfroot](https://www.passionfroot.me/creators-on-air/mastering-youtube-strategies-with-ed-lawrence)
- [EXPERT] **Film Booth workflow:**
  - Packaging should be **tested with a community before a script is written**. His "Thumbnail University" feedback community was built for this.
  - His collaborator James Kelly starts with packaging (angle, title, thumbnail, early payoff) before scripting.
  - [Starter Story](https://www.starterstory.com/film-booth-breakdown); [Passionfroot](https://www.passionfroot.me/creators-on-air/mastering-youtube-strategies-with-ed-lawrence)
- [EXPERT] **MrBeast guide (2024 leak):**
  - Treats title and thumbnail as the **starting point** of each video.
  - "CTR is what dictates what we do for videos."
  - "'I Spent 50 Hours In My Front Yard' is lame, and you wouldn't click it. But you would click 'I Spent 50 Hours In Ketchup.'" In other words, packaging decides which ideas get made at all.
  - The quotes come from secondary sources quoting the guide.
  - [Creator Handbook](https://www.creatorhandbook.net/leaked-document-allegedly-reveals-mrbeasts-secrets-to-youtube-success-the-key-takeaways/); [Alexander Jarvis memo](https://www.alexanderjarvis.com/memo-how-to-succeed-in-mrbeast-production/); [Tubefilter](https://www.tubefilter.com/2024/09/17/mrbeast-internal-production-guide-leaked-key-points/); [HN thread](https://news.ycombinator.com/item?id=41549649)
- [EXPERT] **Paddy Galloway, via Colin and Samir:** small creators spend most of their time on filming and editing, when **packaging offers more leverage than production**. — [Colin and Samir: The New Rules of YouTube From Paddy Galloway](https://www.colinandsamir.com/resources/the-new-rules-of-youtube-from-paddy-galloway)

**The glance test: small mobile tiles**
- [EXPERT] **Paddy Galloway, X post:** "19. Make sure thumbnail passes the 'glance test' - can you process everything in just a quick glance? Viewer gets just milliseconds to view it as they are scrolling." Elsewhere he recommends **three or fewer focal points** and **fewer than five words**. — [Paddy Galloway on X](https://x.com/PaddyG96/status/1811083499044044951); [Marketing Examined](https://www.marketingexamined.com/blog/paddy-galloway-youtube-guide)
- [EXPERT] **Paddy Galloway:** **what is shown** in the thumbnail (the subject) matters more than design styling. — [Creator Science podcast](https://podcast.creatorscience.com/paddy-galloway-2/)
- [DATA] Too many objects hinder information processing in thumbnails. — [Koh & Cui 2022](https://www.sciencedirect.com/science/article/abs/pii/S0167923622000914)

**Title–thumbnail synergy: complement, don't repeat**
- [EXPERT] **Paddy Galloway, X post:** "20. Don't forget to view the title and thumbnail as one, do they compliment each other or contradict/repeat?" — [Paddy Galloway on X](https://x.com/PaddyG96/status/1811083499044044951)
- [EXPERT] **Ed Lawrence, workshop quote relayed by a third party:** "If your title and thumbnail don't create 3 big questions in the viewer's mind, it's probably not good enough." — [Substack: Everything I've learned about YouTube](https://lelon.substack.com/p/everything-ive-learned-about-youtube)
- [EXPERT] **Ed Lawrence's self-check questions:** "Does the thumbnail grab attention? Does the title accurately describe the video while enticing viewers?" The page was not confirmed; candidates are [Creator Science: Ed Lawrence](https://podcast.creatorscience.com/ed-lawrence/) and [Matthew Pollard interview](https://matthewpollard.com/theintrovertsedge/how-to-make-money-as-an-introvert-on-youtube).
- [EXPERT] **Paddy Galloway's team on open loops:** they describe packaging that creates an **open loop** the viewer wants to close ("unpausing the viewer"). They cite "Pulling up the board" and "Taking next step" styles as examples. — [Paddy Galloway on LinkedIn](https://www.linkedin.com/posts/paddy-galloway-459b8913a_what-do-these-four-viral-youtube-videos-have-activity-7444402853705854978-IsL1)

**Remixing proven packaging**
- [EXPERT] **Ed Lawrence** finds a title or thumbnail that worked in his niche or a wider one, takes one element from another, and pairs them. The result is packaging "proven to get clicks." — [1of10: Film Booth's strategy](https://1of10.com/blog/film-booths-strategy-gaining-millions-views/)
- [EXPERT] **Jake Thomas** shows the same title framework transferring across niches:
  - "Do this and you will never hit a fat iron shot" (golf)
  - "Do this to get them hooked in the early stages of dating" (relationships)
  - [Net Influencer](https://www.netinfluencer.com/creator-hooks-jake-thomas-code-on-clickable-youtube-titles/)
- [EXPERT] **Jake Thomas** calls **timeliness** the most powerful trigger, citing MrBeast's Squid Game video as a trend-riding example. The episode was not confirmed; candidates are [Creator Science #193](https://podcast.creatorscience.com/jake-thomas-2/), [Creator Science #125](https://podcast.creatorscience.com/jake-thomas/) and [Become a Writer Today](https://podcast.becomeawritertoday.com/1055644/episodes/12708192-jake-thomas-of-creator-hooks-talks-headlines-and-thumbnails).

**"The click is a promise"**
- [EXPERT] **MrBeast guide:** the title and thumbnail set the viewer's expectations, and the video must fulfil them.
  - Summaries describe the guide's **"World's Largest Bouncy Castle"** example: a thumbnail of a giant yellow bouncy castle beside huge buildings.
  - If the video then shows a different castle, viewers feel misled and leave.
  - Thumbnails "must align with expectations set by the title."
  - [Creator Handbook](https://www.creatorhandbook.net/leaked-document-allegedly-reveals-mrbeasts-secrets-to-youtube-success-the-key-takeaways/); [Tubefilter](https://www.tubefilter.com/2024/09/17/mrbeast-internal-production-guide-leaked-key-points/)

**Branding**
- [EXPERT] **Linus Sebastian, secondhand quote on LTT's forum:** he is creating "a recognizable brand and a media company, not YouTube videos." The thread was not confirmed; candidates are [LTT forum 1019713](https://linustechtips.com/topic/1019713-clickbait-titles-and-thumbnails/) and [LTT forum 748812](https://linustechtips.com/topic/748812-is-anyone-ok-with-the-new-thumbnails-and-titles/page/2/#comment-9487204).

### Inferences
**Synthesized packaging checklist** (each item traces to a cited rule above):
1. Is the title+thumbnail drafted **before** scripting or filming? If you can't package it, kill or reshape the idea (Paddy, Ed, MrBeast).
2. Does the thumbnail pass the **glance test**: one dominant subject, at most 3 focal points, fewer than 5 words, readable at phone-feed size (Paddy; Koh & Cui; vidIQ text data)?
3. Do title and thumbnail **add different information**? The thumbnail shows the image or stakes; the title adds context or curiosity. They must never repeat or contradict each other (Paddy #20).
4. Does the package raise **about 3 questions** or open a loop the viewer must close (Ed; Paddy's team; Jake)?
5. Does it hit **curiosity plus desire or fear**? Is the framing at the **most extreme that is still true** ("I Survived" > "I Spent"; ketchup > front yard)?
6. Is the hook **specific**, not vague? Vague titles like "I Can't Believe This Happened" only convert existing subscribers (Jake; see Q7).
7. Can the video **show the promised image or payoff in the first minute** (MrBeast's bouncy-castle logic)?
8. Is there a timely angle (Jake)? Is the pattern borrowed from a proven outlier (Ed)?
9. Make 2–3 genuinely different variants and run Test & Compare (Q2).

**Branding vs novelty.** The data and advice lean toward **subject and idea over house style**: "what's shown matters more than design," and the evidence on faces and contrast varies by niche. Recognizable branding (LTT) is a long-term asset, but no source showed a measured CTR effect of consistent styling.

### Gaps
- **No retrieved evidence on designing for TV screens.**
  - **UNVERIFIED background:** YouTube CEO Neal Mohan's February 2025 annual letter reportedly said TV has surpassed mobile as the primary device for YouTube viewing in the US. Check this on blog.youtube.
  - Implication, to be treated as an inference only: packages must read both as a tiny mobile tile and on a large 10-foot screen, so simple, high-legibility compositions are the safe choice.
- **No data comparing branding consistency with novelty** for CTR or satisfaction.
- **Not retrieved:**
  - Colin and Samir's own packaging-first content (only their Paddy Galloway resource page)
  - MrBeast interviews outside the leaked guide
  - Veritasium's "Clickbait is Unreasonably Effective" transcript
  - Mark Rober, Ryan Trahan, Dude Perfect and Ali Abdaal on packaging

## 4. What CTR benchmarks are realistic, and how should CTR be judged (traffic source, impression volume, audience temperature)?

### Takeaway
YouTube's only official benchmark is that **half of all channels and videos have an impressions CTR between 2% and 10%**. The range is wider for videos under a week old or with fewer than 100 views. CTR varies by content type, audience and **where the impression was shown**.

CTR should therefore be judged **against the channel's own baseline, per traffic source and at comparable impression volumes**. Higher CTR is not the goal in itself: YouTube's own A/B tool ignores CTR in favor of watch time share.

### Cited Findings
- [OFFICIAL] "Half of all channels and videos on YouTube have an impressions CTR that can range between **2% and 10%**." New videos or channels (e.g., less than a week old) or videos with fewer than 100 views "can see an even wider range." CTR "will vary based on the type of content, audience, and where on YouTube the impression was shown." The page frames this as context, not a target. — [YouTube Help: Impressions & CTR FAQs](https://support.google.com/youtube/answer/7628154?hl=en)
- [VENDOR] **Third-party benchmarks are not YouTube's.** Secondary sites add figures such as "4–5% for successful channels." Specific MrBeast CTR figures such as "8–18%" come from a thumbnail-tool vendor's marketing page and are not in the leaked guide. — [Teleprompter](https://www.teleprompter.com/blog/whats-a-good-click-through-rate-on-youtube); [OutlierKit](https://outlierkit.com/resources/youtube-click-through-rate/); [Mediacube](https://mediacube.io/en/blog/youtube-click-through-rate). The "8–18%" caveat comes from a search summary that did not name the vendor page; the likeliest candidate is [ThumbnailMaker.ai](https://thumbnailmaker.ai/mrbeast-thumbnail-maker) (not confirmed).
- [OFFICIAL, via third parties] **Test & Compare decides on watch time share, not CTR.** One source notes "no CTR data" is shown in title tests. — [Search Engine Journal](https://www.searchenginejournal.com/youtube-title-a-b-testing-rolls-out-globally-to-creators/562571/); [ThumbnailPeak](https://thumbnailpeak.com/blog/youtube-thumbnail-ab-testing)
- [EXPERT] **MrBeast's guide** tracks CTR together with average view duration and average view percentage, never alone. — [Tubefilter](https://www.tubefilter.com/2024/09/17/mrbeast-internal-production-guide-leaked-key-points/)

### Inferences
- **The 2–10% band is a sanity check, not a goal.** A 3% CTR on a video receiving millions of Browse impressions can be a hit; a 12% CTR on 2,000 subscriber-only impressions may not scale.
- **Compare like with like.** Use the same traffic source (Browse/Home vs Suggested vs Search), similar impression volumes, and the same time window since publish (first 24h vs day 7), against the channel's own median.
- **Expect CTR to fall as a video spreads.** Impressions shown to colder, non-subscriber audiences (Home/Suggested at scale) are less pre-qualified. Falling CTR with rising impressions is usually expansion, not failure. This is inferred from YouTube's statement that CTR varies by audience and placement; a direct official quote was not retrieved.
- **Diagnose with the CTR–retention pair:**
  - Low CTR with strong retention: re-package (see Q5).
  - High CTR with weak early retention: possible over-promise (see Q7).

### Gaps
- **No official YouTube quote retrieved** stating that CTR typically declines as impressions grow. Creator Insider and YouTube Liaison material was unreachable (blocked domains).
- **No traffic-source-specific CTR benchmarks** from an authoritative source; YouTube publishes none in the retrieved material.
- **UNVERIFIED background:** YouTube counts an impression when a thumbnail is shown for more than 1 second with at least 50% of it visible. Impressions on external sites/embeds are excluded, so external traffic isn't in impressions CTR. Check on the same Help page (support.google.com/youtube/answer/7628154).

## 5. How and when should creators change titles/thumbnails after publishing (swapping after 24–72h, reviving old videos), and what evidence exists that it works?

### Takeaway
The best-supported mechanism is **native Test & Compare**: up to 3 variants, simultaneous split, judged on watch time share, with no mid-test edits. The common "swap after 24–72 hours" rule is **creator folk practice without published large-scale evidence**.

The most credible expert pattern is to **re-package videos that retain well but get clicked poorly** (Ed Lawrence). Evidence that it works is anecdotal.

### Cited Findings
- [EXPERT] **Ed Lawrence** revisits older videos with **high watch time but low click-through rates** and changes their titles and thumbnails to re-engage viewers. — [Passionfroot: Ed Lawrence](https://www.passionfroot.me/creators-on-air/mastering-youtube-strategies-with-ed-lawrence); [Creator Science: Ed Lawrence](https://podcast.creatorscience.com/ed-lawrence/)
- [OFFICIAL] **During a test, changing the title or thumbnail stops it automatically**, and the test must be restarted. Tests should complete within two weeks. — [YouTube Help](https://support.google.com/youtube/answer/16391400?hl=en-GB)
- [VENDOR] **TubeBuddy's legacy approach** switches between two thumbnails **every 24 hours** until 95% significance. Third-party guides suggest 3–7 days, or winners "typically 24–48 hours depending on view volume"; these estimates conflict and none is backed by data. — [TubeBuddy tool](https://www.tubebuddy.com/tools/youtube-thumbnail-test). The duration claims appeared in one search summary covering several pages, e.g. [Fikaclip](https://fikad.boo/en/blog/youtube-thumbnail-ab-testing-tubebuddy), [OpusClip](https://www.opus.pro/blog/best-youtube-thumbnail-ab-testing-tools) and [TubeAnalytics](https://www.tubeanalytics.net/blog/thumbnail-ab-testing-platforms); which page said which was not confirmed.
- [EXPERT/ANECDOTE] **LTT viewers** noticed thumbnails changing shortly after upload, "to like an hour later." The likely cause is A/B/C testing (LTT's own video "We Need to Change Our Thumbnails NOW"), but this was not confirmed. The thread holding the observation was not confirmed either. — [LTT forum: We Need to Change Our Thumbnails NOW](https://linustechtips.com/topic/1575263-we-need-to-change-our-thumbnails-now/); [LTT forum 748812](https://linustechtips.com/topic/748812-is-anyone-ok-with-the-new-thumbnails-and-titles/page/2/#comment-9487204)
- [EXPERT/ANECDOTE] **Jake Thomas** is credited with a video reaching about **7 million views** where similar niche videos got about **1 million**, attributed to "changing one thing." The search summary did not confirm whether that was a post-publish change. Separately, in a podcast episode, he describes a title that earned **6,000,000 more views than a competitor's**. The episode was not confirmed; candidates are Creator Science #125 or #193. — [Niche Pursuits](https://www.nichepursuits.com/jake-thomas-youtube-video/); [Creator Science #125](https://podcast.creatorscience.com/jake-thomas/); [Creator Science #193](https://podcast.creatorscience.com/jake-thomas-2/)

### Inferences
**Practical protocol, synthesized from the cited rules:**
1. Launch with your strongest package, plus 2 genuinely different alternates loaded into Test & Compare from day one. This replaces manual 24–72h swaps with a simultaneous, confound-free test.
2. Do not edit the title or thumbnail while a test runs.
3. If there is no test and the video is clearly below the channel's own same-age baseline on CTR from Browse/Suggested after the first day or two, while retention or AVD is normal, a re-package is the highest-leverage fix.
4. If CTR is fine but retention is poor, the problem is the content–promise match or the hook, not the package (see Q7).
5. **Evergreen back-catalogue:** periodically audit videos with **above-median retention but below-median CTR** (Ed Lawrence's criterion). Re-package them with a fresher angle or a more extreme-but-true framing, ideally via Test & Compare. These are the best candidates to revive.
6. Judge outcomes on watch time and views per impression over comparable windows. A raw CTR jump after a swap is confounded by changes in traffic mix.

### Gaps
- **No large-scale or independent evidence** found on (a) the effect size of post-publish swaps or (b) the optimal timing (24h vs 72h vs a week).
- **UNVERIFIED background:** YouTube Liaison Rene Ritchie has publicly said that changing a video's title or thumbnail does not penalize it and can help it reach new audiences. Exact quotes were not retrievable; YouTube domains were blocked.
- **No published revival case studies** with numbers from named large creators (MrBeast, LTT, Veritasium, Ali Abdaal) were retrieved.

## 6. What are proven title formulas and thumbnail archetypes for different video types (challenge/entertainment, education/explainer, tutorial/how-to, commentary, vlog, review)? Real high-performing examples.

### Takeaway
The most transferable formulas are:
- **Extreme-stakes challenge**: "I Survived [extreme] for [time]", "Last to [X] wins $[Y]", "$1 vs $[huge] [thing]"
- **Curiosity explainer**: "Why [surprising specific fact]?", "The [superlative] [thing] no one [verb]"
- **Promise tutorial**: "Do this to [desired outcome]", "If I started [X] today, this is what I'd do"
- **Open-loop commentary**: "[Person] FINALLY DID IT…"

Thumbnails should show **one striking subject**, often with **a face reacting to it** or **a scale/contrast comparison**, and at most 0–3 words. View counts could not be verified in this session, so the examples below are sourced for their *existence and wording* only; a separate list of candidates is quarantined in Gaps.

### Cited Findings
**Sourced formulas and examples**
- [EXPERT] **Creator Hooks**, "5 YouTube Title Formulas You Need To Know," including **"If I started (Activity) TODAY, this is what I would do."** — [Creator Hooks](https://creatorhooks.com/5-youtube-title-formulas-you-need-to-know/)
- [EXPERT] **Jake Thomas, open-loop titles** start a story without finishing it. Examples:
  - **"BRONNY JAMES FINALLY DID IT…"**
  - titles that use "this" without saying what "this" is
  - [Net Influencer](https://www.netinfluencer.com/creator-hooks-jake-thomas-code-on-clickable-youtube-titles/); [Passionfroot: Jake Thomas](https://www.passionfroot.me/creators-on-air/how-to-write-youtube-titles-to-get-more-views-with-jake-thomas)
- [EXPERT] **Jake Thomas, cross-niche "Do this" formula:**
  - **"Do this and you will never hit a fat iron shot"** (golf)
  - **"Do this to get them hooked in the early stages of dating"** (relationships)
  - [Net Influencer](https://www.netinfluencer.com/creator-hooks-jake-thomas-code-on-clickable-youtube-titles/)
- [EXPERT] **MrBeast guide, challenge wording:**
  - "**I Spent 50 Hours In Ketchup**" vs "I Spent 50 Hours In My Front Yard" (an illustrative pair, not real videos)
  - **"I Survived" > "I Spent"**
  - "the more extreme the better"
  - [MrBeast guide PDF](https://cdn.prod.website-files.com/6623b7720b009050313e701c/66ede69453b7bbadcd2f05a8_How-To-Succeed-At-MrBeast-Production%20(2).pdf); [Creator Handbook](https://www.creatorhandbook.net/leaked-document-allegedly-reveals-mrbeasts-secrets-to-youtube-success-the-key-takeaways/)
- [EXPERT] **MrBeast guide, thumbnail archetype "giant subject vs. familiar scale reference":** a giant yellow bouncy castle beside huge buildings, for a "World's Largest Bouncy Castle" title. — [Creator Handbook](https://www.creatorhandbook.net/leaked-document-allegedly-reveals-mrbeasts-secrets-to-youtube-success-the-key-takeaways/)
- [EXPERT] **Timeliness:** MrBeast's Squid Game video, cited by Jake Thomas as the archetypal trend-riding package. — [Creator Science #193](https://podcast.creatorscience.com/jake-thomas-2/)
- [FACT] **"50 YouTubers Fight for $1,000,000"** is a MrBeast video with its own Wikipedia article. It fits the "[N] [people] fight for $[big prize]" formula. — [Wikipedia](https://en.wikipedia.org/wiki/50_YouTubers_Fight_for_$1,000,000)
- [FACT] **Veritasium, "Clickbait is Unreasonably Effective"** (Aug 17, 2021; about 19 min). Its working title was **"We Need To Talk About Clickbait"**. My inference: it was re-titled from a topic label to a counter-intuitive claim. — [TheTVDB](https://thetvdb.com/series/veritasium/episodes/8617959)
- [FACT] **LTT, "We Need to Change Our Thumbnails NOW"**: an urgency, "we need to" framing. — [LTT forum](https://linustechtips.com/topic/1575263-we-need-to-change-our-thumbnails-now/)
- [EXPERT] **Paddy Galloway's team** cites "Pulling up the board" and "Taking next step" thumbnail/title styles as open-loop examples. The exact meaning was not retrievable. — [LinkedIn](https://www.linkedin.com/posts/paddy-galloway-459b8913a_what-do-these-four-viral-youtube-videos-have-activity-7444402853705854978-IsL1)
- [ANECDOTAL DATA] **Jake Thomas**'s channels and titles are credited with **100M+ views**, including one video at about **7M views vs about 1M** for similar niche videos. — [Niche Pursuits](https://www.nichepursuits.com/jake-thomas-youtube-video/); [Net Influencer](https://www.netinfluencer.com/creator-hooks-jake-thomas-code-on-clickable-youtube-titles/)
- [DATA] **Thumbnail archetype evidence:**
  - Face reacting to the subject, and multi-face over single-face (1of10 vendor claim; 1of10 Media 300k study)
  - Face presence common among breakouts (vidIQ 69–80%)
  - Minimal text (vidIQ: 52% of breakouts use 0–3 words)
  - [vidIQ](https://vidiq.com/research/youtube-thumbnail-study/); [Search Engine Journal](https://www.searchenginejournal.com/do-faces-help-youtube-thumbnails-heres-what-the-data-says/563944/); [1of10](https://1of10.com/blog/youtube-thumbnail-trends-2026/)

### Inferences
The formula map below is synthesized from the cited patterns. The bracketed examples are templates, not real videos unless sourced above.

| Video type | Title formulas | Thumbnail archetype |
|---|---|---|
| **Challenge / entertainment** | "I Survived [N] [hours/days] in/at [extreme place]"; "Last To [action] Wins $[X]"; "$1 vs $[huge] [thing]"; "[N] [group] vs [N] [group] for $[X]"; "[N] [people] Fight For $[X]"; "I Spent [N] Hours In [absurd substance/place]" | One giant or absurd subject plus a reacting face; scale reference (bouncy castle next to buildings); split-screen tier comparison; 0–2 words or a bold number |
| **Education / explainer** | "Why [surprising specific fact]?"; "The [superlative] [problem/thing] No One Can [verb]"; "The Big Misconception About [topic]"; "[Topic]'s Fundamental Flaw"; "How [X] Was [Invented/Discovered]" (Veritasium-style; examples quarantined in Gaps) | One intriguing object or diagram with a single visual anomaly; optional presenter face showing puzzlement or awe; 0–3 words that pose the question without repeating the title |
| **Tutorial / how-to** | "Do this to [desired outcome]"; "Do this and you'll never [painful mistake] again"; "If I started [X] TODAY, this is what I'd do"; "How to [outcome] (without [pain])" | Before/after or result-first image; mistake vs fix split; 1–3 words naming the outcome |
| **Commentary / news** | "[Person/brand] FINALLY DID IT…"; "What Happened to [X]?"; "The [Fall/Truth] of [X]" | Recognizable person or logo with an emotive expression; a single "evidence" element; avoid fake-news styling (see Q7) |
| **Vlog / personal challenge** | "I [did unusual thing] for [time]"; "I Tried [X] For 30 Days"; "We Need To [urgent action]" | Self in an unusual setting, mid-action; the strongest single frame of the story |
| **Review / tech** | Strong verdict plus superlative ("The Worst [product] I've Ever Reviewed… For Now"); "$[cheap] vs $[expensive] [product]"; "Don't Buy [X] Until…" | Product held or shown at scale with a reacting face; versus layout; 0–2-word verdict |

- **Across all types:**
  - Put the **concrete, curiosity-generating noun or number** first.
  - Keep titles **about 50–60 characters or less**.
  - Make the thumbnail carry the **image/stakes** and the title carry the **context/question**.
  - Pair curiosity with desire or fear.
  - Choose the **most extreme claim that is still literally true**.

### Gaps
- **Verified view counts could not be collected.** The web-search budget was exhausted and youtube.com, socialblade and similar sources were blocked, so the "30+ examples with view counts" requirement could not be met with verified numbers.
- **UNVERIFIED candidate examples** (real titles recalled by the researcher; exact wording should be checked on YouTube or ViewStats; view counts deliberately omitted):
  - **MrBeast (challenge/entertainment):**
    1. "$456,000 Squid Game In Real Life!"
    2. "I Spent 50 Hours Buried Alive"
    3. "Ages 1 - 100 Fight For $500,000"
    4. "$1 vs $1,000,000,000 Yacht!"
    5. "1,000 Blind People See For The First Time"
    6. "Last To Leave Circle Wins $500,000"
    7. "I Built 100 Wells In Africa"
    8. "Would You Fly To Paris For A Baguette?"
    9. "I Survived 50 Hours In Antarctica"
    10. "7 Days Stranded At Sea"
    11. "I Spent 7 Days In Solitary Confinement"
  - **Veritasium (explainer):**
    1. "Why Are 96,000,000 Black Balls on This Reservoir?"
    2. "The Simplest Math Problem No One Can Solve - Collatz Conjecture"
    3. "The Big Misconception About Electricity"
    4. "Math's Fundamental Flaw"
    5. "How Imaginary Numbers Were Invented"
    6. "The Surprising Genius of Sewing Machines"
    7. "Why No One Has Measured The Speed Of Light"
  - **Mark Rober (engineering/entertainment):**
    1. "Glitter Bomb 1.0 vs Porch Pirates"
    2. "Backyard Squirrel Maze 1.0- Ninja Warrior Course"
    3. "Can You Fool A Self Driving Car?"
  - **Review:** MKBHD, "The Worst Product I've Ever Reviewed... For Now" (Humane AI Pin, 2024).
  - **Explainer / story:** Kurzgesagt, "Optimistic Nihilism"; Kurzgesagt, "The Egg - A Short Story".
  - **Packaging stunt:** Tom Scott, "This Video Has [N] Views" (a title that auto-updates with the live view count).
  - **Study tutorial:** Ali Abdaal, "How to Study for Exams - Evidence-based Revision Tips".
  - **Older (2016) trick-shot:** Dude Perfect, "Water Bottle Flip 2".
- **No retrieved data on arrows/circles** or "mystery object" thumbnail archetypes. No archetype-level performance comparisons by video type exist in the retrieved sources.

## 7. Where is the line between effective curiosity and misleading clickbait that triggers dissatisfaction signals?

### Takeaway
The line is **deliverability**. Curiosity that the video pays off ("legitbait") is rewarded. A package that promises something the video doesn't contain ("clicktrap") is now:
- **penalized by YouTube's own A/B metric**, watch time share;
- **subject to removal** under YouTube's "egregious clickbait" enforcement (India-first, announced Dec 2024);
- **corrosive to trust**, according to academic work.

Vagueness is a separate failure: it doesn't mislead, but it doesn't convert new viewers either.

### Cited Findings
- [OFFICIAL] **YouTube's "egregious clickbait" crackdown, announced December 18, 2024.**
  - "We're strengthening our efforts to tackle egregious clickbait on YouTube."
  - It targets titles or thumbnails that **promise something the video doesn't deliver**, with extra scrutiny of **breaking news and current events**.
  - Examples: a video titled **"The President Resigned!"** that doesn't cover a resignation, and a **"Top Political News"** thumbnail on a video with no news.
  - Offending videos are **removed, without channel strikes** at first.
  - Rollout: "We'll start by slowly rolling this out in India over the coming months."
  - [TechCrunch](https://techcrunch.com/2024/12/18/youtube-says-it-will-start-cracking-down-on-videos-with-clickbait-titles-in-india); [Tubefilter](https://www.tubefilter.com/2024/12/19/youtube-clickbait-crackdown-india-egregious-misleading-videos/); [Storyboard18](https://www.storyboard18.com/digital/youtube-to-crack-down-on-egregious-clickbait-in-india-51429.htm)
- [OFFICIAL, critique] **YouTube's blog doesn't clearly define** what makes clickbait "egregious" as opposed to less severe forms. — [Medianama](https://www.medianama.com/2024/12/223-youtube-to-begin-crackdown-on-egregious-clickbait-india/)
- [OFFICIAL] **Test & Compare promotes the variant with the highest watch time share, not the highest CTR.** A package that wins clicks but loses viewers therefore loses the test. — [YouTube Help](https://support.google.com/youtube/answer/16391400?hl=en-GB); [Search Engine Journal](https://www.searchenginejournal.com/youtube-title-a-b-testing-rolls-out-globally-to-creators/562571/)
- [EXPERT] **Veritasium's "Clickbait is Unreasonably Effective" (2021)** splits clickbait into two kinds:
  - **"Legitbait"**: honest packaging that piques curiosity without overpromising.
  - **"Clicktraps"**: packaging that doesn't deliver.
  - The video's episode listing/description states that "the title and thumbnail play a huge role in a video's success or failure."
  - [Third Law Reaction](https://www.thirdlawreaction.com/shocking-secret-behind-clickbait/); [TheTVDB](https://thetvdb.com/series/veritasium/episodes/8617959); [Hacker News](https://news.ycombinator.com/item?id=28265912)
- [EXPERT] **MrBeast guide:** packaging sets expectations, and the video must immediately fulfil the specific promised visual. If the promised castle isn't the one shown, "viewers feel misled and leave." — [Creator Handbook](https://www.creatorhandbook.net/leaked-document-allegedly-reveals-mrbeasts-secrets-to-youtube-success-the-key-takeaways/)
- [EXPERT] **Jake Thomas: the biggest title mistake is being too vague.** Titles like "I Can't Believe This Happened" may get subscribers to click "but they don't help bring in new viewers." — [Net Influencer](https://www.netinfluencer.com/creator-hooks-jake-thomas-code-on-clickable-youtube-titles/); [Passionfroot](https://www.passionfroot.me/creators-on-air/how-to-write-youtube-titles-to-get-more-views-with-jake-thomas)
- [ACADEMIC] **Clickbait thumbnail aesthetics** (emotional imagery, emojis, curiosity-inducing text–image pairing) "can be effective in the short term, but can also mislead viewers and have a negative impact on the credibility and trustworthiness" of outlets. This comes from a news-thumbnail context. — [Clickbait Aesthetics PDF](https://pdfs.semanticscholar.org/c6ef/6cd28a85f864533800b6927aa082caa68dc6.pdf)
- [EXPERT/COMMUNITY] **Audience friction with heavy clickbait:**
  - LTT's community has repeatedly pushed back on "obnoxious" titles and thumbnails.
  - A forum user recalls Linus reaching a "compromise" with the audience because YouTube "favors" such packaging.
  - This is a secondhand recollection.
  - [LTT forum: Please remember your promise to compromise on clickbait](https://linustechtips.com/topic/1155699-please-remember-your-promise-to-compromise-on-clickbait-descriptive-titles/); [LTT forum: Clickbait titles and thumbnails](https://linustechtips.com/topic/1019713-clickbait-titles-and-thumbnails/)

### Inferences
**A practical "promise test"** before publishing, synthesized from the above:
1. **Literal truth:** is every claim or visual in the title and thumbnail literally true of this video? No fabricated events, results or objects; nothing staged in the thumbnail that the video doesn't contain.
2. **Fast payoff:** does the video show the promised image or answer the core question **early**, ideally in the first minute? Curiosity can stay open for the full video only if the viewer sees progress toward it.
3. **Extreme but accurate:** choose the most dramatic **accurate** framing ("Survived" is legitimate only if real danger or hardship exists).
4. **No borrowed authority:** avoid news-style or official-looking packaging ("BREAKING", "resigned", "Top Political News") unless the video is actually news. This is the exact pattern YouTube is removing.
5. **Specific, not vague:** pair the curiosity gap with a concrete subject (Jake), so the click is chosen by people who will enjoy the video. This raises watch time share, the metric YouTube actually optimizes in tests.

**Dissatisfaction signals to monitor after publish:**
- high CTR with a sharp early retention drop
- a below-baseline average view percentage
- "not interested" feedback and comments calling out the bait

These indicate a promise mismatch. Fix it by re-packaging toward accuracy, not by adding more bait.

### Gaps
- **UNVERIFIED background, official:** YouTube's September 2021 blog post by Cristos Goodrow, "On YouTube's recommendation system," reportedly:
  - explains that **clicks alone can be misleading** (clickbait)
  - says YouTube added **watch time** in 2012
  - says it uses **viewer satisfaction surveys** ("valued watchtime"), alongside likes, dislikes, shares and "not interested"
  - Check at https://blog.youtube/inside-youtube/on-youtubes-recommendation-system/ (domain blocked in this session).
- **No quantitative data** was retrieved linking specific clickbait features to YouTube's satisfaction-survey or "not interested" rates. Evidence for the CTR–satisfaction tradeoff is indirect: the watch-time-share test metric, the enforcement policy and the academic credibility findings.
- **Enforcement status unknown:** whether the egregious-clickbait enforcement has expanded beyond India as of late 2026 could not be verified.

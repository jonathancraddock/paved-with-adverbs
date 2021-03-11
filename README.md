# Paved With Adverbs

>I believe the road to hell is paved with adverbs, and I will shout it from the rooftops. To put it another way, they're like dandelions. If you have one on your lawn, it looks pretty and unique. If you fail to root it out, however, you find five the next day... fifty the day after that... and then, my brothers and sisters, your lawn is totally, completely, and profligately covered with dandelions. By then you see them for the weeds they really are, but by then it's—GASP!!—too late.

*Stephen King, On Writing*

## What is this?

It's currently an exception custom dictionary, for use in LibreOffice.

My end goal is to highlight adverb use in a LibreOffice document, in real-time, whilst typing. Adding an *exception* dictionary results in a custom set of words being underlined, as a spelling mistake. It's not ideal, but it's a stepping stone while I think of a better approach.

To build the word list I found half a dozen lists of common adverbs, merged them, and removed duplicates. It's subjective, but I don't accept that a word like "not" is among the more evil adverbs, and so I removed it. And, I'm in two minds regarding potential-adverbs, such as "always", or "never". None of the lists I found online, so far, included the word "completely"; or "profligately" for that matter. 

> 8th March 2021: Apart from some existing lists' inadequacies, I've found there are some novel interpretations of the CSV format when it comes to dictionary files! This project may be a work in progress but, if nothing else, I've attached a sensibly formated version of the OPTED v0.03 dictiorary as a single Libre Office "Calc" ODS file. It contains 176,049 words in three columns; word, category, definition.

But, should I *even* include "even"... when it can function as a noun, or an adjective, or an adverb, or a verb?

## Working Source Dictionary v1 (28th Feb 2021)

I don't know if I can make this work, or not, but it's becoming clear the adverb lists I've found so far are a bit rubbish! It needs a different approach and I'm now working with the OPTED v0.03. My first attempt to manipulate its CSV files led to some inconsistencies and, because this is a one-off task, I merged them into a single Libre Office Calc speadsheet and filtered the resulting list.

> Link to OPTED v0.03, the Online Plain Text English Dictionary: http://www.mso.anu.edu.au/%7Eralph/OPTED/

The usage conditions of this dictionary are that its content must remain in the public domain and in plain format. I've attached the entire working dictionary file - hope it might be useful to someone!

I now have a list of **3791** adverbs, of which **2757** end in -LY.

## Working Source Dictionary v2 (7th Mar 2021)

The file `OPTED_Adverbs_07mar2021.ods` uses the same OPTED v0.03 source files, but I wrote a better parsing macro to turn them into actual CSV files, as opposed to a series of 26 plain text files that had been given the file-extension "csv". ;-)

> 8th March 2021: The current list contains **3451** adverbs, which may appear a step backward, but it's more refined, eliminating several words that might see only very occasional use as an adverb.

## Working Source Dictionary v3 (11th Mar 2021)

Well- if nothing else, this has been an interesting exploration. (So far!)

Having discovered the existance of "Corpus Lists" I found the following website from Adam Kilgarriff (1960-2015) that collects a variety of lemmatised frequency lists. In particular, the list below includes the 6,318 most frequently used words from the British National Corpus.

> http://www.kilgarriff.co.uk/bnc-readme.html

From this list, 427 words are (or may be used as) adverbs. As a cross-check, the website https://prowritingaid.com/ allows you to check a passwage of 500 words on their free tier. Convenient, I thought, and so I pasted those 427 words and ran the Adverb report. This step narrows the list down to 227. They exclude 10 adverbs of time (eg/ regularly, annually, rarely) and they exclude adverbs more commonly seen in other useage.

Take "no" for example. It could be an adverb, but that **is *no* concern** of mine. You see what I did there? ;-) In this context you don't expect words like "no", "forward", "short", or "half", to be highlighted by a simple grammar and style macro.

A typical English speaker has a vocabulary between 20,000-35,000 words. I would like to try this approach with a longer lemmatised list. But, those initial 227 words include many of the most egregious adverbs.


## What's next?

- [ ] In Libre Office, I would prefer adverbs to be highlighted using a different colour, to distinguish them from actual spelling errors. There does not appear to be any way to do that with a custom dictionary, perhaps a macro is required, but either way, that's a work in progress.

> A blog post discussing macros to highlight "confusables" - https://www.louiseharnbyproofreader.com/blog/using-proofreading-macros-highlighting-confusables-with-comparewordlist

- [X] Build and refine a more comprehensive custom dictionary.


## Footnote - 227 Common Adverbs

This is the shortlist of 227 common adverbs, with "really" in first place!

```text
Order,Frequency,Word
194	48062	really
364	27303	probably
385	25990	actually
468	22002	particularly
541	19151	usually
560	18647	certainly
584	17756	simply
586	17694	especially
668	15349	clearly
825	12381	quickly
834	12249	recently
863	11795	suddenly
884	11484	nearly
915	11014	obviously
941	10729	exactly
1021	9877	easily
1045	9652	immediately
1103	9132	highly
1130	8911	fully
1136	8873	slightly
1147	8801	hardly
1152	8784	directly
1177	8605	completely
1247	7914	slowly
1248	7912	relatively
1272	7696	apparently
1292	7596	merely
1321	7350	largely
1342	7211	possibly
1350	7180	carefully
1371	7065	mainly
1374	7050	currently
1406	6892	entirely
1408	6873	previously
1423	6814	extremely
1438	6702	fairly
1454	6634	increasingly
1468	6553	equally
1513	6352	surely
1642	5807	totally
1651	5782	absolutely
1668	5706	partly
1670	5699	seriously
1678	5670	necessarily
1680	5667	properly
1694	5610	widely
1714	5521	closely
1845	5048	effectively
1968	4612	unfortunately
1977	4590	strongly
1986	4558	rapidly
2006	4502	similarly
2011	4492	originally
2028	4439	perfectly
2044	4398	virtually
2072	4329	badly
2127	4179	significantly
2131	4172	naturally
2146	4140	quietly
2177	4079	heavily
2198	4030	gently
2221	3979	firmly
2241	3928	mostly
2276	3828	shortly
2277	3824	initially
2312	3755	specifically
2318	3741	deeply
2342	3677	subsequently
2347	3654	gradually
2361	3631	essentially
2438	3486	precisely
2490	3373	successfully
2509	3335	greatly
2531	3280	briefly
2532	3279	presumably
2564	3213	respectively
2573	3201	truly
2596	3159	definitely
2608	3137	primarily
2624	3116	basically
2648	3084	inevitably
2667	3057	reasonably
2754	2914	considerably
2772	2879	ultimately
2776	2871	secondly
2798	2837	approximately
2819	2805	readily
2831	2789	deliberately
2832	2787	automatically
2877	2724	newly
2932	2635	personally
2955	2586	surprisingly
2969	2562	purely
2973	2554	commonly
2974	2552	sufficiently
3024	2481	consequently
3040	2463	softly
3046	2459	sharply
3062	2437	potentially
3096	2393	undoubtedly
3120	2370	notably
3172	2320	roughly
3206	2293	barely
3214	2288	accordingly
3238	2249	wholly
3281	2206	formally
3313	2164	namely
3349	2131	typically
3374	2107	thoroughly
3425	2054	traditionally
3496	1989	literally
3503	1980	physically
3522	1965	specially
3534	1958	strictly
3535	1958	desperately
3540	1954	lightly
3549	1943	mentally
3597	1914	correctly
3608	1902	sadly
3659	1872	hopefully
3672	1865	formerly
3752	1805	locally
3793	1783	officially
3809	1775	happily
3817	1770	simultaneously
3832	1763	severely
3833	1762	separately
3880	1734	safely
3894	1723	alternatively
3912	1711	substantially
3930	1696	firstly
3932	1695	politically
3946	1681	steadily
3958	1675	scarcely
3975	1663	solely
4011	1644	consistently
4078	1608	instantly
4091	1602	broadly
4102	1591	fortunately
4111	1584	publicly
4116	1581	freely
4160	1556	invariably
4197	1541	differently
4209	1536	dramatically
4229	1525	socially
4294	1493	actively
4299	1489	remarkably
4337	1471	tightly
4388	1447	reportedly
4396	1443	evidently
4436	1423	accurately
4455	1414	genuinely
4473	1407	practically
4518	1388	independently
4551	1370	honestly
4580	1358	rightly
4616	1337	positively
4638	1329	importantly
4639	1329	continually
4662	1313	utterly
4676	1307	partially
4691	1299	explicitly
4721	1288	repeatedly
4724	1287	temporarily
4801	1258	terribly
4822	1248	predominantly
4849	1241	beautifully
4855	1239	neatly
4867	1234	openly
4884	1229	permanently
4887	1228	seemingly
4900	1224	swiftly
4948	1209	privately
4961	1201	silently
4989	1192	comparatively
5058	1165	ideally
5097	1149	adequately
5106	1146	abruptly
5116	1143	legally
5134	1135	sincerely
5239	1097	efficiently
5240	1097	bitterly
5242	1096	individually
5254	1093	angrily
5358	1055	incidentally
5366	1054	loudly
5385	1046	jointly
5389	1043	indirectly
5398	1041	allegedly
5477	1016	strangely
5508	1006	sexually
5517	1004	economically
5526	1002	unusually
5531	999	technically
5588	981	reluctantly
5599	979	vaguely
5605	977	ironically
5612	976	poorly
5615	975	duly
5624	972	smoothly
5645	968	presently
5657	964	principally
5691	955	nicely
5724	946	supposedly
5741	942	comfortably
5747	940	frankly
5796	924	curiously
5807	920	kindly
5810	919	unexpectedly
5831	914	promptly
5856	908	exceptionally
5904	891	extensively
5905	891	appropriately
5915	889	continuously
5941	882	fiercely
6007	866	fundamentally
6026	862	hastily
6033	861	nationally
6046	858	urgently
6056	856	financially
6073	852	lately
6198	823	enormously
6216	821	distinctly
6245	816	conversely
6312	801	incredibly
6313	801	historically
6315	800	wildly
```

autoscale: true <!-- -*- coding: utf-8 -*- -->
footer: Kenji Rikitake / oueees 201706 part 3 27-JUN-2017
slidenumbers: true
theme: Next, 1

![](blair-fraser-15137-slide.jpg)

# oueees-201706 Part 3: Negligence of people

<!-- Use Deckset 1.8,1, Next theme, 4:3 aspect ratio -->

---

# Kenji Rikitake

27-JUN-2017
School of Engineering Science
Osaka University
Toyonaka, Osaka, Japan
@jj1bdx

Copyright © 2017 Kenji Rikitake.
This work is licensed under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).

---

# Lecture notes on GitHub

* [https://github.com/jj1bdx/oueees-201706-public/](https://github.com/jj1bdx/oueees-201706-public/)
* Don't forget to *check out the issues*!

---

# Some thoughts on Part 2 report answers

* Internet and DNS: eventually consistent
* Concurrency = asynchronicity
* Eventual = allowing timeframe variance
* Redundancy: more availability

---

![original](trial-by-jury-slide.jpg)

# [fit] Negligence of people
# [fit] Risks of computer systems
# [fit] caused by human errors

---

![](hindenburg-slide.jpg)

# [fit] Illusion of *distributed* systems:
# [fit] how large systems fail

---

# Case study: Mizuho Bank on April 2002 (1/4) [^1]

* **Failed transactions** on merging 3 banks
* Duplicated transactions also observed
* **Planned since December 1999**, implementation details changed many times
* Single point of failure at the *Relay Computer*

[^1]: [失敗知識データベース: みずほファイナンシャルグループ大規模システム障害](http://www.sozogaku.com/fkd/cf/CA0000623.html)

---
[.hide-footer]
![original fit](mizuhobank-2002.png)

---

# Case study: Mizuho Bank on March 2011 (2/4) [^2]

* **~1.2M unprocessed transactions** on 17-MAR-2011; ATM closed for 3 days to complete the batch during 19~21 MAR-2011[^3]
* **Cascaded failures** by interrupted and duplicated batch operations


[^2]: [みずほ銀障害の全貌判明、懸案はCIO人事 - 第1回 重なった30の不手際 (ITpro)](http://itpro.nikkeibp.co.jp/article/COLUMN/20110607/361134/), [第2回 読み誤りや誤削除など人為ミス続発](http://itpro.nikkeibp.co.jp/article/COLUMN/20110607/361135/)

[^3]: [みずほ銀行: 2011年3月のシステムトラブル (Wikipedia) ](https://ja.wikipedia.org/wiki/みずほ銀行#2011.E5.B9.B43.E6.9C.88.E3.81.AE.E3.82.B7.E3.82.B9.E3.83.86.E3.83.A0.E3.83.88.E3.83.A9.E3.83.96.E3.83.AB)

---

# Case study: Mizuho Bank as of 2016 (3/4) [^4]

* Integration project initiated in 2012
* Scandal of relationship with organized crimininals revealed on September 2013[^5]
* Integration project deadline delayed from March 2016 to December 2016

[^4]: [Akio's Log - みずほ銀行次期システム関連のまとめ](http://elwoodblues.hatenablog.com/entry/20160706/1467806420)

[^5]: [みずほ銀行暴力団融資事件](https://ja.wikipedia.org/wiki/みずほ銀行暴力団融資事件)

---

# Case study: Mizuho Bank as of 2017 (4/4)

* Still recruiting software engineers (May 2017) [^6]
* Project completion by Summer 2017 announced; testing and implementation will take 1 to 1.5 years[^7]

[^6]: [ジョブダイレクト: みずほ情報総研株式会社の求人(2017年5月掲載)](http://www.jobdirect.jp/shigoto/c/j/0015795915)

[^7]: [みずほ銀行の次期システムが今夏にも完成との報道、稼働は18年度以降(ITpro 2017/05/08)](http://itpro.nikkeibp.co.jp/atcl/news/17/050801345/)

---

![](hieu-vu-minh-91994-slide.jpg)

# Why failed?

## [fit] No corporate governance
## [fit] No software engineering skills
## [fit] No project management skills
## [fit] Pervasive complacency
## [fit] Indifference and ignorance

---

# Question
## Can Mizuho Bank successfully complete the project this time?

---

![](exchange-of-ideas-slide.jpg)

# [fit] Fallacies of teamwork
# [fit] ... and other social issues

---

# [fit] Groupthink
# =
# [fit] 「空気読め」
---

# Groupthink (n.)

The practice of thinking or making decisions as a **group** in a way that **discourages creativity or individual responsibility** [^8]

[...]occurs when a group makes **faulty decisions because group pressures lead to a deterioration of "mental efficiency, reality testing, and moral judgment"** (Irving Janis, 1972)[^9]

[^8]: New Oxford American Dictionary, macOS 10.12.5, emphasis by Kenji Rikitake

[^9]: [The Psychologists for Social Responsibility, "What is Groupthink?"](http://www.psysr.org/about/pubs_resources/groupthink%20overview.htm)

---

> When all think alike, no one thinks very much.
-- Walter Lippman [^10]

[^10]: [Walter Lippman, "The Stakes of Diplomacy" (1915)](https://en.wikiquote.org/wiki/Walter_Lippmann)

---

# Groupthink symptoms (1/2) [^9]

* Illusion of invulnerability
* Collective rationalization
* Belief in inherent morality
* Stereotyped views of out-groups

---

# Groupthink symptoms (2/2) [^9]

* Direct pressure on dissenters
* Self-censorship
* Illusion of unanimity
* Self-appointed *mindguards*

---

# Groupthink in news media (1/2) [^9]

* Incomplete survey of alternatives
* Incomplete survey of objectives
* Failure to examine risks of preferred choice
* Failure to reappraise initially rejected alternatives

---

# Groupthink in news media (2/2) [^9]

* Poor information search
* Selective bias in processing information at hand
* Failure to work out contingency plans
* Low probability of successful outcome 

---

# Remedies of groupthink [^9]

* Assign critical evaluator role
* Stop stating preferences/expectations
* Check deliberation by external associates
* Invite outside experts to challenge
* Assign devil's advocate
* Survey rivals' scenarios regularly

---

# Filter Bubble: groupthink in internet [^11] [^12]

* **Filtering out the people and opinions against one's belief**
* **Less exposure to conflicting viewpoints**
* **Isolated in personal ecosystem enforcing ideological frames by the social network services and search engines**

[^11]: Pariser, Eli. The Filter Bubble: What the Internet Is Hiding from You, Penguin Press (New York, May 2011) ISBN 978-1-59420-300-8

[^12]: [Filter Bubble (Wikipedia)](https://en.wikipedia.org/wiki/Filter_bubble)

---

![original](ky-mug-slide.jpg)

# [fit] No groupthink
# [fit] 空気は読むな

---

![original](delacroix-liberte-slide.jpg)

# [fit] Centralized power
## .vs.
# [fit] individual freedom

---

![right fit](network-centralized.png)

# Centralized society

* **Efficient**
* **Power concentrated at the core**
* **Each node depends on the core**
* **System fails if the core fails**
* **Vulnerable to the attacks of the core**

---

![right fit](network-distributed.png)

# Distributed society

* **Inefficient = many hops are required to distribute information**
* **Power given to each node**
* **Each node should survive on its own**
* **Resilient to the attacks of each node**
* **Diversity**

---

# [fit] Distributed systems:
# [fit] Resilience
# [fit] Diversity
# [fit] Autonomy

---

# [fit] But the reality is:
# [fit] Efficiency
# [fit] Uniformity
# [fit] Autocracy

---

![original](matthew-henry-87142-slide.jpg)

# Question
## Are we trading our liberty and freedom for more efficient and convenient society?

---

# Appendix: on choosing your career and professionality

---

# When I chose my career and professionality?

* Age 9: discovered computers and English
* Age 10 discovered ham radio and electronics
* Age 14: earned money by writing software
* **Age 23: finally decided to make my living on my computer software professionality, with my English proficiency**

---

# [fit] If I were at age 22, what I would do
# [fit] after getting a Bachelor's degree?
## ...
# [fit] Get out of Japan ASAP
# [fit] Explore the computer skills
# [fit] Do something unpopular

---

# [fit] What are the most important things
# [fit] to pursue engineering/scientist career?
## ...
# [fit] Physical strength
# [fit] Mental strength
# [fit] Curiosity

---
[.autoscale: true]

Photo and figure credits:

* All photos are modified and edited by Kenji Rikitake

* Title: Blair Fraser, from Unsplash.com
* Negligence of people: [An engraving by D. H. Friston of Gilbert and Sullivan's Trial by Jury, shortly after its première, via Wikimedia Commons, in public domain](https://commons.wikimedia.org/wiki/File:Trial_by_Jury_-_Chaos_in_the_Courtroom.png)
* Illusion of distributed systems: [LZ 129 Hindenburg burning at US NAS Lakehurst, by Gus Pasquarella (US Navy), via Wikimedia Commons, in public domain](https://commons.wikimedia.org/wiki/File:Hindenburg_burning,_1937.jpg)
* Why failed?: Hieu Vu Minh, from Unsplash.com
* Fallacies of teamwork: [geralt from pixabay.com](https://pixabay.com/en/exchange-of-ideas-debate-discussion-222788/)
* No groupthink: [Douglas Paul Perkins, via Wikimedia Commons](https://commons.wikimedia.org/wiki/File:KY_Mug.jpg), licensed under [the Creative Commons CC0 1.0 Universal Public Domain Dedication](https://creativecommons.org/publicdomain/zero/1.0/deed.en)
* Centralized power .vs. individual freedom: [Eugène Delacroix, La liberté guidant le peuple, via Wikimedia Commons, in public domain](https://commons.wikimedia.org/wiki/File:Eugène_Delacroix_-_La_liberté_guidant_le_peuple.jpg)
* Trading our liberty for more efficient society: Matthew Henry, from unsplash.com

<!-- coding: utf-8 -->
<!-- End: -->

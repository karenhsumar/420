# TEST Did White teens lose interest in cannabis?

When [five students](https://en.wikipedia.org/wiki/420_(cannabis_culture)) at
San Rafael High School designated 4:20 p.m. as their regular time to get high,
they probably didn't anticipate the 4/20 meme to grow into an annual global
celebration. But the origin story does hint at the prevalence of marijuana use
in high school. Exactly how common is cannabis consumption for teens? Let's find out.

*Note: Source code and data for this article, including all visualizations, are in this [Github repo](https://github.com/capta-journal/420). You are welcome to fork the repo, edit it, and republish your version within [capta.studio](https://www.capta.studio/publish).*

The Youth Risk Behavior Surveillance System
[(YRBSS)](https://www.cdc.gov/healthyyouth/data/yrbs/index.htm) is a biannual
survey of high school students in the US, compiled by the Center for Disease
Control and Prevention (CDC). Its goal is to monitor risky behaviors that may
contribute to health and social problems, and [one of the behaviors](https://nccd.cdc.gov/youthonline/App/Results.aspx?TT=L&OUT=0&SID=HS&QID=H48&LID=XX&YID=YY&LID2=&YID2=&COL=S&ROW1=N&ROW2=N&HT=QQ&LCT=LL&FS=S1&FR=R1&FG=G1&FA=A1&FI=I1&FP=P1&FSL=S1&FRL=R1&FGL=G1&FAL=A1&FIL=I1&FPL=P1&PV=&TST=False&C1=&C2=&QP=G&DP=1&VA=CI&CS=Y&SYID=1991&EYID=2017&SC=DEFAULT&SO=ASC)
it has tracked since 1991 is whether a student is currently using
marijuana^[Current use is defined as using one or more times during the 30 days before the survey.].

```{vgl file=./cannabis_consumption.vgl.json}
```

Plotting the YRBSS results shows that in the last quarter century, there had
been two waves of marijuana use. The first wave took place in the '90s.
In 1991 marijuana usage was at a relatively low 14.7%. It shot up to 25.3%
in only four years, reaching an all-time peak of 26.7% by the end of the decade.
That is, for half the decade, fully one in four "high" school students were high.

The driver of the first wave was probably rap music. Cypress Hill's eponymous
album came out in 1991, heavily promoting recreational marijuana use.
Dr. Dre's debut solo album *The Chronic* was released in the following year,
in which the album name refers to a particular strain of marijuana. If you've
watched a rap video from that era, you've probably watched some rapper blazing
up. It just looks so cinematic...

![Dr. Dre puffing out smoke](https://media.giphy.com/media/QlzhlVkPmKqY0/giphy.gif =100%x)

The usage of cannabis declined during the aughts, and bottomed out in 2007.
Then a smaller wave arrived and peaked in 2013. As of 2017 (the last data point
we have), we're back at the 2007 level.

The top of the recent wave coincides with the beginning of the marijuana
legalization movement, and it's not clear if or how the two interact. A
[number](https://news.wsu.edu/2019/03/15/teens-report-using-marijuana-less-often-legalization/)
[of](https://www.rand.org/news/press/2018/12/21.html)
[studies](https://jamanetwork.com/journals/jamapediatrics/article-abstract/2718512)
have noted the decline of adolescent marijuana use in Washington after that
state's legalization. However, as we've seen, the decline shows up in the national
aggregate as well. A deeper study is needed to tease out various cause and effects.

```{vgl file=./cannabis_consumption_by_sex.vgl.json}
```

While the overall picture for cannabis consumption seems to have moderated from
the late '90s, a deeper dive into the data shows many nuances within the
general trend. For example, consider the
sexes^[[YRBS data](https://nccd.cdc.gov/Youthonline/App/Results.aspx?TT=L&OUT=1&SID=HS&QID=H48&LID=XX&YID=YY&LID2=&YID2=&COL=S&ROW1=N&ROW2=N&HT=QQ&LCT=LL&FS=S1&FR=R1&FG=G1&FA=A1&FI=I1&FP=P1&FSL=S1&FRL=R1&FGL=G1&FAL=A1&FIL=I1&FPL=P1&PV=&TST=False&C1=&C2=&QP=G&DP=1&VA=CI&CS=Y&SYID=&EYID=&SC=DEFAULT&SO=ASC)].
**Teen males have always been more likely to blaze up than females, but that gap has shrunk and completely closed by 2017.**
This is mostly driven by decreased usage by males. By 2017 teenage men were
consuming marijuana at their lowest rate (20.0%) since 1991.

```{vgl file=./cannabis_consumption_by_race.vgl.json}
```

Cannabis culture also diverges between different
ethnicities^[[YRBS data](https://nccd.cdc.gov/Youthonline/App/Results.aspx?TT=L&OUT=1&SID=HS&QID=H48&LID=XX&YID=YY&LID2=&YID2=&COL=R&ROW1=N&ROW2=N&HT=QQ&LCT=LL&FS=S1&FR=R1&FG=G1&FA=A1&FI=I1&FP=P1&FSL=S1&FRL=R1&FGL=G1&FAL=A1&FIL=I1&FPL=P1&PV=&TST=False&C1=&C2=&QP=G&DP=1&VA=CI&CS=Y&SYID=&EYID=&SC=DEFAULT&SO=ASC)].
Native Americans^[Labeled as AI/AN in the graph, meaning American Indians and Alaskan Natives]
are much more likely to use marijuana while Asian Americans
are much less likely. Whites, Hispanics, and African Americans have tracked
each other in usage most of the time, up till about ten years ago.

Except for Whites, the double hump pattern in marijuana usage are quite visible
in all ethnicities. Furthermore, while the aggregate figure shown earlier
suggests that the second wave of usage was below the peak of late '90s, that's
not true for ethnic minorities. In fact, at the peak of the second wave, more
Asian Americans and Native Americans were smoking than during the first wave.

**So what drove the seeming decrease in consumption in the aggregate? It's entirely due to White teens' lost of interest in cannabis.**
As they are the majority in the population, they alone could bring down the
overall trend. So what happened 10 years ago that led a resurgence of cannabis
consumption for ethnic minorities but not White teens? I don't have any
hypothesis. If you have any idea, join
[the discussion on Github or submit a pull request to update this article](https://github.com/capta-journal/420/issues/1).

###### About Capta
*Capta is a blogging platform for data journalism. The article you're reading is written entirely using Markdown, JSON, and data in CSV format. No Javascript, Python, R, or any other programming language is used. Publishes directly from Github, ensuring version control and reproducibility. All the code for this article are in this [Github repo](https://github.com/capta-journal/420). You are welcome to fork the repo, edit it, and republish your version within [Capta](https://www.capta.studio/publish). Or create a new repo and [publish](https://www.capta.studio/publish) your own article!*

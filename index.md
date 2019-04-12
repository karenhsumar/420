# How High?? - A Look at a Quarter Century of Teenage Cannabis Consumption

Marijuana has been gaining mainstream acceptance in the last few years. Since Washington and Colorado's legalization of recreational use in 2012, eight other states and the District of Columbia have passed similar laws. An additional 14 states have [decriminalized](https://en.wikipedia.org/wiki/Legality_of_cannabis_by_U.S._jurisdiction). In 2018 the [Marijuana Business Conference (MJBizCon)](https://mjbizconference.com/vegas/) attracted [27,600 attendees](https://daily.sevenfifty.com/cannabis-trends-we-should-all-be-watching-in-2019/), more than double its attendance in 2017. And of course, there's now [an app](https://wheresweed.com/) to help you find and rate your nearby dispensaries.

With the 4/20 holiday, however, we're reminded that cannabis culture has a long history outside the mainstream. The "420" term traces its [origin](https://en.wikipedia.org/wiki/420_(cannabis_culture)) to five students at San Rafael High School, who called themselves the Waldos and designated 4:20 p.m. as their meeting time to get high. One of the Waldos would later become a roadie for the Grateful Dead and helped spread the term to its followers and the rest of the counterculture.

As the Waldos would have suggested, cannabis consumption is pretty prevalent among high school students. But how common is it really? And does it vary much within various sub-populations? One dataset compiled by the Center for Disease Control and Prevention (CDC) would give us some insights into those questions. The [Youth Risk Behavior Surveillance System (YRBSS)](https://www.cdc.gov/healthyyouth/data/yrbs/index.htm) is a biannual survey of 9th through 12th grade students in public and private schools in the United States, to monitor risky behaviors that may contribute to health and social problems. [One of the behaviors YRBSS](https://nccd.cdc.gov/youthonline/App/Results.aspx?TT=L&OUT=0&SID=HS&QID=H48&LID=XX&YID=YY&LID2=&YID2=&COL=S&ROW1=N&ROW2=N&HT=QQ&LCT=LL&FS=S1&FR=R1&FG=G1&FA=A1&FI=I1&FP=P1&FSL=S1&FRL=R1&FGL=G1&FAL=A1&FIL=I1&FPL=P1&PV=&TST=False&C1=&C2=&QP=G&DP=1&VA=CI&CS=Y&SYID=1991&EYID=2017&SC=DEFAULT&SO=ASC) has tracked since 1991 is whether a student is currently using marijuana[^1].

(Put an aside here about the Github repo and how they can fork and reproduce this entire article.)

## General Trend over Time

```{vgl file=./cannabis_consumption.vgl.json}
```

Plotting the YRBSS results shows that in the last quarter century, there had been two waves of marijuana use among high-school students. The first wave took place in the '90s. Starting in 1991 marijuana usage was at a relatively low 14.7% and shot up to 25.3% in only four years, reaching an all-time peak of 26.7% by the end of the decade. That is, for half the decade, fully one in four "high" school students were high.

It's not hard to see the origin of this trend in popular culture, as rap music was entering the mainstream. Cypress Hill's eponymous album came out in 1991; their music heavily promoted recreational marijuana use. Dr. Dre's debut solo album *The Chronic* was released in the following year, in which the album name refers to a particularly potent strain of marijuana. These, together with other rap albums of that era, heavily cross promoted hip hop culture and weed smoking. If you've watched a rap video, you've probably watched some rapper blazing up. It just looks so cinematic...

![Dre smoking](https://media.giphy.com/media/QlzhlVkPmKqY0/giphy.gif =100%x)

The usage of cannabis declined during the aughts, and bottomed out in 2007. Then a smaller wave arrived and peaked in 2013. As of 2017 (the last data point we have), we're back at the 2007 level, which is the lowest since 1995.

The top of the recent wave coincides with the beginning of the legalization movement, and it's not clear if or how the two interact. A [number](https://news.wsu.edu/2019/03/15/teens-report-using-marijuana-less-often-legalization/) [of](https://www.rand.org/news/press/2018/12/21.html) [studies](https://jamanetwork.com/journals/jamapediatrics/article-abstract/2718512) have noted the decline of adolescent marijuana use in Washington after its legalization. However, as we've seen, the decline shows up in the national aggregate as well. A deeper state-by-state comparison is needed to tease out possible effects of legalization to teenage cannabis consumption.

## Trends among Various Sub-populations

```{vgl file=./cannabis_consumption_by_sex.vgl.json}
```

While the overall picture for cannabis consumption seemed to have moderated from the late '90s, a deeper dive into the data shows many nuances within the general trend. For example, there are interesting differences between [sexes](https://nccd.cdc.gov/Youthonline/App/Results.aspx?TT=L&OUT=1&SID=HS&QID=H48&LID=XX&YID=YY&LID2=&YID2=&COL=S&ROW1=N&ROW2=N&HT=QQ&LCT=LL&FS=S1&FR=R1&FG=G1&FA=A1&FI=I1&FP=P1&FSL=S1&FRL=R1&FGL=G1&FAL=A1&FIL=I1&FPL=P1&PV=&TST=False&C1=&C2=&QP=G&DP=1&VA=CI&CS=Y&SYID=&EYID=&SC=DEFAULT&SO=ASC). Teen males have always been more likely to blaze up than females, but that gap has steadily closed in the last 25 years. So that by 2017 both sexes are equally likely to use marijuana. That is, the drop in marijuana usage was much more of a male phenomenon. In fact, in 2017 teenage men consumed marijuana at the lowest rate (20.0%) since 1991.

Cannabis culture also diverges between different [ethnicities](https://nccd.cdc.gov/Youthonline/App/Results.aspx?TT=L&OUT=1&SID=HS&QID=H48&LID=XX&YID=YY&LID2=&YID2=&COL=R&ROW1=N&ROW2=N&HT=QQ&LCT=LL&FS=S1&FR=R1&FG=G1&FA=A1&FI=I1&FP=P1&FSL=S1&FRL=R1&FGL=G1&FAL=A1&FIL=I1&FPL=P1&PV=&TST=False&C1=&C2=&QP=G&DP=1&VA=CI&CS=Y&SYID=&EYID=&SC=DEFAULT&SO=ASC). Native Americans are much more likely to use marijuana while Asian Americans are much less likely. Whites, Hispanics, and African Americans have tracked each other in usage most of the time, up till about ten years ago.

```{vgl file=./cannabis_consumption_by_race.vgl.json}
```

Except for Whites, the double hump pattern in marijuana usage are quite visible in all other ethnicities. Furthermore, while the aggregate figure shown earlier suggests that the second wave of usage earlier this decade was below the peak of late '90s, that's not true for ethnic minorities. In fact, at the peak of the second wave, more Asian Americans and Native Americans were smoking than during the first wave.

So what drove the seeming decrease in consumption in the aggregate graph? It's entirely driven by White teens' lost of interest in cannabis. As they are the majority in the population, they alone could bring down the overall trend. In the graph above, I've plotted on the right side data for Whites only, to help clarify how small their second peak in 2011 was. So what happened 10 years ago that led a resurgence of cannabis consumption in ethnic minorities but not White teens? I don't have any hypothesis. If you have any idea, join [the discussion on Github or submit a pull request to update this article]().

[^1]: Current use is defined as using one or more times during the 30 days before the survey.

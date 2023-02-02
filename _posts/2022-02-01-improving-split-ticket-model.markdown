---
layout: post
title:  "Potential Improvements to Split Ticket's WAR model"
date:   2023-02-01 00:00:00
categories: modeling
---
## Potential Improvements to Split Ticket's candidate quality model

The current generic ballot result and shift from 2020 to 2022 is based on [another article](https://split-ticket.org/2022/12/14/the-true-swing-from-2020-to-2022/) which is pretty good, but has its limitations. 

![2020-2022 swing](https://i0.wp.com/split-ticket.org/wp-content/uploads/2022/12/swing-gcb-20-22-3.png?resize=2048%2C1536&ssl=1)

![2022 estimated generic ballot](https://i0.wp.com/split-ticket.org/wp-content/uploads/2022/12/2020-GCB-3.png?resize=2048%2C1536&ssl=1)

Now, onto the Wins Above Replacement model (specifically the [Senate WAR model](https://split-ticket.org/posts/2022-senate-war/))

![2022 senate WAR](https://i0.wp.com/split-ticket.org/wp-content/uploads/2023/01/16_9_senate_2022_war.png?resize=2048%2C1152&ssl=1)

I have some interesting observations. In particular, spending differential is overstated, in my opinion. Jo Rae Perkins and Joe Pinion were getting carried by the overperformances in their state's governor's race. The reason why Jo Rae Perkins and Joe Pinion were given a high WAR was due to their poor funding differential. [Pinion's opponent, Chuck Schumer, spent $41,742,016 while Pinion spent $545,984.](https://www.opensecrets.org/races/candidates?cycle=2022&id=NYS2&spec=N) In itself, somewhat matching the Republican vote share in the governor's race while being underfunded is superb, especially due to lower rates of ticket splitting in federal races, but this fails to account for the fact that the governor's race coattails were a major effect in these two races. 

I would also like to treat incumbency as a percentage instead of a binary 0 or 1 for a party. Incumbency has less of an boost for incumbents with new turf. This is difficult to determine exactly, but percentage of previously represented district is a somewhat okay heuristic. Since 2022 was a redistricting year, this is important ([sorry John Mark Windle](https://twitter.com/LucasTBrooks/status/1608869713043677184)). Thus we could settle the question of whether Kurt Schrader, a moderate Democrat who lost in the primary after taking in new liberal areas of Bend, would have lost in OR-5.

Finally, a WAR for Lisa Murkowski is not included, due to Alaskan strangeness. I would like to treat her as a Democrat and see what happens. Her coalition mirrors Peltola's: she relies on Democrats, Independents, and Alaskan Bush voters (who have been trending rightwards as of late) and a dwindling number of conservative-leaning voters.

Hope to see you soon.
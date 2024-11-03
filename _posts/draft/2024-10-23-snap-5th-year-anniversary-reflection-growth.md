<!-- ---
title: 'Growth = Step-Function Changes + Incremental Improvements'
date: 2024-10-23
permalink: /posts/2024/10/snap_year5_growth/
tags:
  # - growth
--- -->

October 2024 marks my fifth year at Snap, making this my second-longest tenure with an organization, aside from my graduate program. While there are still many challenges to tackle at work, I want to take a moment to reflect on the journey that brought me here and to share some of the insights and lessons I've gathered along the way—many of which were learned the hard way.

__Why Snap?__ 

Rewind to 2019: I was looking for a role in a domain or product that was close to end customers, business-critical, and technically challenging enough to keep me busy and dedicated for at least 3-4 years. When the opportunity arose to build the Friend Recommendation system on Snapchat, I knew it checked every box I’d hoped for. So, I joined Snap to help build Friend Recommendation, a product now used by hundreds of millions of users daily.

__Quick Add__ 

The Friend Recommendation product on Snapchat is known as [Quick Add](https://help.snapchat.com/hc/en-us/articles/7012328615828-How-to-Add-Friends-on-Snapchat#:~:text=Quick%20Add%20may%20appear%20in,different%20depending%20on%20your%20device.). In the industry, friend recommendation systems are commonly referred to as 'PYMK' (People You May Know). This term was initially introduced by LinkedIn (I had thought Facebook coined it first) and was later popularized by Facebook as one of its most crucial [growth products](https://www.youtube.com/watch?v=kl5ijJW50JU). 

Friend recommendation is an intriguing and complex problem with unique challenges. The first challenge is scalability: we’re recommending friends to billions of users from within the same billions of users, which is essentially an N<sup>2</sup> problem. Secondly, because we recommend users to other users in the same social graph, strong network effects make A/B testing and evaluation difficult. Finally, like many other networks, there's a [Matthew effect]((https://en.wikipedia.org/wiki/Matthew_effect)), where 'the rich get richer,' which could hinder growth if not managed carefully. In addressing these challenges and many others, I have repeatedly observed the following pattern. 

__Growth = Step-Function Changes + Incremental Improvements__

Looking closely at the success metrics of Friend Recommendation over the years (adjusted for seasonality), a clear pattern emerges in the chart: a few major surges followed by steady, gradual increases. In other words, growth is driven by two forces — numerous small, incremental changes and a few significant, step-function changes. Both are essential and irreplaceable.

__Step-Function Changes__

First, let's discuss the significant step-function changes and why they are crucial for growth. Like the roles The Development of Language, The Agricultural Revolution, and The Industrial Revolution played in the human history, I found similar events in building Friending products. I have personally experienced each of these changes and can readily associate the surge in the chart with specific feature launches. For example, the online feature store enabled feature engineering of ML models for Snap scale, [embedding based retrieval](https://zariable.github.io/publication/sigir_2023) that introduced a new way to retrieve candidates and motivates the continuous improvement of user embedding, and notable UX and UI changes in reducing friction of Friending experience. These moments are truly exciting and the work laid the foundations and unlocked opportunities that were once considered unattainable. 

While these step function events can change the growth trajectory of a product, we do not see them often. One possibility is these step foundation changes are signficantly less likly to occur as the product matures. In this case, the next step function change only happen when there are new technology innovations or new product ideas. But far more often it is because the team didn't make bold bets that eventually led to those step function changes. There can be many different reasons why the investments have not been made. 

While big changes do occur, they are inherently rare, less likely to happen as the product matures, and most importantly in sufficient to driving growth by themselves alone. Now, let’s turn our attention to the small, incremental changes.

__Incremental Improvements__

The human brain tends to latch onto a few significant events. In Morgan Housel's book 'Same as Ever', he wrote that many people remember that Dwight Eisenhower survived a heart attack in 1955, while far fewer notice the remarkable 70% reduction in the death rate from heart disease since then thanks to advances in detection and treatment because that is 1.5% each year on average, too small of a number to notice by most.

Similarly, in the domain of growth, people tend to celebrate and remember the big wins, while the incremental changes often go unnoticed and are frequently overlooked. Here is an interesting story I experience firsthand. When we launched the first version of user embedding using [Graph Neural Networks](https://zariable.github.io/publication/sigir_2023), we celebrated the achievement with an email to executives and a party. Since that initial launch, we’ve successfully iterated on the embedding quality more than ten times (not counting the unsuccessful attempts). To my surprise, when I later combine the compound metric gains from these later iterations, they far surpass the gains from the initial launch. The compound effect works its magic. My takeaway is we should not rely solely on big and step-fnctional changes in driving growth while overlooking the seemingly small but incremental ones; when enough incremental improvements accumulate, their combined impact can be astonishing.

__An Analogy from Machine Learning__

I see a parallel between this pattern of incremental changes and step-function changes in machine learning—specifically, gradient descent. In gradient descent, the goal is to find the global optimum of a function. Incremental improvements can be viewed as performing local optimizations; they are essential because they help us identify the best solution within the constraints of existing technology. However, if the team exhausts all opportunities offered by the current technology without introducing new innovations, productivity can stall. This underscores the importance of investing in technologies that can help us break free from local optima and facilitate step-function changes. These significant changes elevate the business to new heights and create numerous low-hanging fruits, which can then be realized through further incremental improvements. Additionally, this approach provides engineers with opportunities to learn new technologies and make a meaningful impact.


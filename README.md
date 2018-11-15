# Designing-with-data
What I have done so far to get google analytics to tell me how users behave within my service.

The starting point needs to be a measurement plan, what do you need to report on to measure how the service is performing? 
You also need to know how to capture the data required. 
I have been doing both of these hand in hand.

**Google Analytics (GA)**

Initially I asked Alistair to create a property in Google Analytics for my service.
Then asked the front end dev to add page view recording to all pages on the service.
This is very simple but provides a lot data that is interesting in Google Analytics.
For example about 50% of page views are from IE 8.

**Google Tag Manager (GTM)**

I wanted to know certain things, for example:
How many PERs are sent from each prison and where they are sent to? 
Which courts use the receiver view?
How many PERs are issued each week?
How long does it take to answer all the questions in the risk section?

But these things couldn’t be accessed via page views. More front end code would be needed.
Then I read about Google Tag Manager (GTM). To get GTM wired up to the service I got the dev to  replace the GA code with the GTM code, which is simple. With this in place GTM enables you to write your own tags, triggers and variables and sends data to GA all without altering page code. So no need for a dev. no delay in deployment or waiting for tickets to be prioritised. You can do it yourself. You can also test on staging before publishing the tags. Once published GA reports will start showing the results.

We can now see where PERs are sent from and to and how many. Which courts access the service. How many PERs are issued each week. How many PERs are cancelled and the reason for cancellation. And various other interesting data points. I have yet to work out how to record how long it takes to complete the risk section but I am working on it.

**Data Studio**

GA reports takes time to dig around to find what you are after. To provide easy to digest reports you can use Data Studio, which enables you to create a dashboard of data, populated from your GA data, that you can share with anyone.
Here is a work in progress data studio dashboard for Moving People Safely:
https://datastudio.google.com/open/1v6nTAeEEehBcSBnC6_PClJlJtHzoIdUM

**Show The Thing**
I did a show the thing...to try and whip up interest and find others
https://www.youtube.com/watch?v=CDynjC-uDvc

**Issues**

In IE 8 the tags fail. So the data from events is not recorded. However, pageviews still work. 

**Links to resources**

These are the starting points of the resources I used.

Analytics Academy
https://analytics.google.com/analytics/academy/

Google Tag Manager
https://marketingplatform.google.com/about/tag-manager/?utm_campaign=product-cross-sell&utm_source=analytics-discover-page&utm_medium=referral-internal&utm_content=tag-manager-card

Google Tag Assistant
https://get.google.com/tagassistant/?utm_source=analytics-discover-page&utm_medium=referral-internal&utm-campaign=content-cross-promo&utm_content=ga-tag-assistant-card

Data Studio
https://marketingplatform.google.com/about/data-studio/?utm_campaign=product-cross-sell&utm_source=analytics-discover-page&utm_medium=referral-internal&utm_content=data-studio-card

Lynda.com

YouTube
Measureschool - I have found to be good.

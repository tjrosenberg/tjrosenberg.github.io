---
layout: post
title:  "Why should you care about standard deviation?"
date:   2021-04-24 00:48:52 -0700
categories: jekyll update
---

Before we can answer the question in the title we have to back up and talk about *averages*. And don't worry if you are uncomfortable with math, I am going to do my best to present it in a way that is understandable whether you have a background in math or not.

## What is an average?

Average is a word that gets used a lot in day to day life so you probably already have a intuition about what it means. You might even say: "this is a very *average* blog post". Meaning this blog post is *comparable* to other blog posts. Or maybe you mean that this blog post is approximately *medium* on the "goodness" scale - it hits the standards to be a decent blog post but its not blowing anyone's socks off. For the record, if this blog post lives up to being average I will be thrilled because this is my first! There is one important element here that is easily overlooked; in order for you to make the aforementioned statement you have to know something about other blog posts. This gives us our first working definition of average: when you say "this is a very *average* blog post" you are saying it is *similar* to a lot of (if not most) other blog posts out there. We can also flip this idea around and use an *average* blog post as a *representative* of other blog posts. In general it is quite useful to study an average thing to gain a better understanding of all of those things. A common way this is phrased is that the average is a *measure of center* of a given set of things. 

Okay, its time to get a little more concrete. Lets move on from the example of blog posts and think about groceries instead. Imagine you like to cook and every Sunday you buy groceries to make your meals for the week. However, week to week the number of meals you cook for yourself varies. Maybe one week you end up going out to dinner with old friends and then the next day a coworker brings lunch for everyone at work. Now you have two meals you planned on cooking but never got made. Or perhaps the opposite happens and some dinner plans you had fell through so you run out of food to make your last few meals. One way to try to solve this problem is by recording how many meals you cook and actually eat over many weeks and taking the average of those numbers. This is the first time in this article we are actually taking a numerical average. But don't panic this is something that *anyone* can do. The easiest way to take an average is to search the internet for an average calculator and just plug in your numbers - seriously its super easy. If you are into doing things yourself you can sum all the values of your meals per week then divide by the number of values you have. Or if you really like digging into the math you can sum the products of each value with the probability of that value occurring. But the main takeaway is that each of these methods will give you the same average, known as the mean, of your data. Once you know the average number of meals you cook and eat per week, lets say it was 10, every Sunday when you go grocery shopping you 10 meals worth of groceries. 

Using your new found understanding of averages you never have too many or too few meals again right?

Not quite...

The average doesn't tell the whole story. To complete the picture we have to talk about the ***standard deviation***.

## What is the standard deviation?

The standard deviation is another value or property of a dataset, the same way an average is a property of a dataset. However the biggest difference is where the *average* is a *measure of center* the *standard deviation* is a *measure of spread*. Said differently, the standard deviation tells you how close to the average some item in the set is. 

Lets compare two cases of our grocery example from above:

#### 1. The traveling sales person

Imagine you are a sales person for some company that sends on work trips quite often, usually for 4 or 5 days at a time. When you aren't traveling you work in a regular office near where you live. You don't always know when you will be sent on a work trip - sometimes you come in Monday morning and find out you will be leaving Tuesday and won't be back until Friday afternoon. Since you have no idea whether you will be in town or away you still buy your groceries on Sunday. Just as before you record how many meals you cook and eat over the course of 3 months (12 weeks) and you find the following set: [16,15,2,3,4,18,6,13,14,7,17,5]. 

Next, you compute the average of your data and find:

Average number of meals = (16+15+2+3+4+18+6+13+14+7+17+5)/12 = 10, just as in the example above. 

#### 2. The consistent insurance agent

Imagine this time you are an insurance agent who love a consistent schedule. You work in the same office everyday, where your job provides you lunch, on Fridays you go out to dinner with your coworkers and on Sundays you meet your mom for brunch. You also decide to record your number of meals cooked and eaten over the course of 3 months and find the following set: [9,11,10,8,11,10,9,11,10,12,9,10]

Next, you compute the average of your data and find:

Average number of meals = (9+11+10+8+11+10+9+11+10+12+9+10)/12 = 10, just like the traveling sales person.

#### What's the difference?

From the description of these two different careers it is probably clear to you that they have a very different lifestyles however, they found the same average number of meals cooked and eaten per week. Further, when each of these cases tries the strategy of buying enough groceries to cook 10 meals the traveling sales person finds they are still over/underbuying quite frequently whereas the consistent insurance agent finds they almost always have the exact right number of meals. To understand why this is it is helpful to visualize the two datasets listed above in the form of a *histogram*. If you are unfamiliar, a histogram is just a chart that shows how frequently each possible value shows up in a data set. 



 <img src="standard dev.png" style="zoom:50%;" />



On the left we have the histogram for the traveling sales person and on the right we have that of the consistent insurance agent. Further, the average for each, 10, is shown as well. What is the biggest difference between these? The bulk of the traveling sales persons data sits further away from the average than the bulk of the consistent insurance agents data. We could quantify this in many different ways but the most common way is to use the *standard deviation*. Calculating the standard deviation is not quite as simple as calculating the average, in fact it relies on the average. In words, the standard deviation is the square root of the sum over the values of the square of the difference between the value and the average divided by the number of values (find it in equation form [here](https://en.wikipedia.org/wiki/Standard_deviation)). If that sounds too complicated there are lots of calculators that will do it for you. In general, the standard deviation is given in the same units as your data and can be interpreted as follows. 

A large standard deviation means that a lot of the data is far from the average and a small standard deviation means a lot of the data is close to the average. 

To illustrate this we turn back to the case of the traveling sales person and the consistent insurance agent. The standard deviation of the sales persons data is 5.75 whereas the standard deviation of the insurance agents data is 1.08 which is much smaller. This means that the number of meals per week eaten by the sales person is most likely to fall *almost 6 meals away from the average*. On the other hand the number of meals eaten on a given week by the insurance agent is most likely to fall *about 1 meal away from the average*. The standard deviation has given us insight into why this strategy works well for the insurance agent but poorly for the sales person. 

Now we are ready to answer the question in the title of this article.

## Why should you care about standard deviation?

To put it simply you should care about the standard deviation of a dataset because it tells you exactly how good of a *representative* the average is for the whole. My favorite example of this is the search for the average Australian. 

In 2011 the Australian census data was used to determine the average Australian person. They found the average Australian was age 37, height 5'4", with a son and a daughter, aged six and nine, living in a three-bedroom, free-standing house. Next, they set out to find a living breathing average Australian citizen but to their surprise not a single person actually matched all of those statistics. This is an illustration of the fact that humans are quite diverse and thus data taken about human characteristics often has a large standard deviation. This means that the average human is not a good representative of all humans. Taking this one step further, making statements about the average human will not generalize well to the entire population.

A place I see this mistake made quite often is in the news media. Too often an average is presented without any mention of the standard deviation then conclusions are drawn about the population based on this average all without ever knowing if that average is a good representative of the population or not.

So whenever you see an average, you should ask the question "what is the standard deviation?" *because no statistical description is complete without both a measure of center and a measure of spread.* 



#### Final notes

It is worth mentioning that here I focused used the mean as my measure of center and the standard deviation as the measure of spread. However, in general there are many other measures of center and spread that can be used in various circumstances. 

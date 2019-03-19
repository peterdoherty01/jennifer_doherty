+++ 
date = "2019-02-24"
title = "Building a Static Website with Gatsbyjs"
slug = "build-webpage-gatsbyjs"
tags = ["gatsby","js","experience","framework","technical","guide","startup","bootstrap"]
categories = ["web"]
+++

#### Online Portfolio

My wife needed a portfolio to gather all her media (writings, articles, resume etc) in one place. This hopefully would boost her chances of getting hired as a reporter. 

One solution was to set up a site in Squarespace or a similar vendor and let her design and deploy it. I decided against this due to 1) the $12 per month fee when it could be hosted for free with a custom solution and 2) she might experience technical difficulties and I would have to jump onboard to help. Thus, absorbing too much of both of our time.

As another option, I had played with the idea of building the site in Django and hosting it on Heroku for free. Just prior to this project, I had just rebuilt the [Computation Hub website](www.computationhub.com) in Django, Heroku, AWS S3 and PostgresQL. The issue I foresaw was that hosting a webpage on Heroku, built with Django is painful and tedious to execute - most importantly it could absorb a lot of my time troubleshooting production issues. 

#### Compiling Blog Posts

Moreover, I like the idea of writing posts in [markdown format](https://en.wikipedia.org/wiki/Markdown) as it's seen as a best practice in the web development community. In Django, the posts are "hidden" away in the database. Basically, I or my wife wouldn't be able to write a post in markdown and quickly and easily deploy to the webpage. 

Sidenote: there might be a toolchain out there to do this with a Django backend setup, but I am not aware of it. Again, I didn't want to spend a bunch of hours reading the documentation to see how it would work.

#### Blog

I had been hearing on Twitter about Gatsby and Hugo. In parallel, I had also been hearing a lot of chatter about [Netlify](www.netlify.com) to deploy websites. The word "blazing" appeared alot in tweets by many developers online. Luckily enough I found a post on how to build a [Gatsby](https://www.gatsbyjs.org/starters/?v=2) blog in less than 30mins (that's not the exact title but you get the idea). This was quite inspiring and compelling so I chose Gatsby and fired up a starter template with Netlify.

#### Get started with Gatsby + Netlify

Here's how I did it. **Note:**

1. The steps outlined are good as of January 2019. They may change in the future
2. A Github, Gitlab is required
3. I used Gatsby V2
4. You can configure an existing domain that you bought previously with Netlify. It is a matter of copying and pasting the DNS server names that Netlify provide you with and pasting to your host provider (e.g. GoDaddy, Digital Ocean). Drop me a message if you need help doing that

##### Gatsby Starter

###### Phase 1

1. Go to the [Gatsby Starter page](https://www.gatsbyjs.org/starters/?v=2)
2. Choose a starter. In this case, I chose the [Gatsby Starter Blog](https://www.gatsbyjs.org/starters/gatsbyjs/gatsby-starter-blog/)
3. Scroll down the page to find "Try this starter with Netlify"
4. Click "Netlify"
5. Connect you code repository (repo) host. I chose Github
6. Choose a name for your repo (optional)
7. Click "Save & Deploy" (See Figure 1 below)
8. Keep an eye on the "Site deploy in progress" text, highlighted in orange
9. In the next screen, you'll see a dashboard with three steps. You might need to hit the browser refresh button to update the status
10. The site is deployed when you see some green text and your unique server name e.g. [https://focused-edison-45c24c.netlify.com](https://focused-edison-45c24c.netlify.com)

<center>
![](/posts/post_pics/gatsby_1.jpg)
_**Figure 1** Connect your code hosting repository_
</center>

<center>
![](/posts/post_pics/gatsby_2.jpg)
_**Figure 2** Choose a name and save & deploy_
</center>

###### Phase 2

1. Now, we will set up a domain name. I chose [www.jenniferdoherty.net](www.jenniferdoherty.net) which I had bought from GoDaddy previously
2. It might take a few minutes to connect the domain to your account
3. Optional: if you have a domain already like I did, you can point your DNS servers in GoDaddy to the ones provided by Gatsby

###### Phase 3

1. Let's encrypt is then automatically setup within a few minutes.
2. Follow any other instructions that might appear

#### Conclusion

Gatsbyjs is a nice and fast way to get started with a site, domain and Secure Socket Layer security. It takes around 10 mins without to deploy a simple starter blog, similar to the one I used. 

I discovered that this sort of website configuration is called JAMstack

> Modern web development architecture based on client-side JavaScript, reusable APIs, and prebuilt Markup.
>
<cite>[https://jamstack.org/](https://jamstack.org/)</cite>

Some benefits provided are:

* Better Performance
* Secure
* Cheaper
* Better Developer Experience

I found the startup up very fast, and it emits that rapid feel way too. Another positive - there's no database which, can get hacked in a more complex setup. I used a Gatsby starter and free Netlify account; this saved me $144 per year. The experience was quite pleasant with the starter I chose; the localhost reboots instantly when you update your config file or content.

Regarding Netlify, I found this to be extremely fast, reliable and easy to navigate. I also discovered elsewhere that they have the provide the ability to [manually "drag & drop" a site](https://app.netlify.com/drop) into their service. This is convenient for beginners and if you don't have a code repository on Github or another vendor.

<center>
<iframe width="560" height="315" src="https://www.youtube.com/embed/-LRlQ_jaLAU" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</center>

#### Words of Caution

I had some difficulties with other Gatsby starter templates.

Several templates had difficulty deploying to the Netlify server, mainly due to a sharp plugin or library (I think). Other issues, would be related to plugins working in Gatsby V1 and not V2 (which I was using).

After searching Github for issues similar to mine with the hope someone else solved them, I noticed that some issues were closed by the moderators without reason and without a definitive solution. I found this a bit sketchy.

Other users had noticed this and voiced their frustrations. In my opinion, even though there appears to be some policing of the issues by the moderators, burying Github issues is not a good practice for an open source project. I appreciate that it is an open source project and they are providing a good tool overall. But, this housekeeping gives the impression there are less issues than there actually are. As a result, beginners/newbies might be attracted to using it.

This encouraged me to look for another alternative to Gatsbyjs. I checked out [Hugo.io](www.hugo.io) because I saw some recommendations for it issues logs. I noticed very quickly that the moderation on the Github repo was more stringent. For example, contributors who posted themes/starter templates were prompted to update libraries and dependencies when user encountered install or deploy issues. This had me sold.

Stay tuned for a post on how I built this static site with Hugo 

**Have you tried setting up your own site? Let me know in the comments or drop me a message**
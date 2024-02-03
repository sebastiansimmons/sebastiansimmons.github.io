---
title: 'Making my website MVP'
description: 'How I made a lightweight personal website and deployed it.'
pubDate: '2024-02-02'
heroImage: '/blog-placeholder-3.jpg'
draft: False
---

## My Old Website

In early 2020, I decided to finally make use of owning sebastiansimmons.com. With all the free time 2020 gave me, I threw myself into the project to learn as much as possible. I went through some JavaScript, React, and CSS tutorials to get a handle on what I thought would be needed to make something cool. I used [Next.js](https://nextjs.org/) as the final framework because I could easily deploy it through Netlify. I confirmed my suspicion that web development isn't
my favorite form of programming. However, I gained an appreciation for the hard work and expertise required to keep the front end of the internet looking pretty.

## The New Website

Four years later, I got the itch to start another side project and getting my personal website back online seemed like the perfect project.
[Astro](https://astro.build/) caught my eye as an exciting framework that didn't require as much JavaScipt to get a website up and running.
I ran through the introduction tutorial and played around with a few different out of the box themes.

## Getting the Bones

I went simple and used the built-in [Astro blog template](https://github.com/withastro/astro/tree/latest/examples/blog).
Replace all the boiler plate and default content, then you've got a website!

## Deploying to Production

I decided to deploy through GitHub Pages since I could easily automate the build with the Astro Deploy to Pages action.
[Netlifly's free tier](https://www.netlify.com/github-pages-vs-netlify/) was also a consideration, but for the time being, I don't need any of those features.

### Custom Domain

GitHub Pages has easy to follow [documentation](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/about-custom-domains-and-github-pages) for setting a custom domain and updating your DNS records.

## It's Done

I wanted to get a minimum viable personal website up and running before doing any customization. I started this project 4-5 different times and spent 
significantly more time on each of those attempts without shipping anything.

Now it's out! Time to customize it and make it my own!


## The First Real Modifications

Like I've said, web dev isn't really my thing. Despite acknowledging that it is probably the single most useful language to know outside of Python,
I still find JavaScript more confusing than when I was taking a systems class and learning MIPS assembly or C++ networking.

Still, I didn't feel right shipping the website until I had done a little more than replace template boilerplate.

### Draft Blog Posts

The first thing I added was a `draft` field in my markdown blog posts. The "Blog" page hides all pages with `draft == true`. Simple and useful!

### Future Date Publishing

The next feature I wanted to add was publishing pages based on the `pubDate` field. Basically, if `pubDate` is in the future, hide that post until it's the present.

Both of these changes were simple frontmatter fields and `filter` calls, but that's enough for me to feel like I technically customized the website to fit my needs.

## It's Live!

Yay! I made SebastianSimmons.com 2.0. I actually have no idea what I'm going to do on it. But if I want to do anything, I have a place to put it.

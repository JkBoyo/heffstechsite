+++
title = "Learning_hugo"
date = "2024-12-28T22:41:28-05:00"
#dateFormat = "2006-01-02" # This value can be configured for per-post date formatting
author = ""
authorTwitter = "" #do not include @
cover = ""
tags = ["", ""]
keywords = ["", ""]
description = ""
showFullContent = false
readingTime = false
hideComments = false
+++

What is Hugo?

I am glad you asked! Hugo is a *Static Site Generator* (*SSG*) built in the [golang](https://go.dev/) programming language.

Unless you happen to be into webdevelopment or are one of the lucky people I have rambled about this to, the next logical question is what is an **SSG**? 

If you don't happen to fall into either of those categories at its most basic an SSG is a program that converts MarkDown text which is essentially super simple text formatting into HTML which is the building block that webpages are built on. Open your browser and hit F12 and you will see countless HTML elements nested inside of countless divs. As you can guess writing all of the start tags and end tags repeatedly gets old. Hence the use of SSG's.

At it's most complex (like Hugo) an SSG can include premade themes that come with javascript (the language used to make the web interactive) baked in to provide the use of dropdown menu's interactive animations and everything that we associate with a modern website today!

I learned about this concept while studying backend dev at [boot.dev](https://boot.dev) by going in and building my own [super basic version (not for production use)](https://github.com/jkboyo/SSG) of an SSG.

{{< figure class="left" src="md.png" alt="MD test preconversion" position="center" style="border-radius: 8px;" caption="MD test preconversion" captionPosition="center" captionStyle="color: darkblue; border-radius: 8px;" >}}

{{< figure class="left" src="html.png" alt="Rendered HTML" position="center" style="border-radius: 8px;" caption="Rendered HTML" captionPosition="center" captionStyle="color: darkblue; border-radius: 8px;" >}}

Once I had completed this project I became interested in using a fully featured SSG. Thanks to one of the great go-vangelists of our time [@wagslane](https://x.com/wagslane?mx=2) being the author of the course, Hugo was frequently mentioned as what you should use.

With this knowledge in hand I started trying to figure out how to make a site with Hugo templates.

## The Curve

This process wasn't/isn't the easiest. Since my initial impetus was to try to get a basic website up for a business purpose I picked a template that looked nice but ***wasn't*** easy to learn Hugo with. The warning signs were there on the page telling me that Maintainability was a question mark.

I had mistakenly picked one of the themes that hasn't been kept up with and thus has numerouse problems with implementation and functionality. This made it a horrible place to start. After wasting most of an afternoon on gimp creating a logo that most likely wouldn't even be used and some time struggling to figure out how this particular theme worked I decided I was going to put that project aside for now and work on making a blog with the very terminal theme you are reading this on now!

Once I had moved to the Terminal theme things started to make more sense. The communication around what was needed to even create a new content type heck even what a content type was were much easier to find in this well loved theme! There was even a recently made [Network Chuck](https://www.youtube.com/@NetworkChuck) video about how he setup a blog using this very theme which helped me figure out the implementation of it.

I did have slight confusion about how to create the main page but then I figured out I simply had to create a post and the theme had a contructor that would make the page for me as a list of all of the articles I had already created!

Essentially the way themes are created are instrumental to how the overall site will work. In Terminals case the theme is centered around blog style content. It's only true content type are `posts` which you can create by issuing the `hugo new post` command and start to write MD. It is important to go through and configure your settings in your hugo.toml file but if the theme you are choosing from is sufficiently well documented it should be easy to figure out and configure. From there I was free to just write MD and include whatever headers or pictures or any other text I would like and run the `hugo server` command. This takes it and builds it into HTML with everything it should need to present the webpage and everything hosted from your machine to make sure it's working!

Once I had this part up and running it then took a little bit for me to get the basic version hosted. I opted to go with a cloudflare page pulling from my github as that's where I host my domain and that took a little while but the [docs](https://developers.cloudflare.com/pages/framework-guides/deploy-a-hugo-site/) made it fairly easy to do once i had figured out the problems i had setting up my system.

## End Goals/Thoughts

This post is much more of a retrospective and super high level summary of what I ended up learning from this process. Partially bc I still have yet to dive into this topic as deeply as I would like to.

However, my increased experience with this has given me the confidence and even the desire to potentially setup my own themes and sites using this tool and system!

Plus it has given me this place to talk about and practice writing and also track my to-do/in-process projects as well as give me some accountability so I can have people I share this with ask me about and pester me to do more with these projects instead of doom scrolling my life away.

If you want to see what I am working on/help keep me accountable in this as I'm only really sharing it with friends and family for now feel free to take a look at my [Projects Page](/projects) to see what I'm currently attempting to work on or hoping to do in the future!

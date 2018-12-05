## inFullAPI

<small>
November 2018 Hackathon
</small>

iFM Promotional Stunt

---

But first, since we are on the topic of promotion...

---

This is how we see ourselves on GitHub:

![](gh-sum-l-a.png)

<small>
https://github.com/inFullMobile (logged in as inFullMobile member)
</small>

---

This is how other people see us on GitHub:

![](gh-sum-i-a.png)

<small>
https://github.com/inFullMobile (see in incognito mode)
</small>

---

Who are those brave 4 who don't<br>hide that they belong
to inFullMobile?

---

![](gh-b4.png)

<small>
https://github.com/orgs/inFullMobile/people (see in incognito mode)
</small>

---

It's even worse on Stack Overflow.

Only 3 people have ever admitted<br>working at inFullMobile.

---

![](so-ifm-c.png)

<small>
https://stackoverflow.com/users/story/lists/160162/infullmobile?storyType=1
</small>

---

Recently we were discussing the topic of company
promotion on GitHub and Stack Overflow.

<small>
(Not hiding the fact that we work here would be a good start.)
</small>

---

We should take an example from the design team:

- https://dribbble.com/infullmobile
- https://www.behance.net/inFullMobile

---

Now back to the hackathon.

---

Hackathon theme: iFM Promotional Stunt

A good promotional stunt would be to:

1. Have a *fast* website and blog about its speed
2. Use *modern* technologies and blog about it
3. Make new designs frequently and let people vote
4. Make a periodical contest for a better website

---

Problem #1:

infullmobile.com website is sloooooow.

(*Especially* when accessed from the US.
Wouldn't be a problem if we didn't look for clients there,
but we do.)

---

Problem #2:

It's hard to optimize because we're using ready-made software
not targetted for developers.

---

Problem #3:

To try new designs we can only create WordPress themes.

In PHP.

---

Problem #4:

It's hard to use any modern frontend technology
like Vue, Aurelia Stencil or Svelte.

---

Problem #5:

Using any backend technology other than PHP is out of the question.

---

Problem #6:

It's hard to tell people that we use modern technology
when our own website is powered by PHP ("Personal Home Page")
that is not particularly well known for high quality

https://blog.codinghorror.com/the-php-singularity/

---

Some numbers

---

**5+ seconds** (not milliseconds!)<br>load time on WebPageTest

- First Byte Time: F grade
- Cache static content: F grade
- Effective use of CDN: No

<small>https://www.webpagetest.org/result/181121_86_dad9bcf684a911aee2353d6d98c463a1/</small>

---

**3/100**<br>score on testmysite.io

- Slow TTFB (Time To First Byte)
- Slow loading HTML
- HTTP2 not enabled

<small>https://testmysite.io/5bf530f7e39e7c78ae0e09e4/infullmobile.com</small>

---

![](testmysite.png)

<small>https://testmysite.io/5bf530f7e39e7c78ae0e09e4/infullmobile.com</small>

---

![](webpagetest1.png)

<small>https://www.webpagetest.org/result/181121_WZ_b79026bbf061ef6b5b648bb8083e9dde/</small>

---

HTML load time (no images and no rendering)

![](stats-ifm.png)

<small>(stats for the production website of inFullMobile)</small>

<small>https://testmysite.io/5bf530f7e39e7c78ae0e09e4/infullmobile.com</small>

---

It should be:

![](stats-bv.png)

<small>(stats for the development website of BookVenyou)</small>

<small>https://testmysite.io/5bf537a4b3127472b90dbbb2/bv-web-develop.netlify.com</small>

---

What can we do:

- Use modern technologies
- Expose all data with an API
- Build a Static/JAMstack website
- Use good hosting with CDN

---

What is **JAM**stack

- client-side __J__avaScript
- reusable __A__PIs
- prebuilt __M__arkup

---

Advantages:

- We'll be up-to-date with modern technologies
- Clients will see that we can build fast systems
- Easy to build new website prototypes
- Easy to create a company mobile app

---

We'll have good recruitment tasks:

  - create a website using the API
  - create a mobile app using the API
  - create a Progressive Web App
  - create a backend integration with the API

---

We'll be able to say that even our website is built
with the best technology we could find.

---

I started with creating a simple API
exposing some of the content used on the website

- API: https://ifapi.herokuapp.com/
- Website: https://ifapi.netlify.com/

The API is powered by a Mongo database.

The website gets the data from the API
using delays to show what's happening.

---

Demo time

---

It would not be convenient for non-developers so
I started exploring tools to make the process
of content authoring easier and more convenient.

Using a headless CMS seems like the way to go.

---

What can we do:

1. Put content into a headless CMS
2. Create a static website
3. Connect website to the CMS via API

Now all content changes via GUI will be visible on the website.

---

What's a headless CMS?

Something like WordPress admin panel but without the website.

It decouples the content authoring process from the
frontend implementation.

---

Headless CMS works like this:

- a convenient UI is used to easily edit content
- all the data is exposed via API to the frontend

---

We can switch the frontend:

  - without changing the authoring process
  - without exporting/importing existing content

---

The frontend can be:

- a custom website in vanilla JS
- a single-page application (SPA)
- a progressive web app (PWA)
- it can be rendered client-side or server-side
- using Angular, React, Vue, Ember, Aurelia...
- using Disappearing Frameworks like Svelte, Stencil... 
- using a static site generator

---

Tech stack

---

Headless CMS - hosted:

- Contentful - https://www.contentful.com/
- Prismic - https://prismic.io/
- GatherContent - https://gathercontent.com/
- ButterCMS - https://buttercms.com/
- TakeShape - https://www.takeshape.io/
- Kentico Cloud - https://kenticocloud.com/
- Netlify CMS - https://www.netlifycms.org/

---

**Contentful** is used in one of our commercial projects.

Client is familiar with that and it was a requirement but none of us had any prior experience.

It would be safer to learn those tools on internal projects.

---

Headless CMS - installed:

- Strapi - https://strapi.io/
- KeystoneJS - https://keystonejs.com/

---

Static site generators:

- Jekyll - https://jekyllrb.com/
- Next - https://nextjs.org/
- Gatsby - https://www.gatsbyjs.org/
- Hexo - https://hexo.io/
- VuePress - https://vuepress.vuejs.org/

Much more at: https://www.staticgen.com/

---

Static content handling<br>and asset conversion:

- Cloudinary - https://cloudinary.com/
- Uploadcare - https://uploadcare.com/
- Filestack - https://www.filestack.com/

---

Static hosting and CDN:

- Netlify - https://www.netlify.com/

I didn't find anything better yet.

We already use it.

---

Thank you

---

Slides:

[pocztarski.com/ifa](https://pocztarski.com/ifa)

---

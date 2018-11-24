# inFullApi

Hackathon

---

But first...

---

This is how we see ourselves on GitHub:

![](gh-sum-l.png)

---

This is how other people see us on GitHub:

![](gh-sum-i.png)

---

Who are those brave 4 who<br>don't hide that they work here?

Any guesses?

---

![](gh-b4.png)

---

It's even worse on Stack Overflow.

Only 3 people have ever admitted working at inFullMobile.

---

![](so-ifm-c.png)

---

Now back to the hackathon.

---

Problem:

infullmobile.com website is sloooooow.

Especially when accessed from the US.

Not a problem if we don't look for clients there.

Unfortunately we do.

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

Advantages:

- We'll be up-to-date with modern technologies
- Clients will see that we can build fast systems
- We'll be able to create a company mobile app easily
- We'll be able to build and test new website prototypes

---

We'll have good recruitment tasks:

  - Backend: create an API using the database
  - Frontend: create a website using the API
  - Mobile: create an app using the API

---

JAMstack

- client-side __J__avaScript
- reusable __A__PIs
- prebuilt __M__arkup

---

How can we incrementally achieve the goal:

1. Use a headless CMS
2. Import data from WordPress
3. Create a static website based on the current HTML
4. Populate it with the data from the new CMS via API
5. Incrementally improve the website or create new versions

---

It works like this:

- the headless CMS is used to easily edit content with a convenient UI
- it exposes all the data via API to the frontend
- we can switch the frontend without changing the authoring process

---

The frontend can be:

- a custom website in vanilla JS
- a single-page application (SPA)
- it can be rendered client-side or server-side
- it can use Angular, React, Vue, Ember, Aurelia...
- it can use a static site generator

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

Slides:

[pocztarski.com/ifa](https://pocztarski.com/ifa)

---

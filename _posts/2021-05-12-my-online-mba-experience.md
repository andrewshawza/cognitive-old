---
layout: post
title: My Online MBA Experience
featured-img: sleek
mathjax: true
---

# ![PowerMBA Infographic](/assets/images/powermba-infographic-800x487.jpg)

![image-center](/assets/images/image-alignment-580x300.jpg){: .align-center}

Choosing an online MBA over a traditional MBA.

Let’s start with my motivation for doing an MBA.

I have lots of expertise and skills related to my role, product management, IT and development. I started my career as a Travel Agent and moved onto to the IT side with the leading travel technology provider in the world. While I have extensive experience in finance, marketing and even law, I wanted to understand more from an executive point of view in a global business environment that has changed significantly since I did my tertiary education. (think how much the business landscape has changed just in the last 10 to 15 years). I didn’t want a view from the lens of your typical organisation but agile, startup and digital organisations.

I researched a number of traditional online institutions and very few had online programs and those that had still had a part of the course that needed some kind of physical attendance.

Eventually I discovered some online ads and articles about the PowerMBA, so I did my research as I normally do, and I found a winner.

(The infographic was conceptualised by me and I did the design brief to the last detail. I just had to get a freelance designer that was good with hand-drawn personas to actually do the design and make it look good).

1. **Democratizing Education**
This is their catch-phrase I didn’t come up with it. But it’s an accurate description of what they stand for. It’s available to everyone there are no regulations or entry barriers. All MBA programs have strict requirements for entry including work experience and/or educational qualifications.
There is also a lot less flexibility in the programs offered as they need to adhere to ridiculous educational regulations that are not really applicable to today’s business practices.

2. **Affordable**
Less than $1000 and under €900 (approximately) and if you keep an eye out for early-bird specials you can shave even more off that modest price. This is around 10% of the next most affordable, reputable online MBA program.

3. **Time**
You only need 15 minutes a day! We all know that time is one of the most valuable things and something you never get back. Time is even more precious when you have a demanding job or career and want to spend more time with your family and friends. The typical MBA is also infamously know as the “divorce course’.

4. **Easy**
The course content is delivered as micro-learning bit sized chunks, with no heavy-reading and the majority of the content delivered as video content.

5. **No Exams**
Stress free and no studying! Only quizzies that you need to pass at the end of each section to make sure you understand the syllabus.

6. **Relevant**
The content and case-studies are framed around companies that you know, and can relate to. (like Netflix, AirBnB, Waze, YouTube, and more)

7. **Perspective**
Great insights into leadership and tips from successful leaders.
One session in particular was on the topic of mindfulness and how top execs use meditation or similar practices to take mental breaks and just unwind.

8. **Network**
Reading the reviews on Trust Pilot, and from comments from many of the people I have interacted with, this is one of the main reasons why a lot of people join. There are forums on the student portal for work related topics like , as well as networking events that are normally in person (online during COVID) in cities around the world, bookclubs, and “PowerTalks” webinars with guest presenters that are specialists in their field dealing with a wealth of different topics.

9. **Overview**
In general it provides a great understanding of the whole business landscape. It’s a great way to update your knowledge and help with think out-of-the box.

**Dis-Advantages**

**Detail** — there isn’t a lot of detail, summaries are provided for each section but it’s limited. For those that are detail oriented you’ll need to do more in depth research on the topics you’re interested in.

**Masters** — as it’s not a recognised MBA program with the associated degree. They are also adamant that they don’t plan on doing this any time in the future.

**UI** — trying not to be too much of a stickler and taking my product manager hat off, they use the Typeform platform, which I’m a HUGE fan of and use their surveys all the time, it’s just not great as an education platform, the UI/UX is a little buggy and the navigation needs work.



# Getting started

[GitHub Pages](https://pages.github.com) can automatically generate and serve the website for you.
Let's say you have a username/organisation `my-org` and project `my-proj`; if you locate Jekyll source under `blog` folder of master branch in your repo `github.com/my-org/my-proj`, the website will be served on `my-org.github.io/my-proj`.

1. Just download or fork and clone the source from [github.com/janczizikow/sleek](https://github.com/janczizikow/sleek/).
2. Make sure your local machine has ruby and node
3. Edit site settings in  `_config.yml` file according to your project.
4. Replace `favicons` and `_includes/logo.svg` with your own logo.

**Note** that you might have to adjust some CSS depending on the width and height of your logo. You can find Header / Navigation related SCSS in `_sass/layout/nav.scss`.

## Writing content

### Posts

Create a new Markdown file such as `2017-01-13-my-post.md` in `_post` folder. Configure YAML Front Matter (stuff between `---`):

```yaml

---
layout: post # needs to be post
title: Getting Started with Sleek # title of your post
featured-img: sleek #optional - if you want you can include hero image
---

```

#### Images

In case you want to add a hero image to the post, apart from changing `featured-img` in YAML, you also need to add the image file to the project. To do so, just upload an image in `.jpg` format to `_img` folder. The name must before the `.jpg` file extension has to match with `featured-img` in YAML. Next, run `gulp img` from command line to generate optimized version of the image and all the thumbnails. You have to restart  the jekyll server to see the changes. Sleek uses [Lazy Sizes](https://github.com/aFarkas/lazysizes) Lazy Loader for loading images. Check the link for more info. Lazy Sizes doesnt't require any configuration and it's going to be included in your bundled js file.

### Pages

The home page is located under `index.md` file. To change the content or design you have to edit the `default.html` file in `_layouts` folder.

In order to add a new page, create a new html or markdown file under root directory or inside `_pages` folder. To add a link to the page, edit `navigation` setting in `_config.yml`.

### Images TODO

Introduce gulp optimization

Breakpoint | Image Type | Width | Retina
------------ | ------------ | ------------- | -------------
xs |Post Thumb | 535px | 1070px
sm |Post Thumb | 500px| 1000px
md |Post Thumb | 329.375px | 658.75px
lg |Post Thumb | 445.625px | 891.25px
xl |Post Thumb | 353.125px | 706.25px

Breakpoint | Image Type | Width | Retina
------------ | ------------ | ------------- | -------------
xs |Post Hero | 535px | 1070px
sm |Post Hero | 500px| 1000px
md |Post Hero | 329.375px | 658.75px
lg |Post Hero | 445.625px | 891.25px
xl |Post Hero | 353.125px | 706.25px

### MathJax

If you want to use [MathJax](https://www.mathjax.org/) in your posts, add `mathjax: true` in [YAML front matter](https://jekyllrb.com/docs/frontmatter/) of your post:

```yaml
---
layout: post
title: Blog Post with MathJax
featured-img: sleek # optional - if you want you can include name of hero image
mathjax: true # add this line in order to enable MathJax in the post
---
```

#### Example

In N-dimensional simplex noise, the squared kernel summation radius $r^2$ is $\frac 1 2$
for all values of N. This is because the edge length of the N-simplex $s = \sqrt {\frac {N} {N + 1}}$
divides out of the N-simplex height $h = s \sqrt {\frac {N + 1} {2N}}$.
The kerel summation radius $r$ is equal to the N-simplex height $h$.

$$ r = h = \sqrt{\frac {1} {2}} = \sqrt{\frac {N} {N+1}} \sqrt{\frac {N+1} {2N}} $$
Happy hacking!

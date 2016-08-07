[1]:http://markup.tips/htmlftw
[2]:http://markup.tips/settings.html#focus
[3]:https://gtmetrix.com/put-javascript-at-bottom.html
[4]:http://markup.tips/tips/making-your-markup-speak.html#focus
[5]:https://css-tricks.com/why-ems/
[6]:http://markup.tips/tips/adopting-orphans.html#focus

# Web Guidelines 0.1
WIP. Best practices to use when building any web based&nbsp;experience.

«<h2 id="toc">Table of Contents</h2>»

<ol>
  <li><a href="#preface">Preface</a></li>
  <li>
    Making Pages
    <ol>
      <li><a href="#making-pages-accessible">Accessible</a></li>
      <li><a href="#making-pages-audible">Audible</a></li>
      <li><a href="#making-pages-configurable">Configurable</a></li>
      <li><a href="#making-pages-enhanceable">Enhanceable</a></li>
      <li><a href="#making-pages-legible">Legible</a></li>
      <li><a href="#making-pages-optimal">Optimal</a></li>
      <li><a href="#making-pages-usable">Usable</a></li>
    </ol>
  </li>
</ol>

<h2 id="preface">Preface</h2>
As you author the web you should strive to create interfaces any user can access and use with ease. So how do you handle this responsibility? Relax, we'll walk you through it with these simple guidelines, but first you must understand a few things.

Know that your HTML documents aren't written in stone; they are alive. The experience they offer changes as browsers and web standards evolve. What an exciting medium. You've chosen wisely.

As you work through these guidelines your hyper&ndash;text documents will begin to make use of the evolving browsers that interpret them. As new features land in browsers your experience becomes lighter and more enhanced with time. That is the signature of a Front&ndash;End Developer, and you'll learn to sign it in your own way.

<a name="accessibility-is-for-everyone">Understand that accessibility is for everyone</a>. All of us are users all of the time: we use handles to open doors, wheels to drive our cars, and utensils to eat food. Every _tool_ we utilize is something that gives us _access_ to our environment or the ability to complete a task which might otherwise have been impossible, and these tools &ndash; including tools you provide as a front-end web developer &ndash; define what kind of _user_ we are in a given context.

With the many different ways to access the web, and the just-as-many tools to with which to do it, you must keep in mind that one person can be many different users on any given day. As our user shifts a high powered desktop and mouse&ndash;enabled computer to using a cellular low&ndash;power touch device, their method of access changes. If you don't design your UI for the right use cases, even the [fictional](https://standardbeagle.com/the-frp-post-sxsw-part-2-no-average-user/) "average" user you designed for will be left frustrated and locked out of your application.

Herein is the crux of the web's accessibility issue: UIs that _do_ work for the user you target might be difficult or impossible for a disabled person to use. If you start your application with complete, meaningful user access in mind, it will be better for everyone.

The thought of crafting experiences that can be used by anyone daunts you until you discover that accessibility isn't something you have to roll up your sleeves and add to your experience somehow at the end. Authoring pages HTML&ndash;first allows interfaces to be enhanced and a-synchronized in a progressive, rather than an aggressive manor. At ground&ndash;level we have an experience that anyone can access before we even start styling it with CSS and long before we enhance it with asynchronous&nbsp;scripts.

Experiences you create are buildings entered, re-visited, and avoided by a wide audience of users. You'll build skyscrapers of experiences and from the wheel&ndash;chair access ramp on the first floor to the helicopter landing pad on the roof your users will enter the building all to find the same realization: while our abilities may very greatly and change with time we all justly deserve &nbsp;access.

<h2 id="making-pages-accessible">Making Pages Accessible</h2>
We all know the desire to discover, process, and share information is a defining part of the human experience. So, who are we to decide who deserves that experience and who does not? Unfortunately as an industry we deprive groups of users the ability to access experiences simply because some of us are unwilling to build experiences a top semantic hyper&ndash;text. Think about that. Today people use web based apps and services to aid them with sensitive and important areas of their lives. If you find yourself drawing a line between the users that may access your experience and those that may not stop and consider these truths. If you are comfortable with shutting users out don't be surprised if fewer show up to see what your experience to offer as it progressively&nbsp;decays.

> You are a user. So ask yourself, have you acknowledged your reliance on accessibility?

You see, all users are passionate about accessibility whether they realize it or not. They might not know what a11y stands for but if you were to ask them to name their favorite devices and features sure enough you will find it is the accessible experiences that attract them. Let's take Siri for example. First and foremost, Siri is an accessibility feature. Siri is useful to the blind as well as the eagle&ndash;eyed parent trying to pull up directions while managing a van full of hyper kids who just wont their first soccer match. You see regardless of if the person has a permanent or contextual lack of ability they rely on accessibility. They rely on you. Know that when you build accessible experiences you build experiences that are better for anyone in any&nbsp;context.

<h3 id="the-fear">FEAR</h3>
Even those resistant to accessibility best practices gets frustrated when they try to access a non&ndash;responsive and therefore less accessible interface on their smartphone. They care about accessibility too; they just haven't actualized that in their workflow yet. This is likely because they are afraid of their false impression of what they think creating accessible experiences&nbsp;entails.

I encourage you to allow yourself the understanding that fear is often&nbsp;merely:

- <strong>F</strong>alse
- <strong>E</strong>vidence
- <strong>A</strong>ppearing
- <strong>R</strong>eal

So what is the false evidence assumed and why does it appear real to them? They assume accessibility must be "more work" than otherwise. This may not be their fault though. They may have tried to take a non&ndash;accessible experience and &#8220;make it accessible&#8221; without breaking changes long after it has been built. In that case accessibility is not only harder but may be impossible without making significant breaking changes. Imagine trying to install a shower in the middle of a building with concrete floors that wasn't plumbed for it. You'll need a wrecking ball or&nbsp;two. The key is to keep accessibility in mind from the&nbsp;beginning.

Builders have construction codes that set standards for safety and accessibility. When a builder ignores these codes and refuses to do things like make the entrance wheelchair accessible that building begins to rot the community around it. The community isn't a place of inclusion anymore. That's why there are laws about these things. So why is it any different in the digital&nbsp;industry?

Ironically, the hyper&ndash;accessible nature of the web makes accessibility standards more difficult to enforce and standardize than in other industries. It is much more approachable, and therefore accessible, to spin up a web server and start hosting a website than it is to say buy property, obtain the necessary permits and begin breaking ground. You can have the whole thing done in a few hours even with no experience and next thing you know, you are publishing to the web. Anyone can be a publish to the web. Your journey is to graduate from a web publisher to a web&nbsp;architect.

<h3 id="good-news">The Good News</h3>
You've been wondering what the good news is in all this so here it is. Accessibility doesn't have to be any more complicated than you make it. If you [begin your experience by writing semantic HTML][1] then it already was accessible before you screwed it up by making it fancy with that one script library or whatever. If you jumped straight into JavaScript and didn't start with HTML the solution is simple. Start completely over, this time with an HTML&ndash;first workflow. HTML is accessible so make sure you start with&nbsp;it.

<h3 id="authorship-is-everything">Authorship is Everything</h3>
JavaScript is amazing. It gave us the ability to liven what was once a static and synchronous DOM. Modern JavaScript populates and oversees the DOM for us so we stop worrying about it. Here's the problem. The moment you loose authorship of the DOM to scripts you stop architecting the web. Scripts attempt to create a well architected experience but they fool no one when they don't load or a misplaced semicolon breaks your entire experience. Don't be fooled. Remember that as an architect of the web you are responsible for every state of the underlying DOM which makes up the experience of your user just as the Graphic Designer is responsible for each pixel of their&nbsp;design.

<h3 id="first-byte">The First Byte</h3>
Whenever you begin authoring a page for the web you should have one thing in mind: The first byte. The first byte is really the most exciting byte if you think about it. It's the moment a connection is made, and someone somewhere decides to start downloading your document. Then they wait. Hopefully not for long, but either way they are waiting for your experience! What does this experience feel like for your users? Does the page begin loading immediately as a legible text document before the assets loads or is it a blank white screen until everything has loaded and the scripts have executed successfully? Does your infinite-scroll one&ndash;page website have a pagination component available for .no-js users to access content or does it just stop at nothing? Is that fancy custom designed select box actually a better user&ndash;experience than a native `<select>` on&nbsp;mobile devices? Be mindful of what you are serving and how if at all it is blocking your content from loading.

<h3 id="truth-about-poor-ux">The Truth about Poor User&ndash;Experience</h3>
When there is a truly poor user experience the root issue can often be traced back to HTML not being first and foremost in the design and development processes. Either semantic HTML for your experience didn't exist as a base layer or you screwed it up during the process of styling and enhancing it.

<h3 id="allowing-a11y-into-your-experience">Allowing Accessibility into your Experience</h3>
We've established that HTML is inherently accessible. Leverage this by serving HTML upfront. This may mean an HTML&ndash;layer underneath your asynchronous React component. Maybe it is as simple as a few `<noscript>` tags used to inform users that a given component is disabled and requires them to Enable JavaScript to be used. Start with HTML, get as far as you can, and enhance from there. If a component requires something make sure to inform your users of that. For&nbsp;example:

```html
<noscript>  
  <aside class="alert">  
    <p>Please <a class="apparent-link" href="http://enable-javascript.com" target="_blank">enable <code>JavaScript</code></a> for to use this&nbsp;component.</p>    
  </aside>
</noscript>
```

If you do override native inputs at least give your users an option to configure whether or not native components are overridden on their [settings page][2]. That's right, users should have a settings page for just about anything you build even if it is a simple website. We'll get to settings more in the [configurable&nbsp;section](#making-pages-configurable).

The truth is accessibility is the hidden rockstar behind what makes everything cool. Siri, Responsive Design, Dictation, these are really just accessibility features created by designers who reached for creating hyper&ndash;accessible interfaces. It took striving for  hyper&ndash;accessibility to actualize these features that become of benefit to all users. Even those who may not rely entirely on these considerations enjoy them thouroughly. The architects of these considerations started with accessibility in mind and created incredible things. You can too.

<h3 id="a11y-tips">Accessibility Tips</h3>

  - By [sticking components above the fold](http://markup.tips/tips/sticking-components-above-the-fold.html#focus) and using anchor tags to "jump" passed them you can achieve the familiar experience of having an ever&ndash;present navigational component always nearby in a more accessible and responsive manor than say a left&ndash;hand tree component. 
  - Before you put something behind a modal window make sure that content is accessible as HTML in some way. Maybe you link to another page. Maybe you make clever use of an `<iframe>` within a `<noscript>` tag to load one page as a component within another.<br>
  - Before you create that familiar horizontal slider ensure that for `.no-js` users the slides stack vertically so they can all be viewed synchronously.

<h3 id="scripts-at-the-bottom">Scripts at the Bottom of your Process</h3>
Just as you should be [loading your scripts at the bottom][3] of your HTML document, scripts should also come at the bottom of your process. Try to follow a process roughly consisting of:

- Sketch
- Wireframe
- Clickable HTML
- Make HTML pretty with CSS
- Lastly make stuff fancy with JS

 Remember that the inaccessible experience was either born of another process or simply buggered things up a bit in the last two steps. Maybe the CSS is styled in such a way that it doesn't accommodate for how a page is loaded without certain features. Or maybe when the JavaScript was implemented some of the HTML layer was removed rather than enhanced. The key is the third step. By authoring functional HTML with native inputs and synchronous forms before styling and enhancing the experience you will begin baking accessibility into your experiences without even realizing&nbsp;it.

<h2 id="making-pages-audible">Making Pages Audible</h2>
Writing semantic HTML will make your pages usable to people using screen readers to hear, rather than see, your experience. With jquery.speakable.js you can [create your own simple audio component that reads parts of your document][4] as you wish. For example, you could create a component beneath the title that says &#8220;This posts is a 10 minute read but can be listened to as well&#8221; that will play the blog post like an audio track. It's pretty neat, and works with your HTML by offering classes like `.unspeakable` to do things like specify parts of pages that should not be read aloud. You can even do things like make sure each letter of an acronym is spoken as the corresonponding&nbsp;word.

<h2 id="making-pages-configurable">Making Pages Configurable</h2>
Before you create a web interface allow yourself to consider the following configuration options for improving User Experience. Allow your users to:

 - [Change font&ndash;size][2]
 - [Change font&ndash;face][2]
 - Disable font&ndash;face
 - [Enable a High&ndash;Contrast (or other) theme][2]
 - [Configure the voice used to read posts][2]
 - Opt out of loading high&ndash;resolution assets

HTML5 makes this quick and easy with standard features like localStorage.

<h2 id="making-pages-enhanceable">Making Pages Enhanceable</h2>
progressive enhancement, feature detection, semantic, synchronous

<h2 id="making-pages-legible">Making Pages Legible</h2>
Legibility can be overlooked in the name of Graphic Design. I'm guilty of this myself. Designers love clean, crisp, small and sometimes even subtle type. Sometimes we get too carried away with how our content looks than how able it is to be accessed. Usually it comes down to color and contrast. Either we make the type too small or too subtle in color against the background. Soft grays on white are a popular design trend, but if the gray is too soft the type becomes illegible. webaim.org has a wonderful online [Color Contrast Checker](http://webaim.org/resources/contrastchecker/). You put in the foreground and background colors of your design and it will tell you if they are considered safe. Cool!

Regarding type size there are two main things to keep in mind:

  - [Style your CSS layout using em units][5] when appropriate so that your layout handles increasing the browser font&ndash;size well
  - [Give users a way to set their font&ndash;size preference for size and font&ndash;face][2] on their settings page

Setting a max&ndash;width using em units is a great way to ensure a block of text stays legible in wide viewports. Once you reach a certain number of characters without a line break text becomes less legible regardless of size. Typographic orphans occur when the last word in a line or paragraph of text winds up all alone on it's own line. You can [cleverly adopt orphans][6] using a single HTML entity. There are also [RegEx Patterns available](https://github.com/jpdevries/wool) for you to fight all 10 Typographic Crimes.

<h2 id="making-pages-optimal">Making Pages Optimal</h2>
Frameworks are handy, but unless they are silent they are probably heavy. As a Front&ndash;End Developer you should be keeping an eye on the weight of your project. If you are only making use of a small portion of a framework is there a way to do without it or include less of the framework? Maybe you can use silent Sass libraries instead of including large amounts of unused CSS.

Once you start examining each and every byte of your dependencies you may even find yourself question if jQuery is worth the weight. If you can get by with modern VanillaJS your experience will be that much snappier.

Many stress the importance of minifying their assets for production but it is less commonly understood that [minification makes little difference when assets are served over GZIP](https://css-tricks.com/the-difference-between-minification-and-gzipping/). The moral of the story isn't that you are off the hook for minifying assets like CSS and JavaScript. You should still do that. The moral of the story is that GZIP makes a really big difference, so you should make sure you are serving your assets using GZIP compression.

If you author your CSS using Sass you can make use of Silent Classes. Silent Classes allow you to group common blocks of styles together. By making use of silent classes you will be keeping your CSS weight down because selectors will be bundled together to reduce the total number of style definitions in your stylesheet.

Tools like Grunt or Gulp can help you create your own workflow using nothing more than some JavaScript and a few terminal commands. If this is totally new to you check out Chris Coyier's introductory post.

<h2 id="making-pages-usable">Making Pages Usable</h2>
Here's the beauty of these guidelines. This part is automatically inherited from initially [making your pages accessibile](#making-pages-accessible). Yup. You can create a usable experience that isn't accessible but you cannot create an accessible experience that isn't usable. Knowing this simple truth helps us know where to start, with HTML&ndash;first!

<h2 id="conclusion">Conclusion</h2>
These guidelines are nothing more than that, guidelines. Whether you are a complete greenhorn or have been at this for years they exist to help you make sense of this intriquit web we spin. May they assist you in spinning a silk that is of your own and for the world to enjoy.

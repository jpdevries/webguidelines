[1]:http://markup.tips/htmlftw
[2]:http://markup.tips/settings.html#focus
[3]:https://github.com/jpdevries/webguidelines
[4]:http://markup.tips/tips/making-your-markup-speak.html#focus
[5]:http://youmightnotneedjquery.com/#request
[6]:https://github.com/jpdevries/webguidelines#making-pages-usable

# Manager Interface Guidelines 0.0
WIP. Best practices to use when building any web based manager&nbsp;experience.

<h2 id="toc">Table of Contents</h2>

<ol>
  <li><a href="#preface">Preface</a></li>
  <li>
    Making Manager Interfaces
    <ol>
      <li><a href="#making-pages-accessible">Accessible</a></li>
      <li><a href="#making-pages-accessible">Asyncronous</a></li>
      <li><a href="#making-pages-configurable">Configurable</a></li>
      <li><a href="#making-pages-enhanceable">Enhanceable</a></li>
      <li><a href="#making-pages-future-proof">Future Proof</a></li>
      <li><a href="#making-pages-fun">Fun</a></li>
      <li><a href="#making-pages-legible">Legible</a></li>
      <li><a href="#making-pages-lightweight">Lightweight</a></li>
      <li><a href="#making-pages-syncronous">Syncrounous</a></li>
      <li><a href="#making-pages-usable">Usable</a></li>
      <li><a href="#making-pages-responsive">Responsive</a></li>
    </ol>
  </li>
  <li>
    <a href="#authoring-framework-agnostic-apis">Authoring Framework Agnostic APIs</a>
  </li>
  <li>
     Register Client Scripts Responsively
  </li>
  <li>
    Leveraging the Browser Cache
  </li>
  <li>
    Progressively Enhancing Standard Form Elements
  </li>
</ol>

<h2 id="preface">Preface</h2>

As you create interfaces that enable users to author the web keep in mind the [guidelines for creating&nbsp;webpages][3] as well as the guidelines&nbsp;below.

## Making Manager Interfaces Accessible
Accessibility isn't just about screen readers, keyboard support, or `.no-js` support. Nor is it just about responsive design, ARIA roles, and safe color contrasts ratios. To keep things accessible, keep your most inaccessible denominator in mind. Who is your furthest user? Is it a desktop on a broadband connection or a mobile user on a pay-per-byte connection in Africa? Whoever your lowest common denominator is, design for them. Otherwise, you'll always be left wondering what users are left beyond your interface's reach.

## Making Manager Interfaces Asynchronous
Once your manager interface is functional as synchronous pages you are ready to enhance your interface. By making your interface synchronous with an [HTML-first][1] approach, data for your your application that may otherwise be loaded by scripts may be already accessible in the page. Take these opportunities to keep your JavaScript layer lightweight by capitalizing what is already part of the DOM it is enhancing.

## Making Manager Interfaces Configurable
You've taken on an interesting challenge. Designing a manager interface means designing for a wide variety of people. And any one person can be a number of users throughout the day. How could we possibly satisfy them all with the same styles? We can't, so we don't. Create a simple settings page for your interface that contains components that allow users to choose form a variety of `font-family`, `font-size`, and color contrast options. Within these components, use JavaScript to listen for updates and store the most recent values of each component using `localStorage`. Users can now easily communicate with the interface and let it know how they would like it to be customized! This is a great example of JavaScript being used to enhance accessibility.

## Making Manager Interfaces Enhanceable
By starting with asynchronous and framework agnostic HTML, our interfaces are inherently enhanceable. Since the API is framework agnostic and doesn't require any particular framework, plugin developers have the choice of using any framework or none. To keep your manager interface enhanceable, keep it out-datable and built with web standards.

## Making Manager Interfaces Future Proof
When using semantic versioning for our interfaces, we can't go making breaking changes over night. This means that one of the expenses to using a framework within our API is that if that version of or the framework itself become outdated so do we. Web Standards don't go stale. By building a framework agnostic API upon web standards, we anxiously anticipate new features that land in browsers rather than fear the irrelevance they would bring to a datable codebase.

## Making Manager Interfaces Fun
All seriousness aside, you owe it to your user to allow them to have a little fun. Simple CSS animations and other clever interactions make an interface less of a bore to use. Make an effort to keep your interface not just usable but fun to use.

## Making Manager Interfaces Legible
By making your manger interface configurable with `font-size` and `font-family` preferences you have already made your interface capable of becoming more legible to each individual user. In addition to allowing the legibility of your interface to be configured, keep in mind color contrast ratios, particular eye conditions, and relative luminosity. Using the HTML5 Luminosity API, you can detect the current amount of light reported by the user's device. This allows you to create interfaces that automatically enter "high contrast" dark modes in dim light conditions. By allowing users to switch the dark themes to always be enabled, users with particular eye conditions are given a more legible experience any time of day.

## Making Manager Interfaces Lightweight
Staying away from frameworks helps keep things light, at least until we start using them. It is important to understand that weight is relative to the environment of the DOM. If no frameworks are used, VanillaJS is by far the lightest approach. If frameworks are already being loaded, using a driver specific to that driver may lighten the end payload of the components that make up your interface. Meaning VanillaJS would not be the lightest approach. There are no absolute certainties when optimizing for the web. Keeping in mind the context of the environment you are designing will keep your interface lightweight and responsive.



## Making Manager Interfaces Synchronous
Authoring your interfaces with progressively enhanced HTML allows for an accessible and lightweight experience, but without synchronous pages to handle standard forms they may not be fully functional. It goes without saying that many of the forms in your manager interface will be asynchronously enhanced. Prior to enhancing these forms, test them as standard `<form action>` submissions. Not only will this make your interface accessible in the absence of scripts, it will make your app your stable in the presence of script breakages. JavaScript layer busted on an extra semi-colon? Good thing there is an HTML layer underneath&hellip;



## Making Manager Interfaces Usable
In addition to [guidelines for making web pages usable][6], manager interfaces pose a unique challenge when author for end users. Most websites are designed for consumption. Users come along and eat up all the bytes. Manager interfaces are different. They are designed for authoring, developing, editing, and consuming. Understanding that manager interfaces pose this unique challenge is important. How you keep your manager interface usable will be up to you. Will you create different themes for different user groups? Will you use analytics to change the interface as it is being used? Don't forget that at the end of the day, the best way to know if your interface is usable is do user testing on your target audience. Take any opportunities to conduct user testing without hesitation. Remember that negative feedback from someone who is not part of your target audience may not necessarily be a bad thing.

## Making Manager Interfaces Responsive
Responsive Design is a radical trend. There is an appealing vastness to it. When you consider how your manager interface should respond, challenge yourself to think outside of the width of the viewport. What else should your interface respond to? As your users manage content within your management interface they educate you on both what they use your interface to do and how they prefer to use it. As the architect of a manager interface, you have a valuable opportunity to respond to the habits and preferences your users share with you.

Are you recording user actions in your database that could be used to cleverly present users with widgets and components that are relevant to their recent or most recently performed actions?

The database isn't the only place to look for data to respond to. The JavaScript Session Storage and Location Storage API can be used to store user preferences, actions, or anything else!

<h2 id="authoring-framework-agnostic-apis">Authoring Framework Agnostic APIs</h2>

Web Standards are constantly evolving in an era of browsers that continuously update themselves. There's never been a better time to keep the dependency of a framework out of your API. "VanillaJS", or in other words IE9+, [allows for XHR requests to be made][5] to send and receive data from the server with plain old JavaScript! By writing VanillaJS you'll be giving up some of the "shortcut" familiarities of your favorite library, but your API will lightweight and less opinionated. You'll be directly using the native APIs of JavaScript meaning as part of the browser your API updates itself automatically overnight. For example take this excerpt from&nbsp;[youmightnotneedjquery.com](http://youmightnotneedjquery.com/#request):

#### VanillaJS
```
function getAJAX(url) {
  var request = new XMLHttpRequest();
  request.open('GET', url, true);

  request.onload = function() {
    if (request.status >= 200 && request.status < 400) {
      // Success!
      var resp = request.responseText;
    } else {
      // We reached our target server, but it returned an error

    }
  };

  request.onerror = function() {
    // There was a connection error of some sort
  };

  request.send();
}
```

With VanillaJS, your dependency payload is 0kb and you don't have to worry about frameworks becoming outdated or out of style. This isn't to say that frameworks and libraries don't have their appeal as well. When using a framework or library, do so as a driver by mimicking the same functionality using your dependent API:

#### jQuery
```
function getAJAX(url) {
  $.ajax({
    type: 'GET',
    url: url,
    success: function(resp) {

    },
    error: function() {

    }
  });
}
```

If you must leverage a framework in your API, leverage it as a driver. This way, user running AngularJS can implement the AngularJS "js-driver", users running React can implement the React "js-driver" and users not necessarily running either implement the standard VanillaJS driver. With test-driven development and managers of each driver, tests can be written, passed in VanillaJS, forked and modified to pass in the given framework or flavor, then submitted back as a driver. Without this sort of process, framework agnostic drivers probably aren't plausible. You can't have features being development on a whim within a driver. Test need to be written, passed in the default driver, and enhanced with frameworks and libraries. Framework Agnostic JavaScript APIs are a lot to maintain but they achieve a heroic like ability to step into any environment as an efficient and compatible enhancement.

## Framework Agnostic Components
When creating websites we have a great deal of control over what frameworks, if any, we chose to use. When creating dynamic manager interfaces that support plugins all control goes out the window. To design lightweight components, design them with responsive drivers.

Similarly to <a href="#authoring-framework-agnostic-apis">authoring Framework Agnostic APIs</a>, components can be enhanced with individual drivers. This allows them be efficiently included within a number of different environments with the same look and feel, the same features, but a different driver powering things under the hood. In theory, you should be able to swap between drivers of your components with no indication of difference between the two detected by your user. The need for framework agnostic components presents itself after you've authored a VanillaJS component and realized that while your component can justly claim a light payload, when it is included within certain environments it may actually become bloated. How could this be so? Let's say your VanillaJS script has a payload of 600kb. If your script were flavored with AngularJS instead, it could weight only 400kb. AngularJS itself weights 700kb. For a page loading this component alone, it would not make sense to add 700kb for a savings of 200kb. However, when your component is used within an environment that is already leveraging and depending on Angular anyways, now your VanillaJS driver has 200kb of bloat. With no additional cost to using AngularJS, your AngularJS driver now has a net savings of 200kb.


## Register Client Scripts Responsively
Now that your components are flexible and enhanceable with a variety of js-drivers they are ready to respond to whatever environment they become apart of. Use feature detection in your scripts to detect your targeted frameworks and decide which to load.

## Leveraging the Browser Cache
When creating websites, front end assets are commonly concatenated together to reduce the number of HTTP requests. When creating manager interfaces, combining assets together can actually become anti-optimization by increasing the payload as users browse from page to page. Techniques like reducing HTTP requests and inlining critical styles are designed to optimize initial page loads. They do not target return visits or visits to pages within the same site. Remember that you are designing a manager interface not a website. The two are not the same and do not have the same optimization best practices. When designing multi-page experiences sit back and let the cacheable HTTP request pile up. By allowing the assets to load independently they are commonly cacheable across pages.

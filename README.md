# Research-Towards-MVP-Capstone-



# Intro Web Design & Development
## Understanding the web

### Client and Servers
## 10:00 am cst - 11:00 am cst Preparing and heading to library 
## 11:00 am cst - 2:00 pm cst Outline and brainstorm mvp and how to set it up and what i want to do and technoology to use:

Additonal Tech Stack Added:
Responsive Design: Utilize CSS frameworks like Bootstrap that you're already considering, or Tailwind CSS, which offers utility-first styling. These frameworks facilitate responsive design, ensuring your web page adapts to various screen sizes and devices.

Progressive Web App (PWA): Convert your application into a PWA to allow offline use, fast loading times, and an app-like experience. This involves implementing service workers, a manifest file, and ensuring your site is served over HTTPS.

API Management: For external APIs like Google Custom Search and YouTube, consider using an API gateway or management layer to handle API requests efficiently, cache responses, and manage quotas or rate limits.

Frontend Frameworks: Although not strictly necessary, using frontend frameworks like React, Vue, or Angular can enhance user experience through more dynamic and responsive interfaces. These frameworks also facilitate state management, which can be beneficial for real-time updates.

SEO Optimization: Ensure your application is search engine optimized, especially since it's content-rich. Implementing server-side rendering (SSR) or static site generation (SSG) with frameworks like Next.js (for React) can improve SEO and performance.

Security Measures: Implement proper security measures, including HTTPS, CORS policies, content security policies, and sanitizing user inputs to protect against common web vulnerabilities (like XSS and CSRF attacks).

Performance Optimization: Use tools like Google Lighthouse to analyze and improve performance, accessibility, and best practices. Optimize assets (images, CSS, JavaScript) for faster loading times.

Analytics and Monitoring: Implement analytics to track user behavior and monitor the application’s performance using tools like Google Analytics and error tracking services like Sentry.

Real-time Updates of UFC Fighter Stats:

Frontend: Display fighter statistics in a dynamic section of the webpage.
Backend: Use Node.js and Express to create an API endpoint for fetching fighter stats.
Data Handling: Initially, use mock data stored in SQLite or in-memory to simulate real-time stats.
Real-time Mechanism: Implement Socket.io to push updates from the server to the client.
VS Battle Feature:

UI Components: Create a section where users can select two fighters from a list or dropdown.
Battle Logic: Develop a simple algorithm to decide the winner based on the fighters' stats.
Display Results: Show the winner's name and a basic congratulatory message.
Search Feature:

Search Bar: Implement a text input for searching fighter names.
Autocomplete: Add a JavaScript event listener to the search field to fetch and display suggestions as the user types.
Search Results: Display the selected fighter's basic profile and statistics on a separate page or section.

##  2:30 pm cst - 3:00 pm cst Servers and Clients
- [Let's start with servers. This is a word referring to either software or hardware that serves files or websites to computers which request them. Sometimes, the server software runs on the server hardware, and sometimes the server software is located elsewhere.](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/understanding-clients-and-servers?autoSkip=true&contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)
- T[he server room. It's an over air conditioned space with scores of computers on racks, wires everywhere,](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/understanding-clients-and-servers?autoSkip=true&contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#) [In this case, this is the server as hardware, a very powerful computer that's designed to handle many simultaneous connections, and serve up files as requested.](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/understanding-clients-and-servers?autoSkip=true&contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)
- [But what causes those files to be served up? That's the server software that executes those commands. There are different types of server software like database servers, cloud computing servers, file servers and web server software. Web server software is what we are interested in, and there's several makers of this software. Some of it is free and open-source like Apache or NGINX. Some are proprietary from big companies like Oracle, Microsoft and IBM. When web server software runs on web server hardware, and that system is maintained by a company who will sell you some space on it that is referred to as a web host or hosting.](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/understanding-clients-and-servers?autoSkip=true&contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)
- [A client is the device that talks to the web server to get web pages to display. On a typical Mac or PC computer, the client is the web browser like Firefox, Chrome, Safari or Edge. Your phone or tablet may have different choices for web browsers, but they still function the same way. The client does not have to be a typical web browser. For example, if you've used Netflix, Hulu, Disney+ or similar services on your TV, you're working with a client as well. These clients connect to the appropriate server to send you TV shows and movies on-demand. Regardless of what the client is, it's job is to request materials from the server, and display them on the client's screen. You enter a web address in the browser or you choose a movie on the application. That request is sent over the internet to the appropriate server. The server gathers codes, images, video, audio or whatever else is needed to render the display, and it sends it all back to the client computer. The client receives those assets, and follows the code to assemble the pieces appropriately to fill your request.](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/understanding-clients-and-servers?autoSkip=true&contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)
- T[he web client is the device in front of you, which runs some type of software that allows you to connect to a desired web server. The web server will send you the pages you request.](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/understanding-clients-and-servers?autoSkip=true&contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)


### Native apps vs Web Apps 3:15 pm cst - 3:50 pm cst

- [Both native and web apps run on phones and tablets.](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/understanding-native-apps-vs-web-apps?autoSkip=true&contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)
- [A native app, is an app design for a specific operating system, like IOS or Android. Native apps are often are coded using programming languages, like C++, Java or Swift, among many other choices. These languages require compiling, before they can run on a given device. Each platform provides their own interface elements and development tools for creating native apps. Compilers, interface elements, development tools and debugging mechanisms, are often distributed in the form of a software development kit or SDK. Because there's a large programming overhead to native apps, they tend to be more expensive to build. Once built, native apps are placed in the appropriate location for downloading, often the App Store or Google play. There may be requirements for having your app listed in these locations. Alternatively, you can ask website visitors to download your native app. In any case, site visitors must download and an install the app on their device to use it. Native apps may run offline, not requiring a constant connection to the internet. For example, consider Gmail. If you're using the Gmail website for writing and sending an email, it gets very upset if you're not connected to the internet while you're writing. Indeed, it may lose part of your email. However, if you're using the Gmail app on a phone or a tablet, you may write an email when the phone is not connected to the internet, then send the email when you are back in touch.](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/understanding-native-apps-vs-web-apps?autoSkip=true&contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)
- [Web apps are very different from native apps. Although their user interface may often look or feel the same. A web app always runs through a web browser. There's nothing to download, to use it. Simply visit the website on your device, using your standard web browser and you'll be able to access the web app. The Gmail website is an example of a web app. These days, web apps are often built with JavaScript, HTML, and CSS, which we'll discuss in more detail later in the course. Web apps may talk to databases, located on web servers. In this case, there may be some server side programming languages involved, like PHP, Python, Ruby, or of more JavaScript. No compiling is needed for web apps to run and there's no app store for web apps](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/understanding-native-apps-vs-web-apps?autoSkip=true&contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)

### Understanding Web Browsers 4:00 pm cst - 4:15 pm cst

- [A web browser is the software you use to see websites.](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/understanding-web-browsers?contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)
- [A browser is designed to communicate with the web server, request pages, receive those pages, and display the code, images, video, audio, and other assets received inside of a webpage. Browsers understand only three types of code; HTML, CSS, and JavaScript.](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/understanding-web-browsers?contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)
- [The W3C, the World Wide Web Consortium, writes the standards for HTML, CSS and JavaScript among other technologies. The specifications describe exactly how the code should work and function. The browser manufacturers should follow these specifications exactly so all webpages work the same way.](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/understanding-web-browsers?contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)
- [Web developers use websites like caniuse.com to find out the browser support for various HTML elements, CSS properties, and JavaScript methods. They also use websites like MDN web docs for documentation of code and other reference materials. In general, developers tend to use Firefox and Chrome for their development work because of their longstanding friendliness to developers and because these browsers run on both Mac and PC computers](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/understanding-web-browsers?contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)

## Planning and Prototyping

### Understanding UX and Website Planning 4:30 pm cst - 5:15 pm cst

- [User experience, or UX, refers to the experience someone has when interacting with a product or service. From finding a service in Google, to understanding a product offering, to purchasing the product and sharing a review, UX is about managing website visitors perceptions of ease of use and getting things done quickly.](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/understanding-user-experience-ux-and-website-planning?contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)
- [Everyone has had the experience of being completely lost about what to do next on a website. If you can't find the link, can't understand the product offering, or misunderstand what you're being asked to do, that's a UX fail in process.](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/understanding-user-experience-ux-and-website-planning?contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)
- [UX practitioners are all about identifying and eliminating those moments in existing products and preventing those moments in new products.](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/understanding-user-experience-ux-and-website-planning?contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)
- [However, by most definitions, a UX professional may be a generalist or a specialist in one area of UX. Generalists often work with small businesses, start-ups, and nonprofits through the entire UX process](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/understanding-user-experience-ux-and-website-planning?contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)
- [They identify organizational, user, and website goals. They define and refine the target audience, the group of individuals who need this product or service. They study how problems are solved now, how they could be solved in the future, and how we could simplify the process of solving those problems. They may create prototypes and test them with members of their target audience to help create specifications and pass to an engineering team to implement.](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/understanding-user-experience-ux-and-website-planning?contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)
- [UX Specialists focus on one area of UX in a deep way](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/understanding-user-experience-ux-and-website-planning?contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)
- [UX professionals are open minded, ready to receive feedback from users and managers. They also have some strong opinions about what makes users happy and what makes a great interface, but they're also ready to let those opinions go if testing shows they're wrong. UX professionals rarely write code themselves, however, they should understand the coding process so that they're better able to communicate with their team and understand what makes a codable interface](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/understanding-user-experience-ux-and-website-planning?contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)
- [The most popular product for this is Figma, but Sketch, Adobe XD, Envision, or Balsamiq are other common choices among many others. And, finally, UX professionals rely heavily on sticky notes for creating workflows and organizing information. By the very nature of this work, UX professionals talk to people a lot. They talk with management, with people on the development team, and with people in their target audience.](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/understanding-user-experience-ux-and-website-planning?contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)

## Understanding UI 5:15 pm cst - 5:30 pm cst

- [UI designers focus on the interface, or the front end of the website or application. That's the customer facing portion of the site. The part you see when you visit any web site.](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/understanding-user-interface-ui-design?contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)
- [You might be an interaction designer, a UI specialist, a front end designer, or a front end developer, or you might just be a web designer. Whatever the name, the UI designer is a bridge between the UX researchers and the graphic designers and the programming team.](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/understanding-user-interface-ui-design?contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)
- [JavaScript will focus on the interface primarily and much less on other aspects of programming. Some UI designers are deeply focused in one of these areas, or they're generalists or more fluent in several areas of UI design. As the UI designer bridges research and programming, they're familiar with tons of software. They are experts in Figma, Adobe XD, or similar prototyping tools that the UX team uses. They know a little bit about the Adobe products that the graphic design team uses for making logos, icons, and other graphics. They also have software for editing code. Examples include Sublime Text, VS Code, Brackets, or Adam. Commonly, UI specialists will also interface with the command line and services like Git, GitHub, and Node.js UI designers have mixed days in terms of meetings and focused work](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/understanding-user-interface-ui-design?contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)

## Prototyping tools 5:36 pm cst - (wip) 
## 12:00 pm cst - 4:00 pm cst for the 
- [Prototyping is the process of creating a model of a future product.](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/prototyping-tools?contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)
- [A prototype needs to be created quickly and changed easily because it's likely that several versions of a prototype will be required before the right version is created. With each prototype, a round of user testing is typically performed, analyzed, and measured, and changes are made. To keep costs low and possible interfaces high, prototyping software is often used. With prototyping software, no coding is required.](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/prototyping-tools?contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)
- [Eliminating the coding process is critical to moving quickly and making changes. Prototyping software typically features a drag and drop interface, often with several preconfigured interface options like buttons, search boxes, form elements, navigation bars, and more. You can import graphics like logos and photos. Often, you can add links between prototype screens and small animations when something is clicked. Let's take a quick peek at some prototyping software to see how this type of software looks and functions](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/prototyping-tools?contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)
- FIGMA WALKTHROUGH REFER TO VIDEO TO KNOW EXACTLY WHATS HAPPENING IN VIDEO = [- This is Figma. You can sign up for a free account at figma.com. I wanted to briefly walk you through the kinds of problems that Figma happens to solve. So this is the dashboard. Once you have created an account and logged in you'll see something like this. You'll see you'll have the ability to create several kind of files. So you can create the type of file for designs and prototypes, I'm going to show you one of those in a moment. You'll have the ability to create a FigJam file, which as it says here, is like whiteboards, diagrams, sticky notes, that kind of thing. I'll show you that in a moment, as well. Or you can import a file from someplace else. So maybe you have somebody else's Figma file or you have a file from some other program like Sketch. Using the Figma Community, which is over here on the left-hand side, I found some examples for us to just briefly take a look at. So here's an example of a webpage layout that comes from the community. Somebody already designed this for you to take a look at with the intention that you can learn Figma from this or you can take this and tweak it a little bit and turn it into a different kind of design. So those of you who are familiar with Photoshop, you'll notice this might look somewhat familiar. We have various types of layers and so forth over here on the side. So as I click on things, you can see, we are selecting different elements here on the page, okay? There's that tiny emoji up there at the top. You of course can zoom in or zoom out, zoom to fit, whatever is best for you. Let's zoom in a little bit. So for example here, in this box, I might want make some changes to this. I can, of course, double click on this and change the text, "I want to work from home every day," or whatever changes you wanted to make here. You could select other elements. This is a grouping here, we group inside of this. There's a vector diagram, there's some text associated with this, and then there's this little icon here. We could turn off the eyeball, that would remove that from view. We could also select this little guy here, maybe we get rid of that. Then we can just continue to make changes here. We can make changes to colors. As you see here, the background for this, let me zoom back out again so we can see this. The background for the page overall is this light gray color. We could easily change that background color to something else, maybe this dark gray. And you'll notice that these are in hexadecimal format. We've talked about that other places in the course. So those colors that might come to you from some kind of branding document in hexadecimal format, you can just type those colors right into Figma and make use of them. So this is the kind of thing that you can expect here within Figma for laying out webpages. You have the ability to place shapes and images and so forth. You have some basic drawing tools that are available to you. You have some text tools that are available, and you can make comments and share these with your team. Let's take a brief look over here at a FigJam document. So this is somewhat the same, but also somewhat different. The FigJam functionality I think would be most used by people who are working with user experience. In other words, they are researching and planning some kind of document rather than putting together the actual graphic design or a true interface prototype. This is from earlier in the process of developing a website or web application. In this case, I'm looking at the consumer journey map here. And, as we have done before, we can zoom in and take a closer look at this. So we have an introductory graphic that we have here. We have the ability to put in information about a persona that we might be working with, and we could make a graph here. We have sticky notes that are spanning across these four boxes. This is a pretty common sort of technique that UX people use for organizing a customer journey. So how are people interacting with your product or service from when they find it all the way through until they purchase it, and how are they using it to address problems within their lives? So here we have Actions, Experience, Opportunities, and Pain Points. These sticky notes could easily be rearranged, you can just click and drag. We aren't zoomed in far enough to read what they say. There actually isn't any text on these, but as you can expect, you'd double click on this and say, "This is a sticky note." So there's the sticky note. If we wanted it to be a different color, we have a few choices. We can pick a different color for our sticky note. Down here in our tray, we have the ability to click and drag and add other ones here. We can also click and drag other shapes, and of course, there are many choices of shapes to choose from. That would be useful if you were putting together something like a flow chart, which is a pretty common type of way of planning some kind of functionality inside of a web application. We have the ability to draw on the page, so I can make some kind of drawing here, and it smooths it out for me really nicely. We have the ability to put in various kinds of stamps. So if I really love this particular sticky note, I can put hearts on it. We also have the ability to add silly things here. These are just stickers and so forth, and wow, that's a really great idea. Let's label it as "Fresh." So this is just a very brief overview to give you an idea of what Figma is and how it works. There are two sides to Figma. Side number one that I'm looking at right here is this whiteboarding, sticky note, planning, diagramming type of tool which is called FigJam. And the other side of it is more typically used for planning webpages and prototyping site designs, where you can put in all kinds of pretty elements to the interface, line things up, and truly draw out what a webpage will look like.](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/prototyping-tools?contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)
## Graphic Design Tools
- Many professionals if not all prefer to work with adobe photoshop and illustrator
- [Most professional graphic designers learn the Adobe suite of tools as part of their education. They are experts at two packages in particular. Illustrator is used for illustrations and logos. If it's a drawing, illustrator is often the place to do it. Illustrator's files are vector files, which means they're composed of math that describes the curves and lines in the illustration.](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/graphic-design-tools?autoSkip=true&contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)
- [As such, these kinds of drawings may be displayed online using the SVG format or scalable vector graphic. These graphics load quickly because of their small file size. Photoshop was originally used for processing photos, including cropping, cleaning them up, annotating them, and more. Photoshop produces raster graphics or graphics made up of individual pixels. Exported images are usually in GIF, PNG, or JPEG format to display on the web](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/graphic-design-tools?autoSkip=true&contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)
- [Many graphic designers are starting to incorporate Figma into their work as well. While Figma is primarily a prototyping tool, it does offer some basic graphic design tools for creating quick logos and other graphics for your site. If you're not a professionally-trained graphic designer but you're called on to do the occasional graphic design work, you may want to take a look at Canva. Canva offers a ton of templates to start many types of graphic design work. It offers color palettes, easy type choices, and a simple interface for creating graphics that look good without a steep learning curve. If you have no background in graphic design, Canva is not a bad choice to start work. It has a free plan so you can give it a whirl without commitment.](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/graphic-design-tools?autoSkip=true&contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)

## 4:20 ish pm -5:00 PM Hands on linkdein learning "Three tech of frontend" & "writing code" both of which i wrote notes on and practiced on my creation of my new portfolio project (https://github.com/simioyin222/Portfolio) 

## Supporting Web Development Technologies

## Understanding HTML

- [HTML is the hypertext markup language. HTML is all about identifying commonly used structural elements like paragraphs, headings, lists, links, and more. Computers understand the structure of a document through this type of markup.](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/understanding-html?autoSkip=true&contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)
- [This is made up of opening and closing tags. In this case, the A tag. A stands for anchor, and it's used in creating links. When we talk about the two tags together, this refers to the element. You'll notice in the opening tag, we have a few modifiers available to us called attributes. The href attribute stands for hyper text reference. In other words, where do we want this link to go? The target attribute addresses where we'd like this link to open. In this case, we wanted to open it in a new window or tab in the browser rather than the default behavior of the same window or tab. The words in between the opening and closing tags are the text affected by the tags.](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/understanding-html?autoSkip=true&contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)

## Understanding CSS

- No new info 

## Understanding Javascript

- JavaScript and Java have nothing to do with each other. Java is used more for applications, particularly in Android-based applications and in big data. JavaScript was born on the web and continues to live there. Like CSS, JavaScript is usually contained in its own documents and linked to the HTML page where it will execute. Since JavaScript is a programming language, it includes many of the same elements you find with other languages.

## What is Framework
- [framework is some pre-written code that you may use to create all or part of your website or web application.](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/what-is-a-framework?autoSkip=true&contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)
- [Frameworks often consist of CSS and JavaScript. Some rely on your HTML being crafted in a specific way for the framework to function correctly. A commonly used framework that's beginner-friendly is Bootstrap, found at getbootstrap.com.](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/what-is-a-framework?autoSkip=true&contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)
- [With Bootstrap, you may create website layouts, buttons, color and font schemes and functionality like dropdowns, hamburger buttons, accordions and modal windows. More recently, JavaScript frameworks have become wildly popular. Facebook's React, Open-source Vue and Google's Angular are the three most encountered frameworks for front-end development](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/what-is-a-framework?autoSkip=true&contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)
- [Frameworks in general are often used for two major reasons in programming. The reason that most people want to discuss is that a framework significantly speeds up development time for building websites and web applications. A significant portion of the code is already written. Some parts of the framework may be designed for quick customization. Often, that's things like colors, fonts, layout options and so forth. Developers may also write additions to the framework to make their customized solution for a client. Frameworks are maintained by a team of people and are often free so the code will be updated on a regular basis.](https://www.linkedin.com/learning/introduction-to-web-design-and-development-14628245/what-is-a-framework?autoSkip=true&contextUrn=urn%3Ali%3AlyndaLearningPath%3A56d7a7053dd559b764b88a92&resume=false#)
- Could be seen as a crutch

## CHAPTER QUIZ
- PASSED

## 5:00 PM - 6:00 PM  writing code (will place portofolio code here, still working on it so give me a second as used for practice) :
HTML:
<div class="overlay-navigation">
  <nav role="navigation">
    <ul>
      <li><a href="#" data-content="The beginning">Home</a></li>
      <li><a href="#" data-content="Curious?">About</a></li>
      <li><a href="#" data-content="I got game">Skills</a></li>
      <li><a href="#" data-content="Only the finest">Works</a></li>
      <li><a href="#" data-content="Don't hesitate">Contact</a></li>
    </ul>
  </nav>
</div>

<section class="home">
  <a href="https://codepen.io/fluxus/pen/gPWvZm" target="_blank">Click for a slightly nicer Velocity.js version</a>
  <div class="open-overlay">
    <span class="bar-top"></span>
    <span class="bar-middle"></span>
    <span class="bar-bottom"></span>
  </div>
</section>

CSS:
HTML CSS JSResult Skip Results Iframe
@import url(https://fonts.googleapis.com/css?family=Work+Sans:400,300,700|Open+Sans:400italic,300italic);
body {
  background-color: #fff
}

.home {
  width: 100%;
  height: 100vh;
  position: relative;
  background-image: url(https://images.unsplash.com/photo-1446771326090-d910bfaf00f6?ixlib=rb-0.3.5&q=80&fm=jpg&crop=entropy&s=9216e1a8598a8530ce329b41a8f3725d);
  background-size: cover;
  background-position: center center;
}

JS:
$('.open-overlay').click(function() {
  var overlay_navigation = $('.overlay-navigation'),
    nav_item_1 = $('nav li:nth-of-type(1)'),
    nav_item_2 = $('nav li:nth-of-type(2)'),
    nav_item_3 = $('nav li:nth-of-type(3)'),
    nav_item_4 = $('nav li:nth-of-type(4)'),
    nav_item_5 = $('nav li:nth-of-type(5)'),
    top_bar = $('.bar-top'),
    middle_bar = $('.bar-middle'),
    bottom_bar = $('.bar-bottom');

  overlay_navigation.toggleClass('overlay-active');
  if (overlay_navigation.hasClass('overlay-active')) {

    top_bar.removeClass('animate-out-top-bar').addClass('animate-top-bar');
    middle_bar.removeClass('animate-out-middle-bar').addClass('animate-middle-bar');
    bottom_bar.removeClass('animate-out-bottom-bar').addClass('animate-bottom-bar');
    overlay_navigation.removeClass('overlay-slide-up').addClass('overlay-slide-down')
    nav_item_1.removeClass('slide-in-nav-item-reverse').addClass('slide-in-nav-item');
    nav_item_2.removeClass('slide-in-nav-item-delay-1-reverse').addClass('slide-in-nav-item-delay-1');
    nav_item_3.removeClass('slide-in-nav-item-delay-2-reverse').addClass('slide-in-nav-item-delay-2');
    nav_item_4.removeClass('slide-in-nav-item-delay-3-reverse').addClass('slide-in-nav-item-delay-3');
    nav_item_5.removeClass('slide-in-nav-item-delay-4-reverse').addClass('slide-in-nav-item-delay-4');
  } else {
    top_bar.removeClass('animate-top-bar').addClass('animate-out-top-bar');
    middle_bar.removeClass('animate-middle-bar').addClass('animate-out-middle-bar');
    bottom_bar.removeClass('animate-bottom-bar').addClass('animate-out-bottom-bar');
    overlay_navigation.removeClass('overlay-slide-down').addClass('overlay-slide-up')
    nav_item_1.removeClass('slide-in-nav-item').addClass('slide-in-nav-item-reverse');
    nav_item_2.removeClass('slide-in-nav-item-delay-1').addClass('slide-in-nav-item-delay-1-reverse');
    nav_item_3.removeClass('slide-in-nav-item-delay-2').addClass('slide-in-nav-item-delay-2-reverse');
    nav_item_4.removeClass('slide-in-nav-item-delay-3').addClass('slide-in-nav-item-delay-3-reverse');
    nav_item_5.removeClass('slide-in-nav-item-delay-4').addClass('slide-in-nav-item-delay-4-reverse');
  }
})


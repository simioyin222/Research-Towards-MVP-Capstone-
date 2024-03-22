# Research-Towards-MVP-Capstone-
## Notes and Progress Towards Capstone Notes Will Incorporate By completion of part
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

## Prototyping tools 5:36 pm cst - 

-

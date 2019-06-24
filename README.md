# Teaching tips and tricks
The main goal is to inspire other teachers and share information about how to give a fun class.

## Contents:
- General Teaching Techniques
    - [Live Coding](#live-coding)
    - [Let students create the schedule of the day](#let-students-create-the-schedule-of-the-day)
    - [Give broken applications](#give-them-broken-applications)
    - [Other Teaching Tools](#other-teaching-tools)
- Energizers:
    + [Unique game](#any-module---energizer-unique-game-can-be-used-as-intro-getting-to-know-each-other)
    + [One lie two truths](#any-module---energizer-one-lie-two-truths-can-be-used-as-intro-getting-to-know-each-other)
- Module specific tips:
    + [CLI - Game: I go on holiday and I take with me](#cli---game-i-go-on-holiday-and-i-take-with-me)
    + [GIT - OS concepts and Live coding](#git---os-concepts-and-live-coding)
    + [Javascript array remembering trick](#javascript-array-remembering-trick)
    + [JavaScript: `map` `filter` `=>`](#javascript-map-filter-)
    + [Javascript callstack and eventloop visualisation](#javascript-callstack-and-eventloop-visualisation)
    + [Javascript apis](#javascript-apis)
    + [JavaScript OOP: build a IMDB web scraper with real time code collaboration](#javascript-oop-build-a-imdb-web-scraper-with-real-time-code-collaboration)
    + [Javascript Promises: Learn how to use promises by cooking pasta 🍝](#javascript-promises-learn-how-to-use-promises-by-cooking-pasta)
    + [RobotApp](#robotapp)
    + [React - drawing components](#react---drawing-components)

# General Teaching Techniques

## Live Coding

by [@ChrisOwen101](https://github.com/ChrisOwen101)

A preferred teaching technique is Live coding and it involves walking through each line of code and physically writing each line to show how the code is written.

Particularly good for new students as it’s good to see in practice how the code is written and it takes away some of the "Code Scare" effect when writing code for the first time.

This is really good when you involve the students in the process by acting as the “hands” and they are the “brain” telling you what to type. This reduces syntax errors when you want to move quickly and cover broad concepts in the lessons.

#### Additional note 

by [@mkruijt](https://github.com/mkruijt)

Just like Chris I use a lot of live coding in my classes.
I would try and keep this around 15-20 minutes and follow it up by actual coding.
- You can ask students to implement the code you have written while live coding, in teams of two.
- You can also do one of the below mentioned assignments like a presentation or the research exercises.

I repeat the combination of live coding and practical coding throughout the entire class. 

During the practical coding exercises I walk through the class. When students ask me questions I almost never give them the correct answer, I ask them a question back if they can explain to me what they are trying to solve. And let them google and find the answer themselves.

During live coding I try and involve them in the code we are working on.
- You can do this by asking students to explain certain concepts or parts of the code.
- I also ask students to tell me exactly what to type. For example in HTML/CSS "what if I would like to have a list in my page, how would I do this?" I always follow exactly what they tell me, even if it is incorrect, I like that the rest of the class gets the opportunity to correct possible mistakes.

> In general when live coding I (sometimes) on purpose make mistakes, I think it is a nice way to keep the group sharp. Also It's just really cool if you can correct your teacher right?!

#### Let students create the schedule of the day

by [@mkruijt](https://github.com/mkruijt)

In JavaScript but also in other modules in general, sometimes it makes more sense to spend time on concepts that are unclear then simply just continue with other topics that are on the agenda.

I like to include the group in what needs to be discussed on a given teaching day. This mostly results into covering some unclear concepts from previous weeks, but the class often also writes down topics of the current week.

An exercises I sometimes start my class with:

- Write down for yourself in 1 minute: What did you learn this week?
  + Share with the group what you learned this week
- Write down for yourself in 3 minutes: three questions you have from last week.
- Write down for yourself in 3 minutes: three things, what would like to learn this week?

Give them 10 min to write down what it is they would like to discuss in class today on a board, they have to do it together as a group.

Give them one more chance, they get five more minutes to decide together which three topics they want to be discussed today. They also have to get out the duplicates from the board and prioritize on importance.

## Give them broken applications

by [@KevinTss](https://github.com/KevinTss)

A good approach to make students more able to get programming concept is to let them have problems, be stuck and have to look for solution on internet. Like just let them search and find a way to repair something.

When I'm talking about `app` I'm talking about exercice, could be pure HTML, CSS, JavaScript or more...

Good example of exercices :

- Give a app with synthax errors (coma missing, case mistakes,...)
  ``` javascript
  // Synthax error (very simple)
  /* 1 */
  const firstname = "John";
  const lastname = Doe";

  /* 2 */
  const sayWelcome = function {
    console.log("Welcome guys!");
  }
  ```
  Don't hesitate to give lot of exercice like that, because it's simple, students will be proud of themselves.  

- Give little script with logical errors (like mathematics, algorithme mistakes,...)
  ``` javascript
  // Logical error (synthax validation or converstion needed)
  const age = prompt("Enter you age");
  if ((age * 2) > 36) {
    console.log("Enjoy the website!");
  } else {
    alert("Sorry buddy, you're a bit young!");
  }
  ```

## Other Teaching Tools

### Presentations 

by [@ChrisOwen101](https://github.com/ChrisOwen101)

Often it is nice to have an outline of your lesson in a presentation as it gives the lesson some format. It’s usually best to not rely on it to much though and to use lots of different teaching methods!

### Research Exercises

by [@ChrisOwen101](https://github.com/ChrisOwen101)

Give the students a topic they should research in teams for 10-15 minutes. When the students have completed the research topic they report their findings to the class and share what they have learnt.

### Videos

by [@PGorvitzSH](https://github.com/PGorvitzSH)

Videos are good to break up the lesson and to refocus the students. Never use a video that is longer than five minutes long and try to avoid ones that are just somebody talking over code, you can do that yourself!

It's often good to turn on subtitles in the videos so that students can match up the spelling of words to the pronunciation which can be good for non-native English speakers.

### Collaborative Coding

by [@PGorvitzSH](https://github.com/PGorvitzSH)

Using a website such as [SyncFiddle](www.syncfiddle.com) to have the students work together on a piece of work can be a fun way to break down the barrier between student and teacher. Simply set up a shared workspace on the SyncFiddle website and then send the students to it on Slack. From here you can all work collaboratively on a single piece of code. 

### CodePen Tasks 

By [@kostasx](https://github.com/kostasx) and [@KPouianou](https://github.com/KPouianou)

Constructing a small task on CodePen and distributing to the students to complete during the lesson can be a good way to reinforce what the students have just learnt in a lecture.

See an example for While and For loops here: [CodePen Exercise](https://codepen.io/KPouianou/pen/VQLaVo?editors=0010)

# Energizers:
> the goal of energizers is to have a small break while seeing similarities between students. And have a quick laugh.

## Any module - Energizer: Unique game (can be used as intro 'getting to know each other')
*By [@daanaerts](https://github.com/daanaerts)* 

Everybody stands up, has to tell something about himself that is unique, if someone else in the group has the same unique thing the person who said it needs to sit down and does not participate in the game any more. The game is that whoever stands up last wins the game. To make the games shorter you can let the sitting down students still "participate" if they have something in common with one of the students that are still in the game they can still kick someone out of the game.

## Any module - Energizer: One lie two truths (can be used as intro 'getting to know each other')
*By [@M3kH](https://github.com/M3kH)* 

Everyone stands up. Everyone tells three things about him or herself. Two out of three have to be true, one is a lie. The group has to guess which one of the three is a lie.


# Module specific tips:
> These tips can of course be used in multiple modules, they are more about different ways you can interact with your class and make your students involved and participate. 

## CLI - Game: I go on holiday and I take with me
*By [@unmeshvrije](https://github.com/unmeshvrije)*

_"I go on holiday and I take with me"_ with CLI commands from the week before:

- They have to repeat the commands said before them.
- Add a new command and explain what it does.
- Let the round continue twice otherwise the students that went first don't have to repeat all the commands.

E.g., first student says _"ls : lists commands"_. Second student must say _"ls and cd: change directory"_. Then third student must say _"ls, cd and pwd : show present working directory"_ and so on.

## GIT - OS concepts and Live coding
*By [@unmeshvrije](https://github.com/unmeshvrije)*

* The teacher should explain the file system if they have no idea about it.
* Students often get warning about new lines (CR and LF characters) because they create UNIX-like files on their Windows machines. In this case, teacher should explain the different between interpretation of new lines in UNIX and Windows.
* To keep the students' attention, create files with funny names and ask students for the contents of files and commit messages.
* For lesson 1, every student along with the teacher, creates a repository **MyFirst** in his/her GitHub accounts.
  Together, they create an SSH key, configure email and username.
  It is important to make sure **at every step** that no student is lagging behind. It is easy to lose motivation for a student who is lagging behind the class.
* For lesson 2, following online tool is very helpful: http://git-school.github.io/visualizing-git/
* For lesson 3, students often clone the repository of teacher. Teachers should stress that they should clone the repository which they forked.

## Javascript array remembering trick
*By [@benna100](https://github.com/benna100)* 

Pop, push, unshift and shift which does what. Well the longest of the word pairs (pop, push) (shift, unshift) makes the array longer, really easy to remember that way.

## JavaScript: `map` `filter` `=>`
*By [@joostlubach](https://github.com/joostlubach)* 

All students write a little JSON-object for themselves. for example:

```js
{
  "name": "Joost",
  "age": 34,             // Hierover mochten ze liegen :-)
  "livedIn": [
    {
      "country": "The Netherlands",
      "town": "Groningen"
    },
    {
      "country": "The Netherlands",
      "town": "Delft"
    },
    {
      "country": "Canada",
      "town": "Montreal"
    }
  ]
}
```

## Javascript callstack and eventloop visualisation
*By [@benna100](https://github.com/benna100)* 

[http://latentflip.com/loupe/](http://latentflip.com/loupe/) is the perfect tool for visualizing the call stack and event loop. You can as of right now only write es5 javascript, but apart from that there is no limit. 

you can build a small webapp. where they can send in the JSON. you can download all objects as an array. and than you can procces the array with `map`and `filter`. First you can filter out the invalid input, for example people who have put their age in a string, or people who have only filled in one town.

## Javascript apis
*By [@benna100](https://github.com/benna100)* 

We have had some fun using these apis:
* The giphy api: [https://developers.giphy.com/docs/#operation--gifs-search-get](https://developers.giphy.com/docs/#operation--gifs-search-get)
* How many people are in space: http://open-notify.org/Open-Notify-API/People-In-Space/
* Space X launches: https://api.spacexdata.com/v2/launches

## JavaScript OOP: build a IMDB web scraper with real time code collaboration
*By [@M3kH](https://github.com/M3kH)* 

Start of by letting them all install Atom so they can have live screen sharing and editing. make sure everyone has atom [pair installed](https://atom.io/packages/atom-pair)

The teacher can start of with live coding and explanation. In the second part of the day we ask students to participate in pairs. They form a team, one is the driver and the other students tells him what to code. The idea is that they add a piece of functionality to the code made in the first half of the class. All of this is of course shown live on the screen in front of the class.

for example:
```js
class Actor{
  constructor(name = ''){

  }
}
```

```js
class Movie{
  constructor(title ='', actors =[]){
  this.title = title
  this.actors = actors
  this.finish = false
  this.startDate = new Date()

  }
  addActor(actor){
    if (actor instanceof Actor){
      return this.actors.push(actor)
    }
  }
}

const Ocean11 = new Movie('Ocean11', [Clooney])
```

## Javascript Promises: Learn how to use promises by cooking pasta
*By [@razpudding](https://github.com/Razpudding)*

> Async can be hard to understand without real live example. Cooking is a great example of mixed synchronous and asynchronous tasks. In this assignment we'll cook pasta with promises 💍

Let's say we want a programme to cook some pasta. Some of the steps involved in cooking pasta are:
1. Gathering the ingredients (pasta, garlic, tomatoes, sage, butter)
2. Cutting the garlic
3. Cutting the tomatoes
4. Cooking the water
5. Cooking the pasta
6. Baking the garlic
7. Baking the tomatoes
X. Mixing the pasta with sauce

If we do this synchronolously there is no chance of it becoming a good meal because the pasta would be cold by the time the vegetables are ready. It would also take way too long this way. So let's fix that!
1. Think about how to do this asynchronously; which tasks could be run at the same time? What steps should wait for what other steps? Try to write down a basic recipe (don't write any code yet!)
2. Now convert your recipe to pseudocode (in markdown). The point is to name functions and show which functions call which other functions. The logic should be there but we'll write the code in the next step.
3. Write the actual code using promises. Add timeouts to each task (estimate how many minutes a task would take and then set the timeout to that many seconds so 8 minutes for cooking pasta would be 8 seconds in your programme)
4. Can you get the code to work like you would cook pasta in the kitchen? Try using Promise.all if you want to wait for several tasks to finish.

<!--- Here is my own attempt at completing the exercise. It's actually pretty tough to get the whole thing working with promises so maybe see how far students can get. https://codepen.io/Razpudding/pen/Keygge --->

> Async await really helps simplify asynchronous (promisified) code. The previous example can be improved by applying it.

5. Try rewriting your previous attempt using Async/Await. ⏰🍝⏰

<!--- Here is my solution. It's a lot cleaner than the promises version but could still use some work. Would also be nice if the changes were reflected in the DOM. https://codepen.io/Razpudding/pen/RJZeJO --->

## RobotApp

*By [@remarcmij](https://github.com/remarcmij)*

The project in [RobotApp repository](https://github.com/HackYourFuture/RobotApp) (mirror at: http://roverjs.taalmap.nl/) was inspired by the [RoverJS](http://roverjs.com/) app developed by @joostlubach.

The objective of the project is to write a (plain vanilla) JavaScript single page application that rebuilds the RoverJS game board and adds ways to direct the robot towards the flag, using buttons or commands rather than through user-provided JavaScript functions. This is done step-wise through eight different, progressively more advanced versions of the application.

This project was originally intended for use throughout the JavaScript 1, 2 and 3 modules but soon proved to be far too ambitious, as it attempts to introduce ES6 Classes, the MVC pattern and the Observer pattern in the more advanced versions of the application. Still, the repo may be of interest to JavaScript 3 students who have played with the real RoverJS game and want to know more about how some of its aspects could be implemented.

## React - drawing components
*By [@joostlubach](https://github.com/joostlubach) and [@spirosikmd](https://github.com/spirosikmd)* 

Draw a sketch of the final app on the flipover, and then students took turns in taking a colour pen drawing boxes around what they considered a component. When we were done with that, we draw a component tree hierarchy. This helped a lot when explaining the input (props) and output (prop handlers) of each component with arrows. Also helped a lot with explaining the data flow between components. What we found handy is that one of us was working with the computer, writing code, explaining the concepts by building an example app, while the other was drawing on the flipover explaining mostly the design decisions we made during the class.

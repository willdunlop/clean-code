# Clean Code - Chapter 1: Clean Code

## Attitude

**Why does good code so quickly rot away into bad code?**

According to a bad developer
- Complain that schedules were too tight
- Complain about managers or customers/users

According to a good developer
- We are managing ourselves poorly

**How could it be the developers fault**
- Managers look to us for information so that they can make their own promises
- Even if they don't look to us, we shouldn't be shy about what we think
- They look to us to work out the schedule
- The users look to us to validate their requirements within the system
- We are deeply complicit in the planning of a project
- We therefore share the responsibility for planning failures
- A developer is not a manager yes man, they are a manager informer
- Informing the manager with what they need in order to manage
- Its a managers job to defend the schedule, yes
- Its your job to defend the code


## Art of clean code

*It's no good trying to write clean code if you don't know what it means for code to be clean*

- Writing clean code takes practice
- We may know clean code when we see it, but that doesnt mean we know how to write it
- Writing clean code requires discipline to develop
- The developer needs a sense of "cleanliness" and a "code-sense"
- A sense that not only identifies bad or good code
- But also provides us with the ability to develop a strategy for cleaning up code
- With out this code-sense, you will be able to identify bad code, but not know how to clean it
- Developing this ability takes time and is an art form

## What is clean code?

**Bjarne Stroustrup, inventor of C++ and author of The C++ Programming Language**


*"I like my code to be elegant and efficient. The logic should be straightforward to make it hard for bugs to hide, the dependencies minimal to ease maintenance, error handling complete according to an articulated strategy, and performance close to optimal so as not to tempt people to make the code messy with unprincipled optimisations. Clean code does one thing well."*

    
- Clean code should be *pleasing* to read
- Reading it should make you smile and admire the craftsmanship
- The use of the work "tempt" in Stroustrups quote is important
- Bad code will tempt developers to continue the cycle
- Why waste time being elegant in such an inelegant place?
    - "A building with broken windows looks nobody cares about the place"
    - "So other people stop caring"
- Clean code exhibits a close attention to detail
- Clean code is also focused. "It does one thing"
- Each function, class, module exposes a single-minded attitude.
- They remain entirely undistracted and unpolluted by the surrounding details


**Grady Booch, author of Object Oriented Analysis and Design with Applications**

*"Clean code is simple and direct. Clean code reads like well written prose. Clean code never obscures the designers intent but rather is full of crisp abstractions and straightforward lines of control"*

- Just like when reading a novel, reading clean code should encourage your imagination to see the application process in your mind
- It should expose the tensions in the problem being solved
- As you read it, it should build those tensions to a climax and give the read an "AHA" moment.
- Clean code should be "matter of fact" rather than speculative.
- It should contain only what is necessary.


**"Big" Dave Thomas, founder of OTI, godfather of the eclipse strategy**

*"Clean code can be read, and enhanced by a developer other than its original author. It has unit and acceptance tests. It has meaningful names. It provides one way rather than many ways for doing one thing. It has minimal dependencies, which are explicitly defined, and provides a clear and minimal API. Code should be literate since depending on the language, not all necessary information can be expressed clearly in code alone"*

- Clean code makes it easy for other people to enhance it
- There is a difference between code that is easy to read, and code that is easy to change
- Tests, do them, write them, its not clean if there are no tests
- Minimal. Smaller is better
- Code should be composes in such a way that makes it readable by humans


**Michael Feathers, author of Working Effectively with Legacy Code**

*"I could list all of the qualities that I notice in clean code, but there is one overarching quality that leads to all of them. Clean code always looks like it was written by someone who cares.  There is nothing obvious that you can do to make it better: All of those things were thought about by the codes author, and if you try to imagine improvements, you're led back to where you are, sitting in appreciation of the code someone left for you--code left by someone who cares deeply about the craft."*

- Care, its always about caring
- Clean code is code that has been taken care of
- With appropriate attention to detail


**Ron Jefferies, author of Extreme Programming Installed and Extreme Programming Adventures C#**

*quote is way to big to write here*

- Simple code should:
    - Run all tests and pass
    - Contains no duplication
    - Expresses all the design ideas that are in the system
    - Minimises the number of entities (classes, methods, functions and the like)
- If there is a lot of duplication it signifies there is an idea in our mind(s) that is not represented in the code
- Use meaningful naming
- Single minded functions, only do one thing
    - Extract Method refactoring
    - Parent method states what it does
    - Child methods explain how it is done


**Ward Cunningham, inventor of Wiki, inventor of Fit, co-inventor of eXtreme Programming. Motive force behind Design Patterns.... The godfather of all those who care about code.**

*"You know you are working on clean code when each routine you read turns out to be pretty much what you expected. You can call it beautiful code when the code makers it look like the language was made for the problem"*

- When reading clean code, you shouldn't be suprised
- The code should solve the problem in a way that you would expect.
- It should make it look like the problem being solved was solved easily (even when it wasnt)
- It will be obvious, simple, and compelling
- Good code makes the language being used look simple


## Schools of Thought

In  summary, this book will teach you AN approach to clean code. The code will be clean. You will become a better programmer. It is just important to know there are other profesionals who have other approaches, all of which can be valid. Don't be scared to widen your horizons and see what they have to say on the matter as well.


## We Are Authors

- A programmer is an author. An author has readers. Make sure your readers enjoy what you write
- Even when actively developing software, most of the time is spent reading the code than is spent actually writing it
- You can only write in the context of everything else in the codebase
- This includes code that YOU have written previously
- If you want to go fast, and you want what your currently writing to be good code, then make sure all your code is good code


## Leave it cleaner

- Its not enough to just write the code well, the code has to be kept clean over time
- We must take an active role in avoiding code degredation
- *"Leave the campground cleaner than you found it"*
- The code will not rot if we "checked-in" our code a little cleaner than when we checked it out
- Cleanup doesnt have to be major, your just going through and doing a bit of editing
    - Rename a variable better
    - Split up a function into multiple
    - Eliminate a small piece of duplication


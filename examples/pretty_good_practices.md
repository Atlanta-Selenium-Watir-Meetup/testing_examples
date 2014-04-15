Some "Pretty Good" Practices
================

## Don't use Xpath :{
no really please please stop it. It's brittle and I am willing to bet there are easier ways.
Examples:
* https://groups.google.com/d/msg/selenium-users/eEHcbpudQMg/a2uxllyN0YoJ
* https://groups.google.com/d/msg/selenium-users/on5SrGj8Fho/yReD0BhNa-MJ

### The Answer
* The easiest way is id's they are unique(as per w3c spec they should be!), they are currently the fastest way to locate an item, css is the second.  
* Talk to your team, ask them to make the app testable, ask them if you can update your app to add id's 
* clone their repo and update the app yourself.(I tend to do this as a first step)

##Page Objects Tips
* make your framework return the web element object you want
    * cuts down on code duplication
    * makes it easier to manage your assertions in the test
* dont do assertions in your framework
    * let the framework do the heavy lifting and do your assertions in your tests

##Learn your Language and tools
most problems can be solved by having a basic understanding of the language of you
### The Answer
Selenium is for browser testing that answers most questions, there is a [Selenium Wiki](https://code.google.com/p/selenium/w/list) with a lot of answers no one ever rear choice to use your tools. Like, can selenium test [flash](https://groups.google.com/forum/#!searchin/selenium-users/flash), [flex](https://groups.google.com/forum/#!searchin/selenium-users/flex), [silverlight](https://groups.google.com/forum/#!searchin/selenium-users/silverlight), and [swing](https://groups.google.com/forum/#!searchin/selenium-users/can$20selenium$20test$20swing). 
ds. 
Dont really know the language you need to test in? then become a [Programming Motherfucker](http://programming-motherfucker.com/), No seriously probably the best collection of programming tutorials out there


##Just getting started with Testing and want to learn how to use WebDriver and write tests?
do you know what language you want to use? 
  
* yes? is it ruby? no? pick ruby
* no? pick ruby

Hands down ruby is in my opinion the best language to write tests. I say this because testing is important to the ruby community, so much in fact they have some of the best testing tools around that have been tried to be duplicated in other languages

* Rspec:  hands down my favorite testing framework
* FactoryGirl:  use your database models to create test data!
* Faker: You will need to fill your factory with some fake data, no problem 
* Cucumber: Want to get your whole team speaking the same language, really no better collaboration tool
* Taza:  Need to test a web app :D Very opinionated framework for just that!(yeah I know i know) 

These are just my favorites, there tons more out there really just depends on what you like

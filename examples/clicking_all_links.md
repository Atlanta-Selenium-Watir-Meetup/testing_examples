Clicking on all links 
================

### The Bad
its a pretty common question asked on different user groups like [Selenium](https://groups.google.com/forum/#!searchin/selenium-users/click$20on$20all$20links%7Csort:relevance%7Cspell:true) and [Watir](https://groups.google.com/forum/#!searchin/watir-general/click$20all$20links%7Csort:relevance%7Cspell:true) user groups. while they all have different reasons to why they want to do it. It's just a bad idea. the reason why is simple clicking on each link really gives you no value. 
    
    So lets say you have 10 links on a page you click them now what? What do you actually validate? that the page loads? hmm, 
    *  The page can load but not have the right info on it
    *  it could 500, and that is a valid page load.
    maybe you get past that by checking the header of a section! on that page now we will know for sure that it loaded the right page. 
    
The problem now is that we just made our test really complex for no reason

``` 
  open a page
  collect all links
    click on link in collection
      valditate the header on that page
      go back to the original page
    repeat
```

### The Answer
Don't do it. I am going to guess that each link takes you to a page that has some functionality. I will guess again that you will have to write at the least 1 test for that functionality. so no need to write this test at all really. because if you click on a link and try to do something on that page and your test fails because the page didn't load, or it took you to the wrong place, or even it allows you to do whatever it is on that page and your test passes. you know that the link is doing its job.

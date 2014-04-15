Testing the right thing 
================

### The Bad
There was once a case where we changed versions of jquery. and changed all of our forms from using radio buttons to checkboxes submitted was a set of scenarios that kind of looked like this

    When I check thing blah
    Then foo should not be checked
    Then bar should not be checked
    Then baz should not be checked
    
The problem with this is that its implementation language and its also testing actual browser behavior, and jquery behavior which if it really needs to be tested I think would fall into a javascript unit test. (but that would be testing how jquery actually works so im not sold on that idea either.)

Chris Simon
@ChrisSimonAu
@ChrisSimonAu@hachyderm.io
devcycles.io

- "There's no physics to TDD" there's no iron clad principle to stick to
- Co-location of a domain concept (consider)
	- IE "Student" controllers, classes DTOs etc all under one folder
- concurrency test example.(lu)
	- Utlises  an integrationo style test
- Removing functionality
	- red, green, refactor. 
	- remove code first, check the tests you are expecting to fail fail. 
	- Then remove the tests. 
	- ^^ Argument for granular tests. Easier to remove things later on. 
- Simple project, use simple language and encapsulate the rules inside domain classes
vs cocd extension "contextive" - Provides definitions of terms where used in the code. (Try this [[Todos (Backlinked)]])


A very good talk. When the videos for this one come out, I'd absolutely recommend that others watch it.
The talk centred around implementing an unconsidered/undiscussed domain model relating to enrolling students onto a course at a school. I really enjoyed how Chris demonstrated TDD in this flow and enjoyed a re-presentation of the importance of red/green/refactor over fail/pass/refactor. 

Something I don't often get the opportunity to do is delete unused code. Chris pointed out that the red/green/refactor would indicate that the code should be edited first and the feature expectation updated second. 

Another  ah-hah moment. Was when we arrived at a point where we were working with data that was served across different transactions and was liable to throw errors in the production system. Asking the audience what could be done about this, the answer given was to implement the design under an aggregate. 

To my surprise, we wound up going in a different direction. It was pointed out that this transactional inconsistency probably doesn't exist in the real world and perhaps we should go challenge that. 

Turns out this was the plot-twist moment where by not talking about the domain model our assumptions had turned out wrong. - I enjoyed this, not quite an anti-ddd talk, but showed which domain concepts and hueristics really mattered in the given scenario. Lots to think about in this one. 

Another thing to try out of this one was the speakers vs code extension where the engineer can define terms that can appear as tooltips. 

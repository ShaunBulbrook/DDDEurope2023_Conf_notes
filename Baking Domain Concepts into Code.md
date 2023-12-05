Paul Rayner



- Eventstorming (lu)
	- Business process mapping
- Refactoring data into a value object (T&Cs)
	- Illustrating "Keeping tests green" over the refactoring duration using new constructors to keep things changing by extension
		- Similar but not  the same as what dolphins did with the model refactor on tfs
		- >> Is it possible to nominate a different constructor on a class in TS/csharp?  
	- Testing on value objects is simplified 
		- Is there value in testing these where  you can read them from the entities that manage them?
- When a domain event is fulfulled an event should be fired. 
	- We've been managing these events through a broker. 
	- should those domain event classes mangage the publish? 
		- Alternatively, should they  be managed in a repository.

Great intro to the conference. The talk centered around refactoring code into a domain driven design. It was really lovely to see some alternate approaches to TDD in the way that Paul worked through this problem. "Keeping tests green" was a great example of this. When extending the behaviour of a class, we stepped through the process using an alternate constructor method which allowed the new behaviour to be added without affecting the existing tests in the system.  

When the code was ready to replace, the references were updated and the redundant older method was removed. Recently we adopted a similar approach with an endpoint -- the end goal to merge code sooner as opposed to and breaking the whole test spec and hacking at the job  until done. (Same principle applied in a higher level of design). 

I consider now if we might be able to continuously merge code by using this approach.
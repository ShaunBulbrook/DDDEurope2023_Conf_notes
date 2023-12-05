Yves Lorphelin

- Initial assessment of the codebase
	- Is it realistic for developers to ask as many questions. (requisite experience?)
- Breaking out the new design
	- Surely, this would work better in UML/other kind of diagramming? - Doing this in the code seems counterproductive. 
		- Very difficult to conceptualise the design. 
- When "recovering" from legacy, the demonstrated pattern appears to be
	- Produce a desirable domain model that can be implemented in the code. 
	- Start at the infrastructure and assess what is being saved. Then at what is being read to see what the code is actually doing. 


The premise of this talk was easy enough to get, we were looking at a horror show of a codebase and trying to recover it from a legacy state. 

Yves took us through a journey in the code and began sketching out questions in a notepad file demanding answers as to what random variable names were and what certain concepts were as he followed through. This "audit" felt sadly familiar. 

One key thing stood out as the speaker sought clarity in this mess. He pointed out that we could start by looking at what data was being persisted and start working backwards from there to start breaking out the domain modal. 

After this a new file was made and domain objects started to get created inside of it. Nothing really in the way of implementation to start with, just types and relationships. With a limited knowledge of the domain, I found this quite hard to follow and questioned at the time, the usefulness of writing up these types. Surely diagrams would be more clarifying?

Talks later in the day would have me revise my opinion on this. Defining the domain this way might be quite practical. 

Also worth noting that there was an assumption running through this that because this production code hadn't gotten something wrong for a long period of time, that it was in fact working as desired.
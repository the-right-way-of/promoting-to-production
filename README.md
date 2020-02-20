# promoting-to-production
How to work with artifact promotion,tagging CI vs CD

### Draw the line

CI is not equal to CD.
Tools that claim you can do both CI and CD have been lying to you all along.

### Do you really want me to push the code?

Countless hours have been wasted to retrofit this model when it comes to testing.
Because of this question GitFlow (TM) has been introduced which is another piece of crap on an already rotten cake.

### Would you want to test your software on the CI?

I can't push the artifact before testing but its okay to push the code, really?

#### Developers are not fortune tellers

How can you expect people to push Production Ready (TM?) code everytime?
Its like writing a cheque to someone without knowing the amount.
Artifacts and source code are like cash and book-keeping

#### Artifact promotion as a step

Same artifact should be moved between production and non-production repositories.
CI is not the only decision maker for pushing artifact to production. 
Promotion and CD can be linked, but linking CI to promotion has seen problems, especially with new team members.
Its not safe if all production artifacts are stored in the same repository as non-production ones, one can accidentally deploy an untested artifact to production.

# Storing Passwords Quiz
## Would you like salt with your hash?


With your partner, in words both of you will understand 6 months from now, answer the following questions.

> A customer hires you to consult on a web app.  You notice that they are storing their passwords in plaintext.  What advice would you give the customer.  This advice should outline the risks of the current solution, and give a list of best practices for a new solution.

Dear Customer,

Plaintext passwords are dangerous: if hacked, all is lost and it will be your fault. Instead you should use a good hashing algorithm to encode your sensitive data. In addition, throw some salt on that by assigning another random string on the server-side before hashing. Finally, you may not want to use email address as user-id, because email = id is really common and weak so hackers can easily steal a whole identity.

Thanks,
Tucker & Shannon

p.s. don't use any MD5 encryption - it is completely compromised

p.p.s. SPF 15 or higher sunscreen has been shown to help prevent certain melanomas; we like you and want to ensure you are a valued collaborator for years to come - enjoy the summer!

> You are tasked for creating a RFP (request for proposal) for a new cryptographic hashing algorithm.  What requirements would you put in place for this new algorithm.

A good hashing algorithm (hash-algo to those in the know) uses one-way encryption, outputs cyphered text that is always the same length (regardless of input length), does not repeat hashes (given different inputs - no collisions), small changes have a dramatic effect on hash output (avalanche) and should be relatively slow (like 500ms) to help prevent brute-force attacks.

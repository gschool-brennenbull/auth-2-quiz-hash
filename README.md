# Storing Passwords Quiz
## Would you like salt with your hash?


With your partner, in words both of you will understand 6 months from now, answer the following questions.

> A customer hires you to consult on a web app.  You notice that they are storing their passwords in plaintext.  What advice would you give the customer.  This advice should outline the risks of the current solution, and give a list of best practices for a new solution.

How you are currently storing your passwords is the most insecure because if someone gets access to your database there is no protection for your users and you risk compromising their online security. To fix this I would recommend salting all passwords, then hashing the resulting string then only storing the hash and salt.

> You are tasked for creating a RFP (request for proposal) for a new cryptographic hashing algorithm.  What requirements would you put in place for this new algorithm.

-All resulting hash should be the same length regardless of password length.
-Minor password changes should result in major hash changes(avalanche).
-Ability to slow down the hashing algorithm
-No length requirements for password input.

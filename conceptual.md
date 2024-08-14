### Conceptual Exercise

Answer the following questions below:

- What is a JWT?

A JWT token or JSON Web Token is an open standard for securely transferring data within parties using a json object.
It is used to securely transfer infoprmation to the web(between two parties).


- What is the signature portion of the JWT?  What does it do?

It is a cryptographic signature that verfies the token's integrity and ensures the message hasn't been changed in transit.


- If a JWT is intercepted, can the attacker see what's inside the payload?

Yes, if the jwt token is intercepted, a attacker can see whats inside the payload because the are typically encoded using
Base64Uri encoding, which is not an encryption. This means it can be decodedand viewed.


- How can you implement authentication with a JWT?  Describe how it works at a high level.

First make request with username/password to AJAX login route. Server authenticates & returns token in JSON. Token is encoded & signed with open standard, “JSON Web Token”. Front-end JavaScript receives token & stores in localStorage. For every future request, browser sends token in request. Server gets token from request & validates token.


- Compare and contrast unit, integration and end-to-end tests.

Unit intergration and end-to-end testing are both software testing units. Intergration testing is faster and less complex than end-to-end testing. However, end-to-end testing can help identify defects that intergration testing might miss. Intergration test focus on how individual componenets or modules of a application. End-to-end evaluate the entire application from the users prespective, stimulating real user scenarios.


- What is a mock? What are some things you would mock?

A mock is a fake or stimulated component that mimics the behavior of a real component in a system.
You can mock AJAX requests, reading/writing to files, and impure functions.


- What is continuous integration?

It is the practice of automatically and frequently intergrating code changes into a shared source code repository.


- What is an environment variable and what are they used for?
It a user-definable value that can affect the way running processes will behave on a computer. Ex. ENV_VAR = "test" would make an application run in test mode.


- What is TDD? What are some benefits and drawbacks?

Test-Driven Development is a methodology in software development that focuses on an iterative development cycle where the emphasis is placed on writing test cases before the actual feature or function is written. TDD is more thorough because it questions and strengthens the quality assurance behind each small unit of code. Whereas a drawback is that if the tests are not written correctly it can require twice the amount of debugging.

- What is the value of using JSONSchema for validation?

It is used for improved data qaulity. By enforcing data validation through JSON Schema, you can significantly improve data quality and consistency within your applications.

- What are some ways to decide which code to test?

Test areas of the software with the biggest impact on the users, Test defects based on their severity, and Test that verifies the desired functionality

- What does `RETURNING` do in SQL? When would you use it?

The RETURNING clause allows you to retrieve values of columns, that were modified by an insert, delete or update.  I will use RETURNING every time that I need data back from my query that is not a SELECT statement.


- What are some differences between Web Sockets and HTTP?

HTTP uses a request-response model and is best for static resources like web pages or standard API request. HTTP connection are stateless, meaning each request is handled individually and there's no record of previous request.

Web Sockects enable real-time, bidirectional communication between a client and a server, making them ideal for apps that need continuous data exchange or quick responses.


- Did you prefer using Flask over Express? Why or why not (there is no right
  answer here --- we want to see how you think about technology)?


  I prefer to use Express over Flask because it is a little easier tounderstand. I also love the diffrent libraries that can be added to help run the application more smoothly. 

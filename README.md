
# Hello

Thank you for sharing your take-home test, it was really fun to complete.

The solution uses TypeScript instead of plain JavaScript I really do hope that is not an issue. 

# Other dependencies

I used [axios](https://github.com/axios/axios) for making outgoing http calls. Axios is really powefull http client widely used across the web these days. 
In case you wanted me to build a http client from scratch I am more than happy to amend the solution, I just thought that would be out of scope for this assigment. 

I also used [tysiringe](https://github.com/microsoft/tsyringe) as dependency injection container as I am a big fan of SOLID principles.

# The Solution

I encapsulated the logic within a HttpClass that uses axios as a dependency, it handles the validation and parsing of responses. I did not like the idea of the all or none when one
or more calls fail. So instead I came up with the idea that failed requests also appear in the returned array of responses. That way you can you can use the successful ones and fix or inspect
the failed ones in the list. 

Example output:

![Screenshot](https://github.com/adamkosinar/ft-takehome/blob/master/exmaple.png)


# How to run

Everything is handled by the npm itself.

use `npm i` to install all dependencies.

use `npm run test` to build, lint and to run all unit tests and coverage. 

use `npm run start` to run the project. 

# An Introduction to Refactoring

### Before Refactoring
- Identify the section of code you seek to refactor. Is it a particular function?
- Do you have testing suite for the designated section of code you intend to refactor? If not, make one. You should be continously rerunning tests as you refactor.

### Decompose the Function
- Run through the code, grouping similar statements together and leaving comments preceding key behaviors (now likely code chunks) of the function. 
- Wrap these code chunks into their own functions, referred to as "Extract Function"
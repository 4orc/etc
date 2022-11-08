# Coding

## Data Independence

- Is your internal model isolated from I/O operations (e.g. in a csv file, conversations from strings to types happens once, and once only, before data is loaded into your model)?


## Dialog independence

- In your model, are their no direct writes to "print" but rather to some log function that may or may not write to the screen.
- Can you turn off all logging (no log string generation, nothing logged/printed anywhere)?


## Abstraction
- You writing your own iterators ?
- You using try:catch, try:xcetpt, pcall,

## Functional programming

- Are you using anonymous functions? (e.g. passing in your own customized sort functions)
- Are you writing function that return functions? (e.g. "lt")
- Are you writing code using `map`

## Object-oriented programming

- Are you using polymorphism?
- Are you using inheritance (consider doing less of that)?
- Do you objects have customized create function?
- Do you objects have customized sort functions?
- Do you objects have customized print functions (e.g. not showing private attributes)?

## DSLXXX
- mechanism and pikicy
- usig existing DSLs (regular expresions, build systems)
- do you write your own (docstring==> CLI)

# Packaging

## XXX sharing
- Is your code under some license that enables sharing?
- Does your project have a web site?
- Does your web site include test data, documentation, test suite results?
- Is your code routinely explored by  static code analysis tools (which can be very  simple e.g. syntastic or very complex and slow to run e.g. your model checker of choice)?
- Does your code follow standard formatting conventions?
- Does your code support short release cycles (no standard test is slow, really slow things are explored for optimization)
- Does your code have zero internal boundaries (e.g. everyone uses same tools, config files for those tools in repo)


## Test suite
- Do you have half a dozen tests per person working on the project per week of work?
- Can all the tests be run in batch?
- From the command line can you run just one test?
- If a test fails and crashes, can the rest of the tests still run (hint try:except:)

## Source control
- Is your code in some version control system?
- Everyday you write code, does some branch get updated?
- Is the test suite triggered by each new commit? 
- Do you have an automated build system (Make, Ant, Maven, Cargo, Flutter, Elm, etc etc etc) for all the tedious details.
- Is the build system included in the documentation?

## Documentation
- Do you have (at least) your public functions and classes documented?
- Can you generate doco from comments and type hints in the source code?
- Does your code follow any well-known patterns? Does the doco mention those patterns?

## Settings
- Do you have settings global?
- Can the settings be changed from the command line?
- From the command line, can you get a print of the help text?
- From the command line, you set the random number seed?

## Packages/Modules
- In your package, have you tried using fewer globals?
- Does your code pollute the global space?
- Does your package return a subset of the code in your package?


## Pipes
- Can you accept input from standard input?
- Are your errors written to standard error?
- Is your default output to standard out?

## Reuse
- Have you used your functions/objects for at least three different purposes? (e.g. NB, NN, DT all need DATA, NUM, SYM, etc)


# AI

## Simulation

- As above: Can you turn off all logging (no log string generation, nothing logged anywhere)?
- Does your code store its random number seed?
- Are your random numbers reset to the seed before each run? 





The following are suggestions on how we could implement
better development practices for large development teams.

# Craftsmanship - Large scale implementation

## Important hypothesis

1. Let us forget about SOLID. Nobody can remenber what the letters mean,
and nobody can explain the goal of the Liskov Substition in one shot.
2. Brain can only retain a few simple rules to apply when exercising.
3. In the long run, a developers will always push the same kind of code that they see in the codebase.
4. A central word document on the coding standard and pratices for a team or company is a heresy and is completely counter productive.

## The 3 items strategy

Strategy based on the hypothesis above.

### 3 coding practices only

It should require not effort to retain those 3 simple rules. **Still they have multiple hidden consequences & corrolaries**.

(For each we specify the pros and the possible cons)

* SHORT CLASSES
    * \+ Enforce naturally the Single Responsiblity Principle
    * \+ Enforces a focused and readable unit test
    * \- Smell TooManyClasses
* SHORT METHODS
    * \+ One level of abstraction principle respected
    * \+ Easier to fix a bug as dealing with only one level of abstraction
    * \+ Prevent the vertical distance for variables smell
* BEST POSSIBLE NAMES
    * \+ Readable code & fixable code as we know the originral intent
    * \+ Help to solve the TooManyClasses issue
    * \+ Best names for all artifacts: packages, projects, classes, ...

### Extending the strategy of 3 items

To better communicate & implements within the organization we can extend the idea of having only 3 items to implement for differents aspects of the development. 

#### 3 coding practices (as seen above)
* Short classes
* Short methods
* Best possible name

#### 3 XP practices
* Pair Programming
* Test Driven Development
* Continous Integration

#### 3 Eclipse plugins
* Moreunit (for conventions and easy refactoring)
* Junitflux (for rapid feedback and not keyboard touching)
* Eclemma for legacy code

## Other objectives

* Minimise static code documentation
    *  Rely on ExtractMethod and better naming to have living documentation
* Get rid of the word document that centralizes the coding standard & practices for a team
    * Language & framework evolves nobody will update the document accordingly
    * Newcomer has a bad image/feeling/start when he realises that the document on code standard is not respected in the code base
    * Living code should be the documentation: a newcomer should only look at the code to know where the quality & standard of the code lies



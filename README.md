# Template for setting up a challenge response

## Process
1. User stories / requirements / specifications
2. Break down user stories into small steps
3. Diagrams  
4. Folder and testing set up
5. Github init (if required)
6. Tests
7. Code!

*Set up sequence* (rb)
- mkdir FOLDER
- mkdir lib
- touch README.md
- touch lib/<controller>.rb
- rspec --init
- touch spec/<test_spec>.rb

## diagrams

Input/Output table
```
+-------------+--------------+---------------+
|    INPUT    |    METHOD    |     OUTPUT    |
+-------------+--------------+---------------+
|     'a'     |   .score     |        1      |
|     'aa'    |   .score     |        2      |
|    'aaa'    |   .score     |        3      |
|     'am'    |   .score     |        4      |
+-------------+--------------+---------------+
```
> Use the tests to explore the variety of what you need it to do
> EG: the length of the input and the variety of its components

Questions for IO
- What are the different input cases? (ie in range, below/above range)
- What is the simplest example of each of these cases? (ie 1 freq in each)
- Is one of these simpler than the others? (ie the one in range)

Class diagram
```
+-----------------------+         +------------------------ 
|         NAME          |         |         Shape         |
+-----------------------+         +-----------------------+
|      Attributes       |         | -length               |
+-----------------------+         +-----------------------+
|      Operations       |         | +getLength()          |
|                       |         | +setLength(n)         |
+-----------------------+         +-----------------------+
```
'-' = private, '+' = public




# Template for setting up web app with database

## Process
1. User stories 
2. Break down user stories into small steps
3. Diagrams 
4. Folder and testing set up
5. Github set up
6. Database set up
7. Tests

*File list:*
- README.md
- Gemfile
- app.rb (or another name for controller file)
- config.ru

*Folder list:*
- db
- lib
- spec (created by rspec --init)
-   /features
- views

Gems (in alphabetical order to please rubocop)

1. capybara  - for testing your 
2. rspec  - for testing your ruby code
3. pg  - lets you use SQL within ruby code
4. simplecov - show your test coverage
<!-- get an example of good simplecov setup -->
5. sinatra  - allows app to build for browser

## user stories

do they already exist? 
do you need to write them? 



Then model things in diagrams before building

*CRC Cards* to work out what's going in the *MVC model diagram* 
*Domain model diagram* to work out how the class structure will look
including methods


<!-- _Tips from Katerina:_
_Look up UML
I use class diagrams mostly
Then my own style
occasionally sequence diagrams
That’s all that I use personally _ -->


#kalbonian 
#review 
## sasha vodnik web developer
## prequizes
 - functions
 - conditional logic
 - variables


## collections
- a number of related items under a name (variable).
ads::
1. no need to many variable names in code
2. all reated is together
3. simplified syntax
### list
- simple collection of related data in some order called a list in python
- new=['ff',12,'tg'] 
- each item accessed by  an index new[0]
### dictionary
- groub data with tags called a dict in python
- dict={"bird":"d","city":"c"}
- each item indexed by a key/label
### tuple
- immutable list
- x=(1,2,32)

## other languages
- dict in python is mutable (changable data)
- dict in python key and value can be any type but in c++ must the same type
- dict may called(map,table,associative array)
## iteration
- we need data,what to do on data,when loop stop or its infinte loop.
-  how to iterate through collections in python ::
for anyname in datalist:#stops the end of collection
   print (anttime)
   - custom loop::
   - i= 0 
     while i<=5:
     print(i) 
     i+=1
## external code   
- donot reinvent the wheal
- used in tight deadlinwes because sometimes all from scratch is good
- most famouse is called module.
- module is one file has functions,variables(using import keyword)
- library or package groups moudlues (math)
- framework groubs library and in specific work flow
- you may sometimes make your framework up from libraries (cake you only put a number of years on it with custom size)
- example:
import test //test.py os in the same directory
print(tsst.mul(2,3))
- python shared pkgs ar in pypi.com
- 
![[tomove/Pasted image 20220428135138.png]]

- pytohn frameworks like django,flaskfor web
- javesc libs like (jquery,lodash)
- js frameworks lke (react,angular,vue)
- you donot need to use libs and frames right away ,use may use plain js but always see what is out it may help you

## string manipulating
- **concatinating**  in python through + sign
- string to int through int(str)/float(str) function
-  **repeat** through * sign
- str.**capitlaize(none)** to capitalize
- **.find()/.index()/.rfind()/.rindex()** 
- **str[start:end]** to slice
## regular expression
### elzero
 # -- Regular Expressions => Intro --
# ----------------------------------
# [1] Sequence of Characters That Define A Search Pattern
# [2] Regular Expression is Not In Python Its General Concept
# [3] Used In [Credit Card Validation, IP Address Validation, Email Validation]
# [4] Test RegEx "https://pythex.org/"
# [5] Characters Sheet "https://www.debuggex.com/cheatsheet/regex/python"
- ![[tomove/Pasted image 20220428142423.png]]
- ![[tomove/Pasted image 20220428143010.png]] example
- use pydoc to break down any expression to understand ,after while you can build your own
- using re moudlue
- how to do :is this sring has  5 cosequetive digits??
- ex::
five_digitexpression=re'\d{5}' //five digits//back slash avoided
print(re.search(five_digitexpression,anotherstring))---none or object to emphasize

## code style
- avoid some tools ,go with some tools,others is up to u to choose from
-  style guide::shared code style by developers
- in all languages
- impoertant to stack the same  style if a team wrie a code .
ex::
python style guide-google python style gude-py enchancement guide - pep8

## sudo code 
-  outline what you want to do in code 
- prevent you from start coding and delete code then restart  with anew structure.
## input output
- example taking data of number of cars then print a report of peak hours .
- not all invironments suppoer all i/o
## working with files for large input
```python
infile = open('values.txt', 'rt')#read
## make each line to item in alist
outfile = open('values-totaled.txt', 'wt')
print('Processing input')
sum = 0
for line in infile:
    sum += int(line)
    print(line.rstrip(), file=outfile)
print('\nTotal: ' + str(sum), file=outfile)#output to fileoutfile.close()
print('Output complete')

```
## debugging
 - syntax--not valid in language rules
 - run time --not obvious (calling an undefined functuin)
 - logic error - - not expected output  like (infinte loop  by mistake no error meesage)
 - a;; langauages have tools to debug
 - IDE:help aviding,solving bugs.
 - ide important features : auto completinn,syntax highlighting,linting(check bugs before excuting)
 - search first about the besst ide in certain laugues 
 - not always the inerpreter is a solution take it as aclue
 - sometimes you need to leave the problem ad make anoter thing then you will find it.
 - never forget tring all test cases example:test cases to check all clauses works in if ,else,elif.
 - you can also use the rupper duck approach
## OOP
-  to organize complex massive code ??to be usable .
- the project is form of objects which is made by a blueprint called class.
- each class has data/properotoes/attributes and behaviour/methods which manuplate the data.
- we can make different objects of same class (and also add methods to specific object #understand)
- remember list (pop,count) , strnig (foemat,capitalize)are classess in python that has methods
- #understand By organizing these methods by data type and making them available only to objects that need them, Python ensures that any data object I create has only the methods it needs. This avoids needlessly loading computer memory with unnecessary extra methods. At the same time, this object-oriented approach to organization allows me to easily create a new data object and immediately make use of the most common methods I need to work with that data. (using built in classes)
- class example:
```python
class Attendee:
    'Common base class for all attendees'

    def __init__(self, name, tickets):#constructer
        self.name = name
        self.tickets = tickets

    def displayAttendee(self):
        print('Name : {}, Tickets: {}'.format(self.name, self.tickets))

    def addTicket(self):
        self.tickets += 1
        print('{} tickets increased to {}'.format(self.name, self.tickets))

attendee1 = Attendee('B. Giles', 2)
attendee2 = Attendee('J. Ortega', 1)
attendee1.displayAttendee()
attendee2.displayAttendee()
attendee2.addTicket()
attendee2.addTicket()

```

## advanced topics

### memory manaagment
- you must delate data that you arenot nolonger need .
- some languages support that automaticaly using arbage collector like python ,ruby, and js
- some otherrs you shoud write code manually for managment ,especialy in highperformance games or graphics.
- search about to incras the speed and performance.
### multithreading
- to excute more than one task simultanously ,each task called a thread .
- this perfprmance affect  entire computer spped,memory allocated for program.
- you need to search about it in complex projects ,after mastering basics.
### algorithms
- the steps  to solve specific problem

# what nxt?

- choose aprogrammng langnuage
- keep practise
- connect other developers in the same language.
- learn new topics and you will y understand them bitter by practising
- build something you interested in


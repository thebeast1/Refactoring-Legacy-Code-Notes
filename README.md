# Refactoring-Legacy-Code-Notes


## first note is DRY principle vs DAMP principle:

#### DRY is Dont Repeat Your Self : less duplication and less descriptive.
#### DAMP is Descriptive and Meaningful Phrases: more descriptive but not DRY.

###### so in testing use DAMP to be more isulated and descriptive.
-----------------------------------

## Mocking API Calls or Local DB:
There is three approaches for Mocking it or Fake it:              from "Working with legacy code" book
for any of these approaches first we need to know how is our code base structure?
if the database class is using singleton first approache is:
#### Introduce Static Setter: 
###### for minimal change in your production code
 -replace the original static method of the singleton with test instance.
 -remove the final keyword.
 -change the private constructor to public.

-----------------------------------

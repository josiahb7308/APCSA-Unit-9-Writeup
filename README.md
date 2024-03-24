# Process Writeup

## Name: Josiah Benitez
## Course: Unit 9
## Period: 7
## Concept:Inheritance

### Overview
Unit 9 is about inheritance and parent and child classes in which the child class can inherit from the parent class. There are a lot of other things that come with this inheritance one of them being the permissions these classes have to call other classes which can get confusing.

## First Challenge
### Constructors causing error

In question 13 its asking the following "A Square class which extends the Rectangle class is to be written. Which of the following constructors will cause an error upon compilation when added to this class?". It also gives you a pretty lengthy block of code that you have to base your answer off of. I picked the answer with the following code:

```java
public Square(double w)
{
  super(w, w);
}
```

This code wont cause an error because super is the first line in the constructor and rectangle is accessible by the subclass square. The following answer is the correct one as it will cause an error:


```java
public Square(double w)
{
  height = w;
  width = w;
}
```

This answer causes an error because there is no super statement and it is setting height and width to w but there is no super call to take the w from the rectangle. This causes an error which makes this the correct answer.



## Second Challenge
### Hotel Shenanigans

I really liked this question but I messed up with my strategy when it came to my test-taking, I saw there was a lot of reading required so I skipped over it to go to other questions. The question wants to reader to make a program design using inheritance for a hotel. I picked the wrong answer due to a time crunch but after review I know with proper time I would've picked the correct answer. The answer I picked is the following. "Create a Suite class with the instance variables int numBeds, boolean hasBath, and int numSubrooms. Create a subclass Room of Suite which will inherit the instance variables numBeds and hasBath from Room, but not the instance variable int numSubrooms." This answer isn't the most efficient because the suite class shouldnt be the parent because there are more normal rooms than suites making rooms the default decision. 

This is the correct answer "Create a Room class with the instance variables int numBeds, and boolean hasBath. Create a subclass Suite of Room which will inherit the instance variables of Room and has an additional instance variable int numSubrooms." This answer is correct because it takes room and makes it the default as it should be, then it makes a subclass Suite because a Suite is still a room in definition. It then adds on to the room class to create an actual Suite which is more efficient. I thought this was a well designed question which shows how this knowledge can be useful in a work setting.


## Third Challenge 
### Rhombus Ridicule

Question 7 doesnt have much to break down but I thought I would just add it on because I got it wrong. The question goes as follows "Which of the following statements must be true in order for Rhombus to access a specific constructor in Polygon?" This is based off of a previous question describing a system of inheritance using shapes, polygons, and other geometry terms as examples. The main mistake I made here was forgetting that Rhombus only has access to any of Polygon's methods through quadrilateral inheriting them so Rhombus would have to ask quadrilateral to ask its mom which is polygon for her constructor. This was a simple and easily avoidable mistake that I will do my best not to make again.

### Takeaways

* Skim the long questions before you decide to skip them because you could be missing out on an easy question that you know the answer to.
* Review the beginning of the units before the test because those are normally the things least fresh in your memory so you can refresh on them.
* Put more time towards questions that require more reading of code so you are less likely to skim over important code and end up losing a chance on points you could have got.
* Make it intentional to review the rules of what can and cant happen with inheritance and how only a parents child can ask them to call a constructor directly because they inherit it.
  

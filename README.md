# java programs
# CS 480 L
1. find the median value of 3 integers

2. there are two mouses fighting, win or lose based on the number of legs, winner is normal who have 4 legs, loser's leg number less than 4    (similar as CS 480 - 3)

3. 
```
- Attributes
  + number of eyes
  + number of noses
  + number of mouths
- Member functions
  + Helping function
  + Manager functions
    * Constructor
    * Destructor
  + Implementor
    * void convertToNormal()
    * toString()
    * clone()
    * equals()
  + Access functions
    * 3 get functions
    * 3 set functions
    * Predicate
      - isNormal()
- Test your class by
  Step 1: Create 3 objects 
          f1: 2 eyes, 2 noses, 1 mouth
          f2: 2 eyes, 1 nose, 1 mouth
          f3: this object is a clone of f1
  Step 2: Display the content of f1, f2, and f3
  Step 3: Check whether f1 is equal to f2
  Step 4: Check whether f1 is equal to f3
  Step 5: Convert f1 into a normal one.
  Step 6: Display the content of f1
  Step 7: Check whether f1 is normal after the conversion.
  Step 8: Check whether f1 is equal to f2
  ```

4. create a object at beginning is looks like fObj, display the values, then change the values like fObj1 and display the values, clone fObj to create fObj1, display the values of all the attributes of fObj1, check whether fObj is equal to fObj1
```
----------------------------
| A                        |
|   String name="jack"     |
|  ----------- ----------- |
|  | B       | | F       | |
|  | int b=1 | | int f=2 | |
|  ----------- ----------- |
----------------------------
           |
           |            ---\   fObj
           |            ---/
----------------------------
| E                        |
|   int e=3                |
|    -----------------     |
|    | D             |     |
|    |   int d=4     |     |
|    -----------------     |
----------------------------


----------------------------
| A                        |
|   String name="jack"     |
|  ----------- ----------- |
|  | B       | | F       | |
|  | int b=4 | | int f=5 | |
|  ----------- ----------- |
----------------------------
           |
           |            ---\ fObj1
           |            ---/
----------------------------
| E                        |
|   int e=6                |
|    -----------------     |
|    | D             |     |
|    |   int d=7     |     |
|    -----------------     |
----------------------------
```

5. 
```
+--------------------------------------------------+
| Book                                             |
|                                                  |
|   int np; // Number of pages                     |
|   int w, h; // Width and height                  |
|                                                  |
|                                                  |
|   +-----------------------------------+          |
|   | Cover frontCover                  |          |
|   |                                   |          |
|   |   int int nl; // Number of lines  |          |
|   +-----------------------------------+          |
|                                                  |
|   +-----------------------------------+          |
|   | Cover backCover                   |          |
|   |                                   |          |
|   |   int int nl; // Number of lines  |          |
|   +-----------------------------------+          |
+--------------------------------------------------+
    
                       --------------+
                       | Error       |
                       |   int code  |
                       --------------+
                             |
                             | public
                             |
    +------------------------+------------------+-----------+
    |                        |                  |           |
    | public                 | public           | public    | public
    |                        |                  |           |
+------------------+ +-----------------+ +-----------+ +------------+
| InvalidFrontCover| | InvalidBackCover| | EmptyBook | | SquareBook |
|   int l          | |                 | |   int np  | |  int side  |
|                  | |  int l          | |           | |            |
+------------------+ +-----------------+ +-----------+ +------------+
    code:1                  code: 2           code: 3    code: 4
    
 output: 
     Book 1
         number of pages: 200
         width: 3
         height 4
         Number of lines on the front cover: 5
         Number of lines on the back cover: 6

     Book 2
         number of pages: 300
         width: 4 
         height 4
         Number of lines on the front cover: 4
         Number of lines on the back cover: 5

     Book 3
         number of pages: 435
         width: 5
         height 7
         Number of lines on the front cover: 5
         Number of lines on the back cover: 6
  ```   

6. serialization

7. similar with CS 480 - 9

8.  
```
Regular classes/*

        +-----------+
        | Table     |
        |  int legs |
        |  int sides|
        +-----------+       
              |
     +-----------------+
     | ClassRoomTable  |
     |    int shape    |
     +-----------------+       

Exception classes

                        +-----------+
                        |ErrorCode  |
                        |  int code | 
                        +-----------+
                              |
           +------------------+---------------------+
           |                  |                     |
  +-----------------+ +---------------+  +---------------------+
  | TooFewLegsError | | ZeroSideError |  | IrregularShapeError |
  |    int legs     | |               |  |                     |
  +-----------------+ +---------------+  +---------------------+
        code=1             code=2                code=3
      legs < 4          sides == 0         shape is irregular
```


# CS 480

1. create a program to find the smallest number of all the integers entered on the command line.

2. write a function that can sum the contents of an array

3. there are two mouses fighting, win or lose based on the number of legs, winner is normal who have 4 legs, loser's leg number less than 4

4. about the student ID and is student graduate or not

   isNotAStudent() : if id <= 0 
   graduate() : set the id to -1 if a student is graduated
   lostIDCard() : set the id to 0

5. Mr.Wang a rectangular cake whose width is 4 and height is 3, Mr.Lee ate half of the cake and converted the shape of the cake into a right triangle, Mr.Wang buys another cake that has the same shape and size as the old one for Mr.Lee, Mr.Lee checks whether the old cake and the new one have the same shape and size, Mr.Lee would like to find out the area and perimeter of the new cake

6. there are two ancient Chinese coin which has circular shape and a square hole in the middle of the coin, we need calculate the area of coin and does the square is large, does the circle is large, does the circle is a point, does the coin is normal

    isNormal() : A coin is normal if its diameter is longer than the diagnal of the square
    isLarge() : A circle is large if its radius is larger than 10
    isAPoint() : A circle is a point if r == 0
    isLarge() : A square is large if side is larger than 10

7. https://npu85.npu.edu/~henry/npu/classes/introjava/java_class/slide/exercises3.html (18)

8.  create a object at beginning is looks like fObj, display the values, then change the values like fObj1 and display the values, clone fObj to create fObj1, display the values of all the attributes of fObj1, check whether fObj is equal to fObj1
```
+-----------------------------------------+                       
| D                                       |
|  int d=1                                |
|  +----------------------------------+   |
|  | B                                |   |
|  |    int b=2                       |   |
|  |  +-------------+  +-----------+  |   |
|  |  | A           |  | E         |  |   |
|  |  |   int a=3   |  |   int e=4 |  |   |
|  |  +-------------+  +-----------+  |   |
|  +----------------------------------+   |
+-------------------+---------------------+
                    |
                    |
             +------+--------+
             | F             |   ----\   fObj
             |    int f=5    |   ----/
             +---------------+     
+-----------------------------------------+
| D                                       |
|  int d=1                                |
|  +----------------------------------+   |
|  | B                                |   |
|  |    int b=7                       |   |
|  |  +-------------+  +-----------+  |   |
|  |  | A           |  | E         |  |   |
|  |  |   int a=6   |  |   int e=4 |  |   |
|  |  +-------------+  +-----------+  |   |
|  +----------------------------------+   |
+-------------------+---------------------+
                    |
                    |
             +------+--------+
             | F             |     ---\     fObj1
             |    int f=5    |     ---/
             +---------------+
```
9.
```
------------------------------------------------------------------
| Menu                                                           |
|                                                                |
|     String title;   // The title of the Menu                   |
|                     // For example, "Mexican Food",            |
|                     // "Ammerican Food", "Indian Food", etc.   |
|                                                                |
| ---------------------       ---------------------              |
| |  FrontCover       |       | BackCover         |              |
| |                   |       |                   |              |
| |  String name      |       |                   |              |
| |  int numOfDishes; |       | String phoneNum   |              |
| ---------------------       ---------------------              |
| ---------------------       ---------------------              |
| |  Page             |       |  Page             |              |
| |                   |...... |                   |              |
| |  int pageNum      |       | int pageNum       |              |
| ---------------------       ---------------------              |
------------------------------------------------------------------    
                              |
                              |
                ----------------------------
                |  FancyMenu               |
                |                          |
                |   String color           |
                ----------------------------
  
  Menu printout: 
  Title: Chinese Food
Front Cover:
    name: Forbidden City
    numOfDishes: 123
Back Cover:
    phoneNum: 408-123-4356
Totoal number of pages: 3
    pageNum: 1
    pageNum: 2
    pageNum: 3
    
  Fancy Menu printout: 
 Title: Mexicon Food
Front Cover:
    name: Taco Bell
    numOfDishes: 46
Back Cover:
    phoneNum: 510-123-4567
Totoal number of pages: 4
    pageNum: 1
    pageNum: 2
    pageNum: 3
    pageNum: 4
Color: red
```

10. Visual Studio installation

11. Javadoc for a simple code

12. design the door of a car which behaves correctly when it is opened or closed
```
  +---------+
  | I_Door  |
  +----+----+
       |
 +-----+--------+  +--------+ +-----------+
 |I_LockableDoor|  |I_Alarm | | C_CarPart |
 +-----+--------+  +--+-----+ +------+----+
       |              |              |
       +--------------+--------------+
                      |
              +-------+-----+
              |  C_CarDoor  |
              +-------------+
```

13. error exception handling
```
Regular Class

        +------------------------+
        | Date                   |
        |   int m, d, y;         |
        |   int leap_year_flag;  |
        +------------------------+

Exception Classes

                       --------------+
                       | Error       |
                       |   int code  |
                       --------------+
                             |
                             | public
                             |
    +------------------------+------------------+
    |                        |                  |
    | public                 | public           | public
    |                        |                  |
+--------------+        +------------+     +------------+
| ErroYear     |        | ErrorDay   |     | ErrorMonth |
|   int y      |        |  int m     |     |   int m    |
|              |        |  int d     |     |            |
+--------------+        +----+-------+     +------------+
    code:1                   | code: 2         code: 3
                             |
               +-------------+-------------------------------+
               |public       | public          |             |
               |             |                 |             |
        +------+------+ +----+-------+  +------+------+ +----+-------+
        | Error31Days | | Error29Day |  | Error30Days | | Error28Day |
        |             | |   int y    |  |             | |   int y    |
        +-------------+ +------------+  +-------------+ +------------+
           code: 21         code: 22       code: 23       code: 24
```

14. Create 2 alarm clocks:
      One will alram 2 seconds later and generate one beep soud
      The second will alam 4 seconds later and generate two beep soud

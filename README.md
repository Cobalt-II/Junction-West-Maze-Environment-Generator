# Junction-West
An exploratory work-in-progress branching function concept. The goal of this is to explore and visually examine a branching function that goes from left-right. Class JunctionWest creates a grid with constructor(length, height). jw is a variable that can be edited in console to edit the grid. jw.branch is the branching function of the variable. Branch takes three inputs: 
```
x: x value of where the branching starts on the grid,
y: y value of where the branching starts on the grid,
shifts: a variance value that for each shift will change the y value by 1 up or down (depending on your type parameter, it can choose [-1,1], [1], [-1]), this value of this is the number of shifts that occur. More shifts = more variance.
type: the type value takes either 1, 2, or 3. Type 1 means shifts can either go up or down, type 2 means they can only go down, and type 3 means they can only go up.
```

By no means is this done, however this is merely an exploratory branching concept I've come up with, and wish to expand on. For what may I use this for? I don't know. Just thought it was an interesting concept.


![download (1)](https://user-images.githubusercontent.com/97923189/206877809-0e4af701-7f0b-4fb3-9ec0-ef602502fbd0.png)
shift values in order from top-bottom on a 100x100 grid: 1000, 10, 50, 25



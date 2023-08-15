# Junction-West
Junction West is a tool that is designed for developing maze and 2d environment generation algorithms. Class JunctionWest creates a grid with constructor(length, height). jw is a variable that can be edited in console to edit the grid. jw.branch is the branching function of the variable. Branch takes eight inputs: 
```
x: x value of where the branching starts on the grid,
y: y value of where the branching starts on the grid,
shifts: a variance value that for each shift will change the y value by 1 up or down (depending on your type parameter, it can choose [-1,1], [1], [-1]), this value of this is the number of shifts that occur. More shifts = more variance.
type: the type value takes either 1, 2, or 3. Type 1 means shifts can either go up or down, type 2 means they can only go down, and type 3 means they can only go up.
length: the duration (in tiles) of the branch.
OPTIONALS:
directPosCircs: Array of decimal values of where along the line you want certain radius() formations to form  (leave this value as a null form if you don't want any)
relativeCircs: A decimal value that when the (current position along branch) mod (relativeCircs) congruent to 0 [excluding 0, you can manually add that one yourself if wanted], creates a radius() form (leave this value as a null form if you don't want any)
dimensions: circle dimensions in a 3 length array. First entry is the minimum size, and the second is the max size. The third is unrelated but used for any specific modulo values for relativeCircs you may want to cut out.
```

![download (1)](https://user-images.githubusercontent.com/97923189/206877809-0e4af701-7f0b-4fb3-9ec0-ef602502fbd0.png)
shift values in order from top-bottom on a 100x100 grid: 1000, 10, 50, 25 (all type value 1).

There is also an erosion function, which can be used to make maze generations or environments out of branches. For example: 
![download_12 (2)](https://user-images.githubusercontent.com/97923189/206946698-d7e0eefb-6aee-47eb-bf0c-a1ed66aae201.png)
![download_13 (2)](https://user-images.githubusercontent.com/97923189/206946707-89c36032-ee29-4f85-9e80-20e81b9605e8.png)
![download (15)](https://user-images.githubusercontent.com/97923189/206946756-5e201f23-05d5-4a5a-b514-64acf041f97e.png)
![download_1](https://user-images.githubusercontent.com/97923189/213959377-131804a3-82b6-4c43-80e5-984cb365e71d.png)

There is additionally also a "radius" function, which depending on the type that you enter will fill or remove a chunk of tiles based off of how far they are away from a certain coordinate. It can be used for making maps with holes of open areas in them.



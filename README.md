# mw_mprims

This package is to store the paths for maxl primitives

# For using it 
In maxl update the following params 

`pathFolder: $(find mw_mprims)/paths/{name of the motion primitive folder}`
`pathFile: "/paths"`


# naming convention

- All the generated motion primitives are in 'paths' folder

- each mprim folder name, will two to three sets of digits, the first set of digit, will represent the value of 'dis' param, which basically the lenght of each spline/path

- the seond set of digit repesent the value of `searchRadius`, 

- to measure the searh radius, draw a circle with center at the center of rotation of robot ( during 0 radius turn) - generally between the powered wheels of the robot in differential drive. The circle should be big enough to contain the whole robot. The radius of this circle is the `searchRadius`

- the third set if mentioned, represents the divideByAngle, which basically represents the total number of groups

- the value in the names is represented in metre, and 'x' represents the decimal 


# in order to create new motion primitives visit this website 
[mprim generator](http://ec2-15-207-68-243.ap-south-1.compute.amazonaws.com/)
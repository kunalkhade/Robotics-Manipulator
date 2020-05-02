# Robotics
Robotics Programs -Forward Kinematics and Inverse Kinematics

Problem No – 1

Assume that you have a two-link manipulator with 𝑎1 = 15cm and 𝑎2 = 15cm and that the base of the manipulator is at the origin of the coordinate system. Write a Python program to take the list of workspace points and plug them into the inverse kinematics formulas for the two link manipulator. Plot these points on a graph where 𝜃1 is the horizontal axis and 𝜃2 is the vertical axis. You will have to adjust some aspects to get a good looking plot. (Scale factors etc.) Test your code on the workspace line (a) 𝑥 + 𝑦 = 25, 𝑥, 𝑦 > 0 and (b) 𝑥 = 10 cos(𝑡) + 15, 𝑦 = 10 sin(𝑡) for 0 ≤ 𝑡 ≤ 𝜋. The point here is to see what the configuration space curve looks like.

Solution –

Full Problem Solution Explanation – At the beginning of the solution array (t) of 50 points generated which are equally spaced between 0 to 3.14. Further, these points have passed through the forwarding kinematics equation which generates an array x and y coordinates of the manipulator (requested path fig.1). All the generated points provide the location of x and y coordinates of individual points. Then points passed through Inverse Kinematics equations which generate two angles (t1, t2) (joint angles fig.2) with the end positions of two link manipulators (x1, y1). At the end plot all points using matplot library (traversed path fig.3).

![1 1](https://user-images.githubusercontent.com/50337861/80894022-64a7fa00-8c94-11ea-932f-025307e36e02.png)
![1 2](https://user-images.githubusercontent.com/50337861/80894024-65409080-8c94-11ea-8663-5df970548af1.png)
![1 3](https://user-images.githubusercontent.com/50337861/80894025-65409080-8c94-11ea-8968-fb328468ef49.png)

Problem No – 2

Assume that you have a two-link manipulator with 𝑎1 = 15cm and 𝑎2 = 15cm and that the base of the manipulator is at the origin of the coordinate system. Write a two-link manipulator location program (Python). This program will take a list of angles and compute the location of the end effector. Show how this program works with the list of angles you generated in the previous problem. If the angle inputs are generated by a square, the simulated robot arm’s end-effector should trace a square. Plot the end effector points. You need to plot the input shape and the final shape to see if your code is correct. You will need to use the previous problem with this problem. Demonstrate your code to trace out the four segments which form the square with endpoints (5,0), (5, 15), (20, 15), (20,0).

Solution –

Full Problem Solution – Problem statement consists of four lines so 4 arrays generated for each line. Each array consists of 30 points (requested path fig.1). Inverse Kinematics function made in order to repeat the same process for 4 lines. It takes x and y input of each point and returned joint angles t1, t2 and location x1, y1. Returned values stored inside the array. In the end, all four arrays concatenate and made one single array and plotted that array using a matplot library (joint angles fig.2)(traversed path fig.3).


![2 1](https://user-images.githubusercontent.com/50337861/80894030-76899d00-8c94-11ea-9e86-b3ceb265f73b.png)
![2 3](https://user-images.githubusercontent.com/50337861/80894031-77baca00-8c94-11ea-98ae-c3e05e581261.png)
![2 2](https://user-images.githubusercontent.com/50337861/80894033-78536080-8c94-11ea-8ef3-f52823c14e1b.png)





Problem No – 3

Using Numpy and the space command, build an array of points for Fig. 2.37. The top is given by (𝑥−10)^2+(𝑦−8)^2 = 25 and the bottom is the line segment along with 𝑦 = 8. Traverse the figure starting at the right corner, going counter-clockwise (circle first) and ending on the line segment. Check this with the Python plot command. Show the result.

Solution –

On the basis of the above equation x and y calculated which is the center of the circle is (10,8) with radius r = 5. Using linespace command parallel line plotted with a distance of 10 units (r x 2) center of the distance (10,8). In the ‘for’ loop, an array of 200 points generated on the basis of circle equations (x,y) and points are equally spaced from 0 to 3.14. coordinates of these points are stored in an array named curve and plotted them along x and y a six using matplotlib library (semi-circle and line path fig.1).

![D](https://user-images.githubusercontent.com/50337861/80894042-873a1300-8c94-11ea-81c6-67b87b0daf43.JPG)
![3 1](https://user-images.githubusercontent.com/50337861/80894045-886b4000-8c94-11ea-9bcb-5aa811b65a4b.png)


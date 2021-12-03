# pi_estimation

Choose n number of randomly generated points where:

x = np.random.uniform(-1, 1)
y = np.random.uniform(-1, 1)
distance = np.sqrt( x^2 + y^2 )

We know that for a distance <= 1 that the point will be within the circle (r =1 , centered at (0,0)). Anything greater than this will be outside of the circle

Plot the points within the circle in red and add them to the counter points_circle += 1 (also being added to the points_total)
Plot the points outside the circle in blue and add them to the counter points_total += 1

To visualize this a little better I also plotted the unit circle itself using:

r = 1


angle = np.linspace(0, 2* pi, n)

x_c = r * np.cos(angle)

y_c = r * np.sin(angle)

Finally the estimation of pi itself. Using the area of a circle and the area of a square, we can set up the following ratio

# question1-for-saurabh
here is code where there is a method with a parameter though the parameter does not seem to be defined, but somehow the code still works.  could you explain to me why that is so?  the argument I have a question about is "other_point"

import math

class Point:

    def move(self, other_point):
        return math.sqrt((self.x - other_point.x)**2 + (self.y - other_point.y)**2)
        
point1 = Point()
point2 = Point()

point1.reset()
point2.move(5, 0)
print(point2.calculate_distance(point1))
assert (point2.calculate_distance(point1)) == (point1.calculate_distance(point2))
point1.move(3,4)
print(point1.calculate_distance(point2))
print(point1.calculate_distance(point1))

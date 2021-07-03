Given $n$ lines, containing two points $x[i]$ and $y[i]$. When see a line as border, calculate the difference between number of points on two sides. A point is formed when 2 lines intersect, and there are no 3 lines intersect at the same point.
Solution: For each line, first sort the slope in some way so that we know where each line starts, then we see the intersections with the current line and count the number of inversions. Each pair of inversions means that the two lines have intersected before meeting the current line. This problem is merely just a [[geometry]] problem, and we may need to use [[binary indexed tree]] to find the number of inversions.
Complexity: $O(n^2logn)$ (($nlogn$) to count inversions)
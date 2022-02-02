---
Recreation Activity
---
In this table we are going to see 4 kinds of sports that are available in your town and the cost of playing for each team is also mentioned.

| Sport Type |    Location    | Amount |
| :--------: | :------------: | :-----: |
|  Cricket  |   Oval Park   | 36.76 $ |
| Badminton |  Square Park  | 54.45 $ |
|   Soccer   | Rectangle Park | 76.67 $ |
| Basketball |     D-Park     | 48.75 $ |

---

    Pithy Quotes

---

> I have only made this letter longer because I have not had the time to make it shorter.

-*Blaise Pascal, The Provincial Letters*

> “Mathematicians deal with large numbers sometimes, but never in their income.”

― *Isaac Asimov, Prelude to Foundation*

---

Code Fencing

---

###### S547050 // last digit - 0 // Algorithm - Geometry Elementary/Polygons

> In geometry, a polygon is a plane figure that is described by a finite number of straight line segments connected to form a closed polygonal chain (or polygonal circuit). The bounded plane region, the bounding circuit, or the two together, may be called a polygon.

[Click this for more on Polygons](https://codeforces.com/blog/entry/48868)

code for the *Oriented Area Of Triangle*

~~~
int signed_area_parallelogram(point2d p1, point2d p2, point2d p3) {
    return cross(p2 - p1, p3 - p2);
}

double triangle_area(point2d p1, point2d p2, point2d p3) {
    return abs(signed_area_parallelogram(p1, p2, p3)) / 2.0;
}

bool clockwise(point2d p1, point2d p2, point2d p3) {
    return signed_area_parallelogram(p1, p2, p3) < 0;
}

bool counter_clockwise(point2d p1, point2d p2, point2d p3) {
    return signed_area_parallelogram(p1, p2, p3) > 0;
}
~~~

[Soucrce Code On this](https://cp-algorithms.com/geometry/oriented-triangle-area.html)
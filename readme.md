# Generate .obj normals

Generate vertex normal data from wavefront .obj file

**Input:** sample.obj (without vertex normal info) <br> 
**Output:** sample_out.obj (with vertex normal info)


### Run
```
python normal.py filepath
```


### Sample file input:
```
# cube.obj

v 0.0 0.0 0.0
v 0.0 0.0 1.0
v 0.0 1.0 0.0
v 0.0 1.0 1.0
v 1.0 0.0 0.0
v 1.0 0.0 1.0
v 1.0 1.0 0.0
v 1.0 1.0 1.0

f 1 7 5
f 1 3 7
f 1 4 3
f 1 2 4
f 3 8 7
f 3 4 8
f 5 7 8
f 5 8 6
f 1 5 6
f 1 6 2
f 2 6 8
f 2 8 4
```

### Sample file output:
```
# cube_out.obj

v 0.0 0.0 0.0
v 0.0 0.0 1.0
v 0.0 1.0 0.0
v 0.0 1.0 1.0
v 1.0 0.0 0.0
v 1.0 0.0 1.0
v 1.0 1.0 0.0
v 1.0 1.0 1.0

vn 0.0 0.0 -1.0
vn 0.0 0.0 -1.0
vn -1.0 0.0 0.0
vn -1.0 0.0 0.0
vn 0.0 1.0 0.0
vn 0.0 1.0 0.0
vn 1.0 0.0 0.0
vn 1.0 0.0 0.0
vn 0.0 -1.0 0.0
vn 0.0 -1.0 0.0
vn 0.0 0.0 1.0
vn 0.0 0.0 1.0

f 1//1 7//1 5//1
f 1//2 3//2 7//2
f 1//3 4//3 3//3
f 1//4 2//4 4//4
f 3//5 8//5 7//5
f 3//6 4//6 8//6
f 5//7 7//7 8//7
f 5//8 8//8 6//8
f 1//9 5//9 6//9
f 1//10 6//10 2//10
f 2//11 6//11 8//11
f 2//12 8//12 4//12
```
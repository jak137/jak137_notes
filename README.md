# JAK's miscellaneous notes

## MC extension file

### Show .stl files with https://openscad.org/ 

```
[STL]
Shell=.stl
Open=openscad %f
```

Press <F5> to show preview.


### Preview Jupyter notebooks (code only) with https://jqlang.org/ 


```
[IPYNB]
Shell=.ipynb
View=%view{ascii} cat %f | jq '.cells[] | (.source + ["\\n"]) | join("")' -r
```

### Metadata of HDF5 files

```
[HDF5]
Shell=.h5
View=%view{ascii} h5dump -A %f
```

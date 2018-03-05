# orhowdoihandlemissdickeypython
dict
```
favorite={"k1":"v1","k2":"v2"}
```
###### 01:30
simplest way
```
"k3" in favorite  #false
```

###### 03:20
get method
```
dictname.get("key","fallback")
```
the final solution:
```
def describe(category):
  missing = object()
  fav = favorites.get(category,missing)
  if fav is missing:
    message = "{} not exist".format(category)
  else:
    "{} is {}".format(category,fav)
  print(message)
  
```

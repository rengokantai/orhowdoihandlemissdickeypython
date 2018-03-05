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

###### 05:00
```None``` sentinal.  
Do not work if the value is `None`
```
def describe(category):
  fav = favorites.get(category)
  if fav is None:
    message = "{} not exist".format(category)
  else:
    "{} is {}".format(category,fav)
  print(message)
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

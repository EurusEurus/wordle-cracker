# wordle-crash
- [wordle: a daily world game](https://www.powerlanguage.co.uk/wordle/)
- wordle-crash: guess answer  


## usage
```python
status = {
    "green": 0,
    "yellow": 1,
    "gray": -1
}
```
Build function arguments from responses

```python
reqp = {"y": 1, "o": -1, "u": 1, "n": -1, "g": -1}
```

```shell script
python wordle.py
```

# example
```python
resp = {"y": 1, "o": -1, "u": 1, "n": -1, "g": -1}
```
```txt
lummy
lumpy
luray
lurky
lurry
lusby
lushy
lusky
lusty
mucky
...
```

## todo
- [x]  dict generate english world token len(token) == 5
- [ ]  [optimization] Recommendations based on word components && init world
- [x]  status   {"green":0,"yellow":"1","gray":"-1"}
- [ ]  request  ["w","a","t","e","r"]
- [x]  response {"w":0,"a":1,"t":-1,"e":1, "r":1}
- [x]  filter or transfer
- [ ]  Method 1 Generate a rule transfer function according to eachset
 of responses, and optimize on the basis of the original functio  n
- [x]  Method 2 Generate a regular function according to each set of responses,
 and further filter on the dictionary
- [ ]  [optimization] Recommendations based on word components && init world
- [ ]  [analyze] Can guess 6 times to cover the solution space?
# wordle-crash
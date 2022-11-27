# Python Goodies 🐍

## Profile a script to get a list of all function calls sorted by cumulative time:
```
python3 -m cProfile -s cumtime ./thescript.py
```

## Debug a script:
```
python3 -m pdb ./thescript.py
```
This will throw you into the debugger right from the start.
`c<enter>` will run the script.
If it encounters an error, you will be back in the debugger and be able to examine local variables.

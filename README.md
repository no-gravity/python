# Python Goodies 🐍

## Profile a script to get a list of all function calls sorted by cumulative time:
```
python3 -B -m cProfile -s cumtime ./thescript.py
```

## Debug a script:
```
python3 -B -m pdb ./thescript.py
```
This will throw you into the debugger right from the start.
`c<enter>` will run the script.
If it encounters an error, you will be back in the debugger and be able to examine local variables.

## Debug a script with a breakpoint:
```
python3 -B -m pdb -c 'b some_module.py:123' ./thescript.py
```

## Debug from within a script:
pudb is a nicer experience than pdb.
Put this where you want the debugger to kick in:
```
import pudb; pudb.set_trace();
```

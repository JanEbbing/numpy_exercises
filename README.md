# My run through the first 70 of the 100 NumPy exercises.

*AI assistance status*: No AI used for any solutions. Sometimes I used `hint` for help, I extensively used the numpy documentation and asked Claude after solving some of the exercises. In some cases I found the questions unclear and needed to use the `answer()` help.

Based on [rougier](https://github.com/rougier/)'s [repo](https://github.com/rougier/numpy-100). You'll need the `initialise.py`, `generators.py` files and the `source` directory to run this yourself (I'd just recommend cloning his repo).

## Requirements

Set up a virtual environment and install the dependencies

```
pip install numpy mdutils nbformat
```

Copy the `initialise.py`, `generators.py` and `source` directory from the original repo into this repository.

Open the jupyter notebook and try the exercises in each cell/the `hint(question_id)`/`answer(question_id)` helper functions (e.g. `hint(1)` for the hint to the second question).

## Comments

I found this a super valuable resource to get more comfortable with numpy notation and writing code myself.
I used no AI assistance to do any of the exercises (that would defeat the purpose IMO), the `hint()` and `answer()` methods are super useful however.
There are a few times when the question is very short and I was not 100% sure what the author wanted, I usually did the exercise as I understood it, and then double checked with the `answer`.
I can also whole-heartedly recommend asking an LLM after trying an exercise yourself - there are often surprising nuances why something gives a certain result that is lost if you just compare your answer to the gold standard.

Overall I probably spent around 10h on this (hard to estimate, also requires a lot of concentration). After doing ~50 I found the usefulness of each new one quickly diminished.

Learnings: The point of numpy is obviously to perform common matrix operations in fast C code, rather than slow python code. In practice, this means
you need to rewire your brain a bit - tasks that you can easily solve in python need to now be solved via the existing NumPy library functions, so you need to
find the right keyhole to push your problem through. There are also some lower level details that are somewhat hidden in docs or that you should know, e.g. about memory
allocation (some methods allow you to specify an output array, some methods are in-place, others create a new array), time complexity of some operations, what the memory
layout of an array is like, etc

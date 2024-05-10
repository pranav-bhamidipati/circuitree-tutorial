# circuitree-tutorial
Tutorials and source code for the [`circuitree`](https://github.com/pranav-bhamidipati/circuitree) package.

# Quick start

Clone the repository onto your filesystem

```git clone https://github.com/pranav-bhamidipati/circuitree-tutorial.git```

Move into the `circuitree-tutorial` directory

```cd circuitree-tutorial```

Make a virtual environment, activate it, and install the required package(s)

```
python -m venv ./env
source ./env/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```

Now, you can run any of the executable scripts in the `src` directory by running `python ./run_search.py`. 

# Usage

[Tutorial notebook #1](src/tutorial-1-getting-started.ipynb) describes the basics of using the package by walking through how to write a `CircuiTree` class and run a search for an example design problem. If you're just looking for example code, the module `bistability.py`contains just the functions and classes defined in the first tutorial, and `run_search.py` is an executable script that runs the tree search. 

The [parallel search notebook](src/tutorial-2-mcts-in-parallel.ipynb) explains how parallelism is achieved in the package and how to set up the required infrastructure for a parallelized search. The modules `bistability_parallel.py` and `bistability_app.py` and the executable script `run_search_parallel.py` contain example code for writing a parallelizable `CircuiTree` object and running a parallel search.

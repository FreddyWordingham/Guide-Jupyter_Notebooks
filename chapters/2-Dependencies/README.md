# Dependencies

## Add dependencies

I'm going to write a notebook to plot some interesting locations in the Mandelbrot set.
First I'll need to install the package we created in the previous guide.

We can do this either from `pypi`:

```shell
poetry add mandybrot
```

Or from a directory:

```shell
poetry add ../path/to/Mandybrot
```

## Try it out

Run the notebook server:

```shell
poetry run jupyter notebook examples --port 8888
```

And then import the `mandybrot` package:

```python
import mandybrot as mandy
```

Open https://localhost:8888 in your browser and open the `mandybrot.ipynb` notebook.
Get plotting!

## Return

[Return to the top-level README](./../../README.md)

# Setup

We'll create the minimal file structure for a Python project using the Poetry package manager with the Jupyter notebooks tool installed.

## Poetry init

Create a new Poetry project:

```shell
poetry init
```

-   I'm going to call this project `my_notes`
-   Starting at version `0.1.0`
-   My description will be: `Jupyter notebook example.`
-   I am: `Freddy Wordingham <freddy@digilab.co.uk>`
-   I'm not going to add a license
-   Compatible with Python versions `3.8` and above
-   And I'm not going to add any dependencies right now

This will generate a [`pyproject.toml`](./pyproject.toml) file containing the project metadata.

As we're not building a package here, we'll remove the `packages` section from the `pyproject.toml` file.

## Install the package

We can install the package by running the following command:

```shell
poetry install
```

## Add .gitignore

I'm going to add a [`.gitignore`](./.gitignore) file to my project.
Python projects use a lot of files that we don't want to commit to Git, so we can use a template to generate a `.gitignore` file for us.

I'm going to pull the code from https://www.toptal.com/developers/gitignore/api/python into a `.gitignore` file using the `curl` command:

```shell
curl -L https://www.toptal.com/developers/gitignore/api/python > .gitignore
```

Alternatively, you can go to [gitignore.io](https://gitignore.io/) and generate a template more tailored to your needs.

## Add Jupyter

We're going to need the `jupyter` tool to get started:

```shell
poetry add jupyter
```

## Try it

We can run the application by running the following command:

```shell
poetry run jupyter notebook --port 8888
```

This will start a notebook server on port 8888.
If you go to http://localhost:8888, you should see the Jupyter notebook interface.

## Return

[Return to the top-level README](./../../README.md)

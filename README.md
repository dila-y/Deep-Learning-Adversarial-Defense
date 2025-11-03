# Adversarial Attacks

This directory contains code and examples related to adversarial attacks on machine learning models. Adversarial attacks are techniques used to fool models by providing deceptive input.

## How to use

As always, start by installing the required packages:

```bash
uv sync
```

> **Warning**  
> Mac OS user on Intel CPU: builds for recent Python and TensorFlow versions may fail.

Use the Mac OS Intel CPU environment:

```bash
cp .python-version-macos-intel .python-version
cp pyproject-macos-intel pyproject.toml
uv sync
```

And add this line in the first cell of your notebook:

```python
tf.compat.v1.disable_eager_execution()
```

---
layout: single
title: Including a Jupyter notebook in Github Jekyll
excerpt: Some examples of the capabilitites of Jekyll and Notebooks

---
The goal of this post is to share how to make Jupyter notebook generate Markdown for Github. This accelerates the publication of code and ideas. Jupyter notebook is a feature-rich environment where you can type equations, put code, and figures.

The basic idea is to run a basic script in the `notebooks` folder, named `run_jupyter.sh`, which runs a custom configuration for Jupyter notebook. This configuration adds a hook to the saving cycle of the notebook. This hook transforms the Jupyter notebook (`.ipynb`) file into a Markdown file (`.md`) and generates the figures embeeded in it. Then, it moves the files into the `_posts` folder. Then, you only need to run Jekyll to see how the post look like.

First, I will load some Python packages:


```python
%matplotlib inline
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
```

I will run plot this simple example:


```python
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt

sns.set(style="dark")
rs = np.random.RandomState(50)

f, axes = plt.subplots(3, 3, figsize=(9, 9), sharex=True, sharey=True)

for ax, s in zip(axes.flat, np.linspace(0, 3, 10)):

    # Create a cubehelix colormap to use with kdeplot
    cmap = sns.cubehelix_palette(start=s, light=1, as_cmap=True)

    # Generate and plot a random bivariate dataset
    x, y = rs.randn(2, 50)
    sns.kdeplot(x, y, cmap=cmap, shade=True, cut=5, ax=ax)
    ax.set(xlim=(-3, 3), ylim=(-3, 3))

f.tight_layout()
```


![png](2017-05-27-jupyter-notebook-to-markdown_files/2017-05-27-jupyter-notebook-to-markdown_5_0.png)


Also, you can add math $$f(x) = 1 + x^2$$

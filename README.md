# Travail Pratique 2 : Arbres
travail_pratique


```{python}
#| output: true
#| echo: false
import os
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
from matplotlib import rc

from sklearn import tree, datasets
from sklearn.model_selection import train_test_split
from tp_arbres_source import (rand_gauss, rand_bi_gauss, rand_tri_gauss,
                              rand_checkers, rand_clown,
                              plot_2d, frontiere)


rc('font', **{'family': 'sans-serif', 'sans-serif': ['Computer Modern Roman']})
params = {'axes.labelsize': 6,
          'font.size': 12,
          'legend.fontsize': 12,
          'text.usetex': False,
          'figure.figsize': (10, 12)}
plt.rcParams.update(params)

sns.set_context("poster")
sns.set_palette("colorblind")
sns.set_style("white")
_ = sns.axes_style()
```
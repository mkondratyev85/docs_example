<!-- DO NOT EDIT. -->
<!-- THIS FILE WAS AUTOMATICALLY GENERATED BY SPHINX-GALLERY. -->
<!-- TO MAKE CHANGES, EDIT THE SOURCE PYTHON FILE: -->
<!-- "auto_gallery-2/plot_0_gal2_example.py" -->
<!-- LINE NUMBERS ARE GIVEN BELOW. -->

<a id="sphx-glr-auto-gallery-2-plot-0-gal2-example-py"></a>

# First example of gallery 2

Here we will provide some different examples that show how Sphinx-Gallery can
capture figures output by Matplotlib and html representations of objects,
if present.

<!-- GENERATED FROM PYTHON SOURCE LINES 9-14 -->
```Python
import matplotlib.pyplot as plt

_ = plt.plot([1,2,3])
```

<!-- GENERATED FROM PYTHON SOURCE LINES 15-16 -->

pandas dataframes have a html representation, and this is captured:

<!-- GENERATED FROM PYTHON SOURCE LINES 16-24 -->
```Python
import pandas as pd

df = pd.DataFrame({'col1': [1,2,3],
                   'col2': [4,5,6]})
df

# s = pd.Series([1,2,3])
```

<div class="output_subarea output_html rendered_html output_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>col1</th>
      <th>col2</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1</td>
      <td>4</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2</td>
      <td>5</td>
    </tr>
    <tr>
      <th>2</th>
      <td>3</td>
      <td>6</td>
    </tr>
  </tbody>
</table>
</div>
</div>
<br />
<br />

**Total running time of the script:** (0 minutes 0.150 seconds)

<a id="sphx-glr-download-auto-gallery-2-plot-0-gal2-example-py"></a>

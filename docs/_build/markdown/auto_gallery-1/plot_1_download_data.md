<!-- DO NOT EDIT. -->
<!-- THIS FILE WAS AUTOMATICALLY GENERATED BY SPHINX-GALLERY. -->
<!-- TO MAKE CHANGES, EDIT THE SOURCE PYTHON FILE: -->
<!-- "auto_gallery-1/plot_1_download_data.py" -->
<!-- LINE NUMBERS ARE GIVEN BELOW. -->

<a id="sphx-glr-auto-gallery-1-plot-1-download-data-py"></a>

# Data download example

This example shows one way of dealing with large data files required for your
examples.

The `download_data` function first checks if the data has already been
downloaded, looking in either the data directory saved the configuration file
(by default `~/.sg_template`) or the default data directory. If the data has
not already been downloaded, it downloads the data from the url and saves the
data directory to the configuration file. This allows you to use the data
again in a different example without downloading it again.

Note that examples in the gallery are ordered according to their filenames, thus
the number after ‘plot_’ dictates the order the example appears in the gallery.

<!-- GENERATED FROM PYTHON SOURCE LINES 18-36 --><div class="output_subarea output_html rendered_html output_result">
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
      <th>0</th>
      <th>1</th>
      <th>2</th>
      <th>3</th>
      <th>4</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>5.1</td>
      <td>3.5</td>
      <td>1.4</td>
      <td>0.2</td>
      <td>Iris-setosa</td>
    </tr>
    <tr>
      <th>1</th>
      <td>4.9</td>
      <td>3.0</td>
      <td>1.4</td>
      <td>0.2</td>
      <td>Iris-setosa</td>
    </tr>
    <tr>
      <th>2</th>
      <td>4.7</td>
      <td>3.2</td>
      <td>1.3</td>
      <td>0.2</td>
      <td>Iris-setosa</td>
    </tr>
    <tr>
      <th>3</th>
      <td>4.6</td>
      <td>3.1</td>
      <td>1.5</td>
      <td>0.2</td>
      <td>Iris-setosa</td>
    </tr>
    <tr>
      <th>4</th>
      <td>5.0</td>
      <td>3.6</td>
      <td>1.4</td>
      <td>0.2</td>
      <td>Iris-setosa</td>
    </tr>
  </tbody>
</table>
</div>
</div>
<br />
<br />
```Python
import pandas as pd
import SampleModule.data_download as dd


data_file = dd.download_data(
    url='http://archive.ics.uci.edu/ml/machine-learning-databases/iris/iris.data',\
    data_file_name='iris.csv',
    data_key='data_dir')

iris = pd.read_csv(data_file, header=None)
iris.head()
```

**Total running time of the script:** (0 minutes 0.394 seconds)

<a id="sphx-glr-download-auto-gallery-1-plot-1-download-data-py"></a>
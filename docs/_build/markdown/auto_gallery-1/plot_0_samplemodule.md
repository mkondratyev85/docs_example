<!-- DO NOT EDIT. -->
<!-- THIS FILE WAS AUTOMATICALLY GENERATED BY SPHINX-GALLERY. -->
<!-- TO MAKE CHANGES, EDIT THE SOURCE PYTHON FILE: -->
<!-- "auto_gallery-1/plot_0_samplemodule.py" -->
<!-- LINE NUMBERS ARE GIVEN BELOW. -->

<a id="sphx-glr-auto-gallery-1-plot-0-samplemodule-py"></a>

# SampleModule example

This example will demonstrate the `power` function and `class_power` from
our package ‘SampleModule’.

<!-- GENERATED FROM PYTHON SOURCE LINES 8-13 -->
```Python
import SampleModule.module

SampleModule.module.fun_power(2,3)
```

```none
8
```

<!-- GENERATED FROM PYTHON SOURCE LINES 14-16 -->

The function `power` returns the first number raised to the power of the
second number.

<!-- GENERATED FROM PYTHON SOURCE LINES 16-20 -->
```Python
my_class = SampleModule.module.class_power(2,3)
my_class.power()
```

```none
8
```

<!-- GENERATED FROM PYTHON SOURCE LINES 21-23 -->

Instances of `power_class` have a `power` method. If a non-number is
used when initiating the class, an informative statement is printed:

<!-- GENERATED FROM PYTHON SOURCE LINES 23-26 -->
```Python
my_class = SampleModule.module.class_power('a',3)
my_class.power()
```

```none
Something went wrong. Make sure x and y are both numbers
```

**Total running time of the script:** (0 minutes 0.002 seconds)

<a id="sphx-glr-download-auto-gallery-1-plot-0-samplemodule-py"></a>
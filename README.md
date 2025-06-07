# Elementum
## General Information
Element is a Python library that allows users to easily get information on the elements. It also allows you to make compounds from those elements.

## Documentation
To create an instance of an element, type:

```py
import elementum
element = elementum.Element("Hydrogen")
```

Note that `element = elementum.Element("H")`, `element = elementum.Element(1)`, or `element = elementum.Element(1.008)` will also work.

Once an element is created, you can view its properties with the `identity` function, used like this:

```py
import element
h = elementum.Element("Hydrogen")
print(h)
```

The identity property shows the element's:
- Name
- Symbol
- Atomic Number
- Atomic Mass (rounded to 3 decimal places)
- Type (Alkali metals, Noble gasses, etc.)
- Radioactivity (either True or False)

To view common compounds containing the element, there is another function called `compounds`.

```py
import element
h = elementum.Element("Hydrogen")
print(h.compounds())
```

Last but not least, one can view the full periodic table with the `table` function.

```py
import element
table = elementum.table()
```

## Compounds
You can add elements together and multiply them to make compounds, like so:

```py
import element
H = elementum.Element("Hydrogen")
O = elementum.Element("Oxygen")
water = H*2+O
print(water)
```
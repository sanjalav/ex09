---
# Do not edit the text between these lines!
layout: default
---

# This is a big header

<!-- This is a comment. Below, you'll see code for inserting an image. To make this image appear, update <custom-path>. To add an image, save it inside the imgs folder of this repository. -->
<img src="<custom-path>/static/imgs/logo.png" alt="Image of Comp110 rainbow logo. "  width="500"/>

## This is a small header

This is basic paragraph text.

#Comp110 Data Analysis: Student Insights

Welcome! I'm Sanjala Vasudev. As an undergraduate at UNC Chapel Hill pursuing a Bachelors of Science in Neuroscience, I am passionate about using computational tools to uncover meaningful patterns in human behavior. 

This project showcases a custom data utility library I built to process and analzye campus survey data.

#Technical Implementation: 'data_utils.py'

To perform my analysis, I developed several key functions to transform "raw" CSV data into a format that Python can easily manipulate.

#test

### 1. Data Selection and Transformation
The 'select' and 'columnar' functions allow me to isolate specific variables-like a student's major and their class year-from a massive dataset.

```python
def select(table: dict[str, list[str]], names: list[str]) -> dict[str, list[str]]:
    """Isolates a specific subset of columns for focused analysis."""
    result: dict[str, list[str]] = {}
    for name in names:
        result[name] = table[name]
    return result

The count function is the engine of my analysis, allowing me to build frequency tables for categorical data.

def count(valyes: list[str]) -> dict[str, int]"
    """Produces a dictionary of unique value frequencies."""
    result: dict[str, int] = {}
    for item in values:
        if item in result:
            result[item] += 1
        else:
            result[item] = 1
    return result
```


Using these tools, I explored how different academic backgrounds impact the student experience in introductory computer science.

Reflecting on my experience, I believe the course could create even more value by incorporating industry-specific problem sets. This would help students see how Python can be a useful tool for automating data anlaysis in their specific professional domains.


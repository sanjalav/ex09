---
# Do not edit the text between these lines!
layout: default
---
test

# COMP110 Data Analysis: Student Insights

Welcome! I'm Sanjala Vasudev. As an undergraduate at UNC Chapel Hill pursuing a Bachelors of Science in Neuroscience, I am passionate about using computational tools to uncover meaningful patterns in human behavior. 

## Technical Implementation: 'data_utils.py'

To perform my analysis, I developed several key functions to transform "raw" CSV data into a format that Python can easily manipulate.

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


## Analysis: The Case for Interdisciplinary Examples

My analysis explored whether COMP110 should provide more examples from diverse fields to support student learning. Based on survey_izzi dataset, the data strongly supports this modification.

Major Distribution
Using the count utility, I visualized the academic backgrounds of students. The distribution shows a large variety of majors, including Biology, Economics, Psychology, and Media/Journalism.

CS vs Non-CS Interest in Connections
I compared interest levels in seeing connections between CS and other fields. While CS majors have high interest, Non-CS majors also reported significantly high scores (ratings 4-7).

Interest Density across All Students
The histogram below highlights that both groups value the integration of computer sicence with other professional domains. 


## Conclusion and Reflections
The analysis shows a high level of interest in the connections between computer science and other fields across all students.

Implementation and Trade-offs
I recommend that the course try to include at least one interdisciplinary example into each major module. While this would increase engagement, there are trade-offs:
    Cost: Creating these examples requires significant time and effort from instructors and TAs.
    Complexity: Diverse examples could potentially confuse students if the core programming logic is not kept consistent. 

Future Work
Ultimately, with the large number of non-CS majors taking this course, a "select your coding exercise" model, where students choose a "theme" for the same logic, would make the course much more engaging and practical.

<img src="/ex09/static/imgs/major_dist.png" alt="Distribution of Majors" width="600"/>

<img src="/ex09/static/imgs/interest_comparison.png" alt="Box Plot Comparison" width="500">

<img src="/ex09/static/imgs/interest_density.png" alt="Interest Histogram" width="500">



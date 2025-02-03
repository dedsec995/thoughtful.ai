### Package Sorting System

### Objective
The goal of this program is to classify packages based on their dimensions and mass into three categories: STANDARD, SPECIAL, or REJECTED.

### Classification Criteria
#### 1. Bulky Package
A package is considered bulky if:
Its volume (Width × Height × Length) is greater than or equal to 1,000,000 cm³.
Or if any one of its dimensions (Width, Height, or Length) is greater than or equal to 150 cm.
#### 2. Heavy Package
A package is considered heavy if:
Its mass is greater than or equal to 20 kg.
#### 3. Stack Classification
Packages are classified into the following stacks:

STANDARD: Packages that are neither bulky nor heavy.
SPECIAL: Packages that are either bulky or heavy, but not both.
REJECTED: Packages that are both bulky and heavy.
Function Implementation
`sort(width, height, length, mass)`
This function sorts the package based on the provided criteria and returns the appropriate stack name.

Parameters:
width (int or float): The width of the package in centimeters.
height (int or float): The height of the package in centimeters.
length (int or float): The length of the package in centimeters.
mass (int or float): The mass of the package in kilograms.
Returns:
"STANDARD" if the package is neither bulky nor heavy.
"SPECIAL" if the package is either bulky or heavy, but not both.
"REJECTED" if the package is both bulky and heavy.
Example:
``` python
sort(100, 100, 100, 15)
# Output: "STANDARD" (not bulky, not heavy)

sort(200, 50, 50, 15)
# Output: "SPECIAL" (bulky but not heavy)

sort(100, 100, 100, 25)
# Output: "SPECIAL" (heavy but not bulky)

sort(200, 200, 200, 30)
# Output: "REJECTED" (bulky and heavy)
```

### Usage
To use the sort() function, simply call it with the width, height, length, and mass of the package:
```bash
stack = sort(width, height, length, mass)
print(f"The package should be placed in the {stack} stack.")
```
### Installation
Just python interpreter. Just Copy the function into your Python environment and call the function.


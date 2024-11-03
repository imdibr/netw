# IP Address Finder using Backtracking

This repository contains a solution to find all valid IP addresses from a given string using backtracking. The solution explores possible placements of dots in the string to form valid IP addresses, verifying each possibility with backtracking.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Usage](#usage)
- [Example](#example)
- [Backtracking Approach](#backtracking-approach)
- [Requirements](#requirements)
- [Installation](#installation)
- [License](#license)

## Overview
The goal of this project is to parse a given string of digits and return all possible valid IP addresses. An IP address consists of four numbers (each between 0 and 255) separated by dots. Using backtracking, this solution identifies all valid placements of dots that form an IP address.

## Features
- Validates IP addresses with constraints:
  - Each segment is a number between 0 and 255.
  - No segment has leading zeroes unless it is "0".
- Backtracking ensures efficient exploration of possible solutions.
- Returns all valid IP addresses from the given string.

## Usage
1. Clone this repository.
2. Run the script by providing a string of digits as input.

### Function Signature
```python
def restore_ip_addresses(s: str) -> List[str]:
    """
    Finds all valid IP addresses from a string of digits using backtracking.
    
    Args:
        s (str): Input string containing only digits.

    Returns:
        List[str]: List of all valid IP addresses.
    ```
    
## Example
```python
# Example usage
input_str = "25525511135"
print(restore_ip_addresses(input_str))
# Output:
# [
#     "255.255.11.135",
#     "255.255.111.35"
# ]

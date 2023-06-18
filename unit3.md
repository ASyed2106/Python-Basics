### Tuples
  - Immutable sequenceable data-type object
  - Tuples are declared with parenthesis
  - () is an empty tuple
  - (50,) is a singleton tuple; the comma is required
  - Tuples are sliceable; therefore, indexable using square brackets

### map()
  - a = map(function_name, sequence)
  - map() is a built-in function that applies a given function to every item in the given sequence and returns the result.

### filter()
  - a = filter(bool_function_name, sequence)
  - filter() is a built-in function that filters out the items in the sequence that the function would evaluate to True and returns the result

### Iterator Function
  - A function that returns an object that is iterable.
  - The range() function returns an iterable collection of integer values that fit the criteria of the arguments

**range,map and filter are interator function**

### Sets
  - a well-defined collection of distinct objects, considered as an object in its own right. A set can be denoted with {} brackets mathematically
  - A set does not need to be ordered {a,b,c} == {c,b,a}
  - A set can contain duplicates; moreover, the set with no duplicates of same objects will still be considered equal
  - A set is a collection of discrete data items. The members of the set can be numbers or names.
 
### Union
  - The union of set A and set B is the result of all its member into a singular set with duplicate members discarded
    Example:
        A={Mary, Mark, Fred, Angela, Frank, Laura}
        B={Fred, Mary, Frank, Jane}
        A U B = {Mary, Mark, Fred, Angela, Frank, Laura, Jane}
 
 ### Interactions
   - The intersection of set A and B is members that are present in both sets
    Example:
        A={Mary, Mark, Fred, Angela, Frank, Laura}
        B={Fred, Mary, Frank, Jane}
        A intersect B = {Mary, Fred, Frank}

  #### Disjoint
    - Two sets are considered to be “disjoint” if the intersection is empty

### Subtraction
  - it doesn't really exist… The act of A - B results to removing the members that exist in set B from set A.

### Symmetric Difference
  - Elements that are in either set, BUT they cannot intersect

### Complement
  -A complement of set A will be the set that contain members from the Universe set that doesn’t exist in set A
  
### SETS IN PYHON
  -  A set is an unordered collection with no duplicate elements 
      - Uses
         - membership testing and eliminating duplicate entries
      - Supported Operations:
         - Union
         - Intersection
         - Difference
         - Symmetric Difference

### Sets
  - What can we do with Sets in Python 3:
        - Check membership → x in set
        - Determine the number of members → len(set)
        - Iterate through the set → for x in set
  - What can’t we do with Sets:
        - Sets are not indexable
        - Set cannot be sliced
        - Sets have no sequence-like behavior
        - Sets don’t record element position or order of insertion; therefore, we cannot sort

### Set Assignment Operations
  - # let setA and setB be sets
  - setA |= setB # Assigns the union of A and B to A
        # works also with setA.update(setB)
  - setA &= setB # Assigns the intersection of A and B to A
        # works also with setA.intersection_update(setB)
  - setA -= setB # Assigns the difference of A and B to A
        # works also with setA.difference_update(setB)
  - setA ^= setB # The symmetric difference of A and B to A
        # works also with setA.symmetric_difference_update(setB)

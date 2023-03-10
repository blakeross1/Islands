# Objective:

Write a program that reads stdin with these properties:

- Every line ends with a newline character.
- Every line has the same length.
- Every line consists of an arbitrary sequence of hyphens ("~") and carets ("\^").
- The final line of input is terminated by a newline character.

This input represents a rectangular section of a map. Each `~` represents water, and
each `^` represents land. One or more contiguous `^`s represents an island, with
contiguity defined as horizontal or vertical (but _not_ diagonal) adjacency.

## Example Island

```
~~^~~~
~~~^~~
~~~^~~
```

# How to Use:

## Built using:
- Python 3.10.4
- numpy 1.22.3

## You may use map from a .txt file or type a map on the terminal input
### Text File:
- The txt file must be contained in the same dir as the .py file.
- Include the name of the text file as a parameter in the terminal command.
```
python islandArea.py map.txt
```
Result:
```
Using Map:  map.txt
The largest island is: 11 in size.
```
### Terminal Input
- If no argument is provided or the file is not found you may type in your own map.
- Type in each line of the map followed by return
- When finished enter end of message (Ctrl+Z on Windows, Ctrl+D on mac)
```
python islandArea.py
```
Result:
```
No file provided.
Please type in your map: (Ctrl+Z on Windows, Ctrl+D on mac when finished)
~~~^^^~~^^
~~^^^~~~~
^^~~~~^^~^
^Z
The largest island is: 6 in size.
```

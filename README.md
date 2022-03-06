
# Basic Usages

## Problem Choosen
Shell Sort vs Recursive Bubble Sort

## Installation of Packages
The program is written in python. Make sure you have python3 on your computer. You also need to install some required packages by using these following commands

$ pip install -r requirements.txt

## Running the code
Use Jupyter notebook to run the program.The file by name AOS_Project_SourceCode has to be taken where in we need to run all the cells having the programs.

## Analysis of the Problem
This project aims to retrieve system-level information of programs in addition to user-level and then uses this information to compare the two algorithms under three different conditions namely,
- The Shell Sort Algorithm only
- The Recursive Bubble Sort Algorithm only
- The two programs running simultaneously

The aspects we followed in this project are as follows:
- Running time of the program
- CPU Usage
- Memory Usage(Resident set size, Virtual memory size, etc)
- Hard drive usage
- Number of Page Faults

# Solution Design 
The first program named shell sort executes by sorting the pairs of elements far apart from each other then progressively reducing the gap between elements to be compared.The second program named Recursive Bubble Sort executes by repeatedly comparing the adjacent elements and swapping them if they are in the wrong order. The repeated comparisons bubble up the smallest/largest element towards the end of the array. The data is given randomly using random() function. We run and take measurements for these programs and then compare the results. In order to measure system-level information we make use of package [psutil] to carry out the experiments. All the programs are written in python and run in jupyter notebook.


## Comparisons
The ***Shell sort*** takes longer time to finish than ***recursive bubble sort*** When running these programs simultaneously, each program takes more time when ran simultaneously than alone because there is more work for CPU in the former case as two programs are being run simultaneously

In terms of CPU Utilization, ***Shell Sort*** has better CPU Percent than ***Recursive Bubble Sort***. These numbers have increased when we run the two programs simultaneously as two programs are running at the same time CPU Utilization has increased.

Besides, the *Resident set size* (RSS), *Virtual memory size* (VMS),  *Unique Set Size* (USS - the memory unique to a process and which would be freed if the process was terminated right now) and *Size on Hard Disk* are almost the same in the two programs in both the conditions. It is worth mentioning that we can see the *VMS(s)* are much large than *RSS(s)*.

In terms of *the number of Page-faults*, the number of ***Shell Sort*** is a bit smaller than that of ***Recursive Bubble Sort***. These figures are similar when running the two programs at the same time, just a slight smaller for shell sort when compared to recursive bubble sort.

## SnakeViz
SnakeViz is a viewer for profiling the data which runs as a web application in your browser.


## Results
The results for the programs run separately and the programs runs simultaneously can be found in the word document named AOS_Project_Doc.

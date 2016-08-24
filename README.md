# mimic
Workload generator
Copyright (c) 2016 Michael Cahill (michael.cahill@gmail.com)

Python code to generate multi-threaded database workloads.

## Manifesto

* Describe workloads with Python code.
 * Make use of scripting, inheritance, etc.
* Do as much as possible in Python except threading.
 * includes creating databases / tables for most cases.
 * keep Python code deterministic (including generating identical workloads
   for a given input and random seed).
* Generate portable C11 and invoke GCC / clang to create a workload binary.
* Develop separately from a specific database, so a specific version of
  mimic can easily test multiple versions of the database.

## Goal

* Become the go-to tool for performance testing and multi-threaded testing
  for WiredTiger

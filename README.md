# Unexpected Behavior of Direct Assignment to Getter Methods in Ruby

This repository demonstrates an unexpected behavior in Ruby concerning direct assignment to getter methods. In many other languages, assigning a value to a getter would implicitly update the underlying internal variable (setter).  In Ruby, this is not the case.

The `bug.rb` file showcases the issue. The `bugSolution.rb` provides a proper solution.

## Problem
Direct assignment to a getter method in Ruby does not update the instance variable.  This can lead to unexpected results and hard-to-debug errors if the underlying behavior is not understood.

## Solution
The recommended approach is to use setter methods (or `attr_writer`) to modify instance variables.
# Ruby - Unexpected NoMethodError when modifying instance variable

This repository demonstrates a common error in Ruby related to modifying instance variables.  The `bug.rb` file contains code that attempts to modify an instance variable (`@value`) directly, causing a `NoMethodError`. The `bugSolution.rb` file shows how to properly define setter methods or use `attr_accessor` to fix this.

## Bug

The issue arises from attempting to assign a new value to the instance variable `@value` outside of the class's methods. In Ruby, instance variables are typically accessed and modified using getter and setter methods.

## Solution

The solution involves defining either a `value=` setter method or using `attr_accessor` to create both getter and setter methods automatically.
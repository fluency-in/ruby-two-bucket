# Ruby: Two Bucket

Given two buckets of different size, write a program to demonstrate how to measure an exact number of liters.

Given two buckets of different size, write a program to demonstrate how to measure an exact number of liters by strategically transferring liters of fluid between the buckets.

Since this mathematical problem is fairly subject to interpretation / individual approach, the tests have been written specifically to expect one overarching solution.

To help, the tests provide you with which bucket to fill first. That means, when starting with the larger bucket full, you are NOT allowed at any point to have the smaller bucket full and the larger bucket empty (aka, the opposite starting point); that would defeat the purpose of comparing both approaches! 

Your program will take as input:
- the size of bucket one, passed as a numeric value
- the size of bucket two, passed as a numeric value
- the desired number of liters to reach, passed as a numeric value
- which bucket to fill first, passed as a String (either 'one' or 'two')

Your program should determine:
- the total number of "moves" it should take to reach the desired number of liters, including the first fill - expects a numeric value
- which bucket should end up with the desired number of liters (let's say this is bucket A) - expects a String (either 'one' or 'two')
- how many liters are left in the other bucket (bucket B) - expects a numeric value

Note: any time a change is made to either or both buckets counts as one (1) move. 

Example: 
Bucket one can hold up to 7 liters, and bucket two can hold up to 11 liters. Let's say bucket one, at a given step, is holding 7 liters, and bucket two is holding 8 liters (7,8). If you empty bucket one and make no change to bucket two, leaving you with 0 liters and 8 liters respectively (0,8), that counts as one "move". Instead, if you had poured from bucket one into bucket two until bucket two was full, leaving you with 4 liters in bucket one and 11 liters in bucket two (4,11), that would count as only one "move" as well.

To conclude, the only valid moves are:
- pouring from one bucket to another
- emptying one bucket and doing nothing to the other
- filling one bucket and doing nothing to the other

Written with <3 at [Fullstack Academy](http://www.fullstackacademy.com/) by [Lindsay](http://lindsaylevine.com).
The tests use the Minitest testing framework. To install it run the command:

    gem install minitest

Run the tests with the `ruby` command:

    ruby two_bucket_test.rb

## Resources

If you have never used Minitest, check out [Intro to TDD][tdd] tutorial from Jumpstart Lab.

[tdd]: http://tutorials.jumpstartlab.com/topics/testing/intro-to-tdd.html

## Source

Water Pouring Problem [http://demonstrations.wolfram.com/WaterPouringProblem/](http://demonstrations.wolfram.com/WaterPouringProblem/)

This exercise is from the [Ruby][ruby] track on [Exercism][exercism]

[exercism]: http://exercism.io
[ruby]: http://exercism.io/languages/ruby




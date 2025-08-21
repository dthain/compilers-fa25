---
layout: default
title: Homework 2 - RegEx to Finite Automata

## Homework 2

**Problem 1** - Write regular expressions that match following entities.  (And don't match other things!)  Keep your expressions simple, sticking to the basic three operations and the limited extensions that we discussed in class.  You are encouraged to use `regex101.com` to test and develop your solutions.

- (a) Match any [ICAO airport code](https://en.wikipedia.org/wiki/ICAO_airport_code    
) from countries in North, Central, and South America.  Assume only upper case letters are used.  Take a good look at the black-and-white map that shows all the country.  Make the RE as compact as you can.  (Include the Carribean, exclude Greenland and Iceland.)
  Examples: `KSBN` or `SBGL` or `PANC`
- (b) Match any valid [IPv4 Address](https://en.wikipedia.org/wiki/Internet_Protocol_version_4) in dot-decimal format.  Note that no field can be larger than 255!
  Examples: `192.168.1.1` or `10.200.1.1` or `255.255.255.255`
- (c) Match any polynomial of degree three or less, with integer coefficients and powers.
  Examples: `5x^3-10` or `-10x^2+3x+20`
- (d) Match any string on the alphabet `{a,b,c}` of length three or greater that does **not** end in `abc`.
  Examples: `cba` or `ccbbaa` or `cbacba` or `abcabb`
- (e) Match any C-Style comment.
  Examples: `/* a comment */` `/* also *** a comment */` `/*******/`

**Problem 1: ** Convert these REs into NFAs using Thompson's construction:

- (a) `for | [a-z]+ | [xb]?[0-9]+`
- (b) `a ( bc*d | ed ) d+`
- (c) `( a*b | b*a | ba ) *`

**Problem 2:** Convert the NFAs in the previous problem into DFAs using the subset construction method.

- (a) from above
- (b) from above
- (c) from above

**Problem 3:** Combine the three DFAs



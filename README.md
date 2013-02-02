hw2_cs1300
==========

# basic_functions.py
#
# Your Name: Tatyana Sasynuik
# Your TA: Hally Profita (I'm pretty sure...)
# Your List of Colaborators:
#
# Welcome to your first *real* programming assignment in CS 1300! This
# is all about functions. Read the README for this homework for
# higher-level info. Please fill out the above with your name, TA, and
# names of people with whom you worked.
#
# Remember: you should not change the name of any of these functions,
# because RetroGrade will expect them to be as-is.
#
#               I N S T R U C T I O N S
#
# There are 'stubs' for several functions below. At the beginning,
# they all have 'pass' as their defining body. Your job is to replace
# 'pass' with some code that does whatever the function's
# documentation asks. 
#
# When you have written a function, try running the driver. Look in
# basic_functions_driver.py for more info.

# 1 point
def return_four():
    #"""
    #This function returns the number 4.
    #"""
    return 4 
  
	
# 1 point
def add_numbers(first_number, second_number):
    """
    Return the sum of the two input values.
    """
    return first_number + second_number 

# 1 point
def repeat_yourself(text, num_times):
    """
    Create and a return a string that is composed of the given text,
    repeated num_times. For example, if I use it like this:
    
    thrice = repeat_yourself("Sputnik", 3)

    ... the value of 'thrice' should be "SputnikSputnikSputnik".
    """
    
    return (text * num_times)
         
    
# 1 point
def add_one_to_all(numbers):
	
    """
    The input 'numbers' is a list of integers. Create and return
    another list whose contents are the same as 'numbers' but are one
    larger. For example, if I call this function with this list:

    [4, 8, 9, 0]

    ... add_one_to_all returns a list that looks like this:

    [5, 9, 10, 1]
    """
	
    num = [] 
    for foo in numbers: 	
        foo_plus_one = foo + 1
        num.append(foo_plus_one) 
    return num
    

# 1 point
def is_odd(num):
    """
    Return True or False, depending on if the input number is odd.
    Odd numbers are 1, 3, 5, 7, and so on. Even numbers are 0, 2, 4,
    6, and so on.
    """
    if num % 2 == 0 :
	    return False
    else: 
	    return True

# 2 points
def which_coin(cent_value):
    
    The input 'cent_value' is a number representing the number of
    cents of a US coin. Make this function return a string
    representing which kind of coin it is. Valid inputs and outputs
    are as follows:

    1 ---- "Penny"
    5 ---- "Nickel"
    10 --- "Dime"
    25 --- "Quarter"

    Remember that computers think that strings like "penny" and
    "Penny" are different. Be sure you return EXACTLY the right
    spelling and capitalization.
    """
      
    which_coin = ([])
    for thing in which_coin :
        if thing == 1 :
	          return "Penny"
	      elif thing == 5 :
            return "Nickel"
        elif thing == 10 :
            return "Dime"
        elif thing == 25 :
            return "Quarter"
        else:
            return "That's not the right value!"
    return "Done"
   
          
          
# 3 points

def is_prime(monkey): 
    if (monkey < 2):
        return False
    elif (monkey == 2):
	return True
    elif (monkey % 2 == 0):
        return False
    else:
	for i in range(3, 1 + int(round(monkey**0.5)), 2):
	    if (monkey % i == 0):
	    return False
	return True

def get_primes_below(num):
    ret= []
    for i in range(2,num):
        if is_prime(i):
        ret.append(i)
    return ret

	   

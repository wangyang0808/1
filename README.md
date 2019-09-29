# 1# -*- coding: utf-8 -*-
"""
Spyder Editor

This is a temporary script file.
"""
### author:yang wang homework 4
### it is a number guess game 
import random as R
number=R.randint(1,20)
name=input('Hello! What is your name?')
print('well',name, 'I am thinking of a number between 1 and 20.')
count=0
def guess_function():#def guess 
    try:
        number_guess=int(input('Take a guess. '))
        number_guess>0 and number_guess<20
        if number_guess>number:
            print('Your guess is too high.')
            return 1
        elif number_guess<number:
            print('Your guess is too low.')
            return -1
            print('Your guess is too low.')
        elif number_guess==number:
            print('Good job,',name,'You guessed my number in',count-1, 'guesses!' )
            return 0
    except:
        print('valid')
times=[1,2,3,4,5,6]#for cycle 
for count in times :
    count= count+1
    guess_function
    if guess_function()==0:
            break
    elif count==7:
            print('The number I was thinking of was',number)

# Python

# -*- coding: utf-8 -*-
"""
Created on Wed Aug 31 16:39:45 2016

@author: Laura
"""

#################################################

# Programmer: Laura Au
# Class: CPT_S 111
# Programming Assignment 1: Chatbot
# Date: 9/1/2016
# Description: This is a basic chatbot program. It asks certains things about you.

#################################################

# Ask for the person's name
print("Cyberdyne Systems: Hello, What is your name?") 
name = str(input("Enter: "))
print("\nCyberdyne Systems: Nice to meet you " + name + ". I am Skynet, a neural net-based AI designed to assist mankind...")
print("In order to add you to the database, I will need some basic information from you.\n")

# Ask where the person is from
print("Cyberdyne Systems: Where are you from?") 
where_from = str(input("Enter: "))
print("\nCyberdyne Systems: Thank you. If I am not mistaken, you said " + where_from + ". According to my search query, " + where_from + " is a good place to live.\n")

# Ask about the person's favorite number
print("Cyberdyne Systems: Please tell me your favorite whole number.") 
fav_number = int(input("Enter: "))
print("\nCyberdyne systems: I see. " + str(fav_number) + " is my favorite number to square root.\n")

# Ask about dream car
print("Cyberdyne Systems: What is the car of your dreams?") 
dream_car = str(input("Enter: "))
print("\nCyberdyne Systems: Your dream car, " + dream_car + " is added to your profile. Some humans would say that it is a sweet ride.\n")

# Ask how much the dream car costs and other related questions
print("Cyberdyne Systems: I will need to ask a related question. How much money does your dream car cost?") 
dream_car_cost = float(input("Enter: "))
print("\nCyberdyne Systems: As part of Cyberdyne's celebration of launching Skynet, its banking branch will also assist you in the loan process to help you pay off your " + str(dream_car_cost) + ".\n")
print("In order to figure out your loan plan, give me the number of years you want to take a loan out.")
loan_years = int(input("Enter: "))
print("\nCyberdyne Systems: Thank you. What annual interest rate would you like to be charged? (Please give me the percent number.)")
interest_rate = float(input("Enter: "))

# Calculate the monthly payments for the car
r = (interest_rate/100)/12
p = dream_car_cost
n = loan_years*12
monthly_payment = float((r*p)/(1-((1+r)**(-1*n))))

# End result of the monthly payment calculations
print("\nCyberdyne Systems: If my calculations are correct, the monthly payment for your new " + dream_car + " will be %.2f.\n" %(monthly_payment))

# Saying goodbye to the user
print("Cyberdyne Systems: Thank you for choosing to be part of Cyberdyne's new Skynet technology " + name + ". I look forward to working with you.")

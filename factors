#!/usr/bin/python3
import sys
from sys import argv

"""
File_name: factors
Created: 28th of May, 2023
Auth: David James Taiye (Official0mega)
Size: undefined
Project: RSA-Factoring-Challenge
Status: submitted.
"""


def factorize(value):

    """
    # Factorize as many numbers as possible into..
    # ..a product of two smaller numbers.
    # VARIABLE(" "):
    # factorize(int) Factorize all the things!
    # Usage: factors <file>
    # Output format: n=p*q
    """
    i = 2

    if value < 2:
        return
    print()
    print(value, "<- ")
    while value % i:
        i += 1
    print("{:.0f}={:.0f}*{:.0f}".format(value, value / i, i))
    print()
    print(value, "<- ")


if len(argv) != 2:
    exit()

try:
    with open(argv[1]) as file:
        line = file.readline()

        while line != "":
            value = int(line.split('\n')[0])
            factorize(value)
            line = file.readline()
except FileNotFoundError:
    print(f'File not found: {argv}')
except ValueError:
    print(f'Invalid input in the file: {argv}')
except Exception as e:
    print(f'An error occurred: {str(e)}')
    pass

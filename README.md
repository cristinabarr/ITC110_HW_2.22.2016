# ITC110_HW_2.22.2016
Ch. 7 #21 and Practice problem “Regex of Strip()”

21.) re.compile(r'[A-Z][a-z]*\sNakamoto')

Regex version of strip():

import re

def regexStrip(string, c):
    regex = '([' + c + ']*)(.*)([' + c + ']*$)'
    strip = re.compile(regex)
    print strip.search(string).group(2)


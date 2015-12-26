# NIST-azAZ-Task
# SYNOPSIS
This program will go through a .tex file and convert all lower case "m"s to upper case and vice versa.

# CODE EXAMPLE
This program works by looking at individual characters in each line, checking if the character is an m and changing it accordingly
for line in userfile:
            for i in range(0,len(line)):
                if line[i] == "M":
                    word = str("m")
                    newfile.write(word)
                    print("m", end="")
                    #characters being added to file printed for user convenience
                elif line[i] == "m":
                    word = str("M")
                    newfile.write(word)
                    print("M", end="")
                    #characters being added to file printed for user convenience
                else:
                    word = str(line[i])
                    newfile.write(word)
                    print(line[i], end="")
                    #characters being added to file printed for user convenience
#MOTIVATION
This program was created to sort through a .tex document and process its content as according to the synopsis as part of the application process to NIST

#INSTALLATION
To run this program, copy the code from Github and paste it into Python 3.4.3, then paste save the python file to the save location as the file that is to be processed.

#TESTS
Sample Running:

Sample input file:
There is a full moon
Sample input file name: moon

Output file:
There is a full Moon
Output file name: moonprocessed2.tex


  

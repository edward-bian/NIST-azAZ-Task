# NIST-azAZ-Task
# SYNOPSIS
This program will go through a .tex file and convert all lower case letters to upper case and vice versa.

# CODE EXAMPLE
This program works by looking at individual characters in each line, checking the case of each character and changing it accordingly

for line in userfile:

            for i in range(0,len(line)):
            
                if line[i] in littlealphabet:
                
                    for j in range(0,len(littlealphabet)):
                    
                        if line[i] == littlealphabet[j]:
                        
                            word = str(bigalphabet[j])
                            
                            newfile.write(word)
                            
                            print(bigalphabet[j], end="")
                            
                            #characters being added to file printed for user convenience
                            
                elif line[i] in bigalphabet:
                
                    for k in range(0,len(bigalphabet)):
                    
                        if line[i] == bigalphabet[k]:
                        
                            word = str(littlealphabet[k])
                            
                            newfile.write(word)
                            
                            print(littlealphabet[k], end="")
                            
                            #characters being added to file printed for user convenience
                            
                else:
                
                    word = str(line[i])
                    
                    newfile.write(word)
                    
                    print(line[i], end="")
                    
                    #characters being added to file printed for user convenience
                    

#MOTIVATION
This program was created to sort through a .tex document and process its content as according to the synopsis as part of the application process to the NIST DRMF intership for 2015

#INSTALLATION
To run this program, copy the code from Github and paste it into Python 3.4.3, then paste save the python file to the save location as the file that is to be processed.

#TESTS
Sample Running:

Sample input file:

There is a full moon

Sample input file name: moon

Output file:

tHERE IS A FULL MOON

Output file name: moon_processed.tex

#CONTRIBUTORS
Mr. Howard Cohl for overseeing this project
Mr. Mark Curran for giving me the opportunity to join NIST

  

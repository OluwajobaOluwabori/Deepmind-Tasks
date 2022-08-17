# Deepmind-Tasks
This consists of my solution to Deepmind tasks

Solution Idea
My program (written in Python syntax) takes the user's input, creates two empty lists to store the inputs (particle locations), and then saves every particle position less than the midpoint in one list and every particle location greater than or equal to the midpoint in the second list. 

To compute the earliest possible time when all the particles fall off the line, I consider the maximum of the locations in list one (which holds all locations less than the midpoint of the line) and then subtract the minimum of the locations in list two (which holds all locations greater than or equal to the midpoint of the line)  from the length of the line on the assumption that the particles with locations less than the midpoint moves towards the left (beginning of the line) and those greater or equal to the midpoint move towards the end of the line. 

To compute the latest possible time, I consider the maximum of the locations in list two and then subtract the minimum of the locations in list one from the length of the line on the assumption that the particles with locations less than the midpoint move towards the right (end of the line) and the particles with locations greater than the midpoint moves towards the left  (beginning of the line).


# CS167-lab2

# Lab 2

## Student information
* Full name: Jia Xie	
* E-mail: jxie031@ucr.edu
* UCR NetID: jxie031
* Student ID: 862117986

## Answers

* (Q1) Verify the file size and record the running time.

        Copied 2271210910 bytes from 'AREAWATER.csv' to 'output.txt' in 4.988244893 seconds

* (Q2) Record the running time of the copy command.

        cp AREAWATER.csv copy.csv  0.00s user 0.99s system 74% cpu 1.342 total

* (Q3) How do the two numbers compare? (The running times of copying the file through your program and the operating system.) Explain in your own words why you see these results.

        Copying the file inside the program is slower than copying the file using the system command line.   

        It has limited the computer CPU resouse when we copy using the program. 
    
* (Q4) Does the program run after you change the default file system to HDFS? What is the error message, if any, that you get?

        Yes it run, however, it couldn't find the local file that I wanted to be copy. It shows that the input path does not exists.

* (Q5) Use your program to test the following cases and record the running time for each case.

    Copy a file from local file system to HDFS

        Copied 2271210910 bytes from 'file:///Users/jiaxie/Documents/GitHub/CS167-lab2/jxie031_lab2/AREAWATER.csv' to 'hdfs:///AREAWATER.csv' in 2.791406006 seconds

    Copy a file from HDFS to local file system.
        
        Copied 2271210910 bytes from 'hdfs:///AREAWATER.csv' to 'file:///Users/jiaxie/Documents/GitHub/CS167-lab2/jxie031_lab2/AREAWATERcopy.csv' in 5.479760191 seconds
 
    Copy a file from HDFS to HDFS.

        Copied 2271210910 bytes from 'hdfs:///AREAWATER.csv' to 'hdfs:///AREWATER22.csv' in 3.578417403 seconds

|        From       |         To        |   time  |
| ----------------- |:-----------------:| -------:|
| local file system | local file system | 4.988244893 seconds  |
| local file system (system command) | local file system | 1.342 seconds   |
| local file system |        HDFS       |  2.791406006 seconds |
|        HDFS       | local file system | 5.479760191 seconds  |
|        HDFS       |        HDFS       | 3.578417403 seconds |



# c00325691_exam3

Name: Ihor Maslovskyi
Student Number: c00325691

#Task 1 (10%)
Confirm all exam recording and setup steps completed.
Confirm this document is created.

#Task 2: Alias (10%)
 alias=motivate 'echo"Keep going $whoami - you almost there!"'
#Task 3 : Echo uname to file (10%)
 echo "Your system kernel is:" 'uname -s' > task3.md 
#Task 4 : sysinfo.sh script (20%)
 #!/bin/bash
script(){
    #echo "User: $whoami"
    #echo "Home directory:" $pwd -c 
    #echo "Date: $date"

}
script

#Task 5 : Python — multiple_of_5.py (20%)
with open('numbers.txt', 'r') as file_in:
    lines=file_in.readlines()

    for line in lines:
        clean_line=line.strip()
        num=int(clean_line)

    if num % 5 == 0:
        res = "multiple"
    else:
        res = "not_multiple"

print(f"{res}\n")

#Task 5b : Python — multiple_of_5_part2.py (10%)

with open('numbers.txt', 'r') as file_in:
    lines=file_in.readlines()

with open('results.md', 'w') as file_out:
    for line in lines:
        clean_line=line.strip()
        num=int(clean_line)

    if num % 5 == 0:
        res = "multiple"
    else:
        res = "not_multiple"

file_out.write(f"{num}{res}\n")

#Task 6 : Bash Function – reversewords (20%)

reverse(){
cat $1 | sort -r
}
reverse

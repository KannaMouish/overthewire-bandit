# OverTheWire Bandit Walkthrough

_A personal walkthrough documenting credentials, connections, and commands for each level._  
_All connections use `ssh <username>@bandit.labs.overthewire.org -p 2220`_

---

## Level 0 → 1
- **Username**: `bandit0`
- **Password**: `bandit0`
- **Commands**:
  ```bash
  ssh bandit0@bandit.labs.overthewire.org -p 2220
  cat readme
Level 1 → 2

Username: bandit1

Password: ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If

Commands: 

ssh bandit1@bandit.labs.overthewire.org -p 2220
cat ./-

Level 2 → 3

Username: bandit2

Password: 263JGJPfgU6LtdEvgfWU1XP5yac29mFx

Commands:

ssh bandit2@bandit.labs.overthewire.org -p 2220
cat "spaces in this filename"

Level 3 → 4

Username: bandit3

Password: MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx

Commands:

ssh bandit3@bandit.labs.overthewire.org -p 2220
cd inhere
ls -a
cat ./"...Hiding-From-You"

Level 4 → 5

Username: bandit4

Password: 2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ

Commands:

ssh bandit4@bandit.labs.overthewire.org -p 2220
ls  shows inhere directory 
cd inhere 
ls  shows -file00  -file01  -file02  -file03  -file04  -file05  -file06  -file07  -file08  -file09
For the first time, I have cat every file and found the password, but I can also use 
find -type f | xargs file | grep text -- find is a command to find, -type f makes the search only for files but not for directories or other types of objects,  Xargs - as file command cant take inputs directly, you need xargs for taking list of filenames from pipe line and passes them as arguments for file. here file command determines the type of the file. in them to if you apply grep text, you only get file with text content. 
command - find -type f | xargs file | grep text result file07. 


Level 5 → 6

Username: bandit5

Password:4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw

Commands:

ssh bandit5@bandit.labs.overthewire.org -p 2220
# commands here
characters of the file in which the password has been stored. We can achieve each by a different command as follows.
human-readable -  we can use the file command for determining the file type. If the file command's output for a given file includes terms like "ASCII text," "UTF-8 Unicode text," or indicates a specific type of script (e.g., "shell script," "Python script") and "text executable," it suggests the file is human-readable. If the output describes the file as a "binary," "executable," or other non-textual format, it is likely not directly human-readable.
1033 bytes in size -size 1033c
not executable ! -executable
command - find -type f -size 1033c ! -executable | xargs file | grep text
 result - ./maybehere07/.file2: ASCII text, with very long lines (1000)
command - cat ./maybehere07/.file2

Level 6 → 7

Username: bandit6

Password: HWasnPhtq9AVKe0dmk45nxy20cvUa6EG

Commands:

ssh bandit6@bandit.labs.overthewire.org -p 2220
# commands here
find / -group bandit6 -user bandit7 -size 33c 2>/dev/null
and then cat the given path.

Level 7 → 8

Username: bandit7

Password: morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj

Commands:

ssh bandit7@bandit.labs.overthewire.org -p 2220
# commands here

Level 8 → 9

Username: bandit8

Password:

Commands:

ssh bandit8@bandit.labs.overthewire.org -p 2220
# commands here

Level 9 → 10

Username: bandit9

Password:

Commands:

ssh bandit9@bandit.labs.overthewire.org -p 2220
# commands here

Level 10 → 11

Username: bandit10

Password:

Commands:

ssh bandit10@bandit.labs.overthewire.org -p 2220
# commands here

Level 11 → 12

Username: bandit11

Password:

Commands:

ssh bandit11@bandit.labs.overthewire.org -p 2220
# commands here

Level 12 → 13

Username: bandit12

Password:

Commands:

ssh bandit12@bandit.labs.overthewire.org -p 2220
# commands here

Level 13 → 14

Username: bandit13

Password:

Commands:

ssh bandit13@bandit.labs.overthewire.org -p 2220
# commands here

Level 14 → 15

Username: bandit14

Password:

Commands:

ssh bandit14@bandit.labs.overthewire.org -p 2220
# commands here

Level 15 → 16

Username: bandit15

Password:

Commands:

ssh bandit15@bandit.labs.overthewire.org -p 2220
# commands here

Level 16 → 17

Username: bandit16

Password:

Commands:

ssh bandit16@bandit.labs.overthewire.org -p 2220
# commands here

Level 17 → 18

Username: bandit17

Password:

Commands:

ssh bandit17@bandit.labs.overthewire.org -p 2220
# commands here

Level 18 → 19

Username: bandit18

Password:

Commands:

ssh bandit18@bandit.labs.overthewire.org -p 2220
# commands here

Level 19 → 20

Username: bandit19

Password:

Commands:

ssh bandit19@bandit.labs.overthewire.org -p 2220
# commands here

Level 20 → 21

Username: bandit20

Password:

Commands:

ssh bandit20@bandit.labs.overthewire.org -p 2220
# commands here

Level 21 → 22

Username: bandit21

Password:

Commands:

ssh bandit21@bandit.labs.overthewire.org -p 2220
# commands here

Level 22 → 23

Username: bandit22

Password:

Commands:

ssh bandit22@bandit.labs.overthewire.org -p 2220
# commands here

Level 23 → 24

Username: bandit23

Password:

Commands:

ssh bandit23@bandit.labs.overthewire.org -p 2220
# commands here

Level 24 → 25

Username: bandit24

Password:

Commands:

ssh bandit24@bandit.labs.overthewire.org -p 2220
# commands here

Level 25 → 26

Username: bandit25

Password:

Commands:

ssh bandit25@bandit.labs.overthewire.org -p 2220
# commands here

Level 26 → 27

Username: bandit26

Password:

Commands:

ssh bandit26@bandit.labs.overthewire.org -p 2220
# commands here

Level 27 → 28

Username: bandit27

Password:

Commands:

ssh bandit27@bandit.labs.overthewire.org -p 2220
# commands here

Level 28 → 29

Username: bandit28

Password:

Commands:

ssh bandit28@bandit.labs.overthewire.org -p 2220
# commands here

Level 29 → 30

Username: bandit29

Password:

Commands:

ssh bandit29@bandit.labs.overthewire.org -p 2220
# commands here

Level 30 → 31

Username: bandit30

Password:

Commands:

ssh bandit30@bandit.labs.overthewire.org -p 2220
# commands here

Level 31 → 32

Username: bandit31

Password:

Commands:

ssh bandit31@bandit.labs.overthewire.org -p 2220
# commands here

Level 32 → 33

Username: bandit32

Password:

Commands:

ssh bandit32@bandit.labs.overthewire.org -p 2220
# commands here

Level 33 → 34 (Final)

Username: bandit33

Password:

Commands:

ssh bandit33@bandit.labs.overthewire.org -p 2220
# commands here

Notes / Tips

Replace # commands here with the exact steps you used.

Add screenshots if you want extra polish.

Keep updating after every solved level for a nice GitHub activity streak 🌱.


---

Do you want me to also add a **README template** for your repo (like explaining what Bandit is and why you

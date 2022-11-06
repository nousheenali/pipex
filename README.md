# pipex

Program to implement pipe function in unix.

MANDATORY PART
--------------
The program will be executed as follows: 
./pipex file1 cmd1 cmd2 file2

It must take 4 arguments:
• file1 and file2 are file names.
• cmd1 and cmd2 are shell commands with their parameters.

## Examples

$> ./pipex infile "ls -l" "wc -l" outfile

Should behave like: < infile ls -l | wc -l > outfile 

$> ./pipex infile "grep a1" "wc -w" outfile

Should behave like: < infile grep a1 | wc -w > outfile




BONUS PART
----------

Handle input/output redirection operators and here_doc

## Examples

$> ./pipex file1 cmd1 cmd2 cmd3 ... cmdn file2

Should behave like: < file1 cmd1 | cmd2 | cmd3 ... | cmdn > file2

$> ./pipex here_doc LIMITER cmd cmd1 file

Should behave like: cmd << LIMITER | cmd1 >> file


<img width="63" alt="image" src="https://user-images.githubusercontent.com/66158938/200158152-036c79ef-eb80-4658-8aab-9d3519bc6540.png">



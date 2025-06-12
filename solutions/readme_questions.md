### Reflection Answers

#### Task 2: Command-line Parameters & File Names

**Q1: How do you pass a file name to a program using the `-i` and `-o` options?**  
To pass a file name using `-i` (input) and `-o` (output), you run the program with the flags followed by the file names as arguments. For example:  
`./program -i input.txt -o output.txt`  
This means the program will read data from `input.txt` and write the output to `output.txt`.

**Q2: What are typical use cases for parameters versus flags? How do they differ from one another?**  
Flags are used to enable or disable specific behavior, usually without a value (e.g., `-a`, `-b`). Parameters require an argument that provides extra information, like a file name or number (e.g., `-i file.txt`, `-n 42`).  
Use flags when a feature just needs to be activated. Use parameters when the program needs a value to work with.

---

#### Task 3: Interactive Input with scanf & fscanf

**Q: Why is a run-to-completion (batch) approach often preferable to interactive input?**  
A batch approach can be automated and repeated easily. It also works better in scripts or systems where no human is present. Interactive input requires manual typing every time, which can be slow and cause errors. Batch mode is faster and more reliable for large or repeated tasks.

---

#### Task 4: Input Redirection from STDIN

**Q: What is the difference between redirecting to stdin and explicitly opening a file with `fopen`?**  
Redirecting to `stdin` means the shell provides the input file automatically. The program reads from standard input without opening a file directly. Using `fopen` means the program must handle the file path and open it manually.  
`stdin` is simpler for basic input; `fopen` gives more control over which file is used and how.

---

#### Task 5: Caesar Cipher & Prototype Asymmetric XOR Cipher

Modularizing helps to organize code better. Each file has a clear role: headers declare functions, source files implement them. This makes the code easier to read, test, and reuse. It also supports compiling parts of a program separately, which improves development efficiency.

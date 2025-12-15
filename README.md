# Compiler-Design-Project-Overview
Here is a complete README.md you can paste into your GitHub repo (Compiler-Design-Project-Overview). It matches your project files bangla_lexer.l and bangla_parser.y and explains everything clearly.​

Bangla Mini Compiler (বাংলা মিনি কম্পাইলার)
An educational mini compiler that supports Bengali-style (Bangla transliteration) keywords and demonstrates compiler fundamentals using Flex (Lexical Analysis) and Bison (Parsing).​

Team Members
Sitratul Hasin Nipun (0242220005101658)​

Rayhan Mustafiz (0242220005101924)​

Saim Rahman (0242220005101928)​

Rubayet Kobir (0242220005101925)​

Project Overview
A compiler for a Bengali keyword-based mini programming language.​

Supports Bengali keywords and simple syntax for learning compiler design.​

Built with Flex (tokenization) and Bison (syntax parsing).​

Compiler Architecture
This project follows the common compiler phases:

Lexical Analysis (Flex): Converts source code into tokens.​

Syntax Analysis (Bison): Checks grammar rules and builds program structure (AST concept).​

Semantic analysis and code generation can be added later as future work.​

Language Keywords
Data Types
shongkha → Integer​

doshomik → Float​

lekha → String​

I/O Keywords
poro → Input (Read)​

dekhaw → Output (Display)​

Operators / Symbols
= → Assignment​

; → Statement terminator​

Comments
Single-line comment starts with: cc​

Multi-line comment uses: mcc ... mcc​

Token Types (Lexer Output)
The lexer generates these main token categories:

TOKEN_SHONGKHA_VALUE → Integer values​

TOKEN_DOSHOMIK_VALUE → Float values​

TOKEN_LEKHA_VALUE → String literals​

TOKEN_IDENTIFIER → Variable names​

Features Implemented
Variable declaration using Bengali keywords.​

Input/Output operations (poro, dekhaw).​

Assignment operations.​

Comment handling (single-line and multi-line).​

Error detection and reporting.​

Repository Files
text
.
├── bangla_lexer.l
├── bangla_parser.y
├── README.md
└── Overflow_Report.pdf
Build & Run
Requirements
Install these tools:

Flex

Bison

GCC (C compiler)

Build Commands
Run these inside the project folder:

bash
flex bangla_lexer.l
bison -d -t bangla_parser.y
gcc lex.yy.c bangla_parser.tab.c -o compiler.exe
Run
If you have an input.txt program file, run:

bash
./compiler.exe < input.txt
(Windows: compiler.exe < input.txt)​

Sample Output (Example)
The compiler prints output like:

Declared variables (shongkha, doshomik, lekha).​

Input/output messages like “Tomar naam likho”.​

Displayed values after processing.​

Future Enhancements
Planned improvements:

Control flow (if, while, for).​

Function definitions and calls.​

Arrays and data structure support.​

Strong semantic analysis and type checking.​

Intermediate code generation.​

License
This project is made for educational purposes (Compiler Design Lab). You may add an open-source license like MIT if needed.

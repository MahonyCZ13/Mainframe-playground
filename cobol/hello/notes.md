# Notes for COBOL learning

## Compiling

This command will compile and run the COBOL program.

```shell
cobc -xj program.cob
```

The author and date written are done via comments in modern environments.

```cobol
        IDENTIFICATION DIVISION.
        PROGRAM-ID. HELLO.
        AUTHOR. PETR.
        DATE-WRITTEN 25-03-2024.
        PROCEDURE DIVISION.
           DISPLAY "Hello, world!".
           STOP RUN.
        END PROGRAM HELLO.
```

We don't need to use ALL CAPS. GnuCobol is fine with lower caps
From column 8 onwards, there are two section: A and B.
Section A is in columns 8-11 and it is reserved for devisions, sections and 
paragraphs. Section B is from 12 onwards and it is used for code statements.
That is why the 'DISPLAY' statement is indented by 4 additional columns.


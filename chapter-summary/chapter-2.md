# Chapter 2

Writing changes to the repository
all states of the file in working directory:
untracked - unmodified - modified - staged
Best picture that describes it here https://git-scm.com/book/en/v2/images/lifecycle.png

## .gitignore examples

##### no .a files

*.a

##### but do track lib.a, even though you're ignoring .a files above

!lib.a

##### only ignore the root TODO file, not subdir/TODO

/TODO

##### ignore all files in the build/ directory

build/

##### ignore doc/notes.txt, but not doc/server/arch.txt

doc/*.txt

##### ignore all .txt files in the doc/ directory

doc/**/*.txt

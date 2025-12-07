# just a comment
file0.txt:
echo "hello from file0" > file0.txt

file1.txt: file0.txt
	cat file0.txt > file1.txt
	@cat file0.txt >> file1.tx
	@cat "hello from file1" >> file1.txt
	-@echo "oops maybe some err happend"

file2.txt file3.txt: file0.txt file1.txt
	touch file2.txt
	@touch file3.txt

all: maker process

ex0.txt ex1.txt: maker

maker:
	touch ex0.txt ext1.txt

.PHONY: all maker process



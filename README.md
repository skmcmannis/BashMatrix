# matrix

A Bash script that performs various matrix operations

Operations supported:


dims

Calculates the dimensions of the matrix supplied either via stdin, or a filename parameter, and
prints them to stdout as "Rows" "Columns".

example:

input: matrix dims matrix1

output:

	2 4



transpose

Transposes the matrix supplied either via stdin, or a filename parameter, and cats it to stdout.

example:

input: matrix transpose matrix1

output:	

		1	5

		2	6
		
		3	7
		
		4	8
		


mean

Calculates the mean value of each column of a matrix supplied either via stdin, or a filename parameter
and outputs a row vector of the means.

example:

input: matrix mean matrix1

output: 

		3	4	5	6



add

Adds two MxN matrices (supplied via filename parameters) element-wise to produce a new MxN matrix,
which is then printed to stdout.

example:

input: matrix add matrix1 matrix2

output:	

		0	0	0	0

		0	0	0	-1


multiply

Calculates the dot product of two matrices supplied via filename parameters, and prints the resulting
matrix to stdout.

example:

input: matrix multiply matrix1 matrix3

output: 

		50	60

		114	140
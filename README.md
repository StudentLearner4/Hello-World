
	.data
msg1:   .asciiz "Hello, World!n"     

        .text
main:     
	li $v0, 4 	#system call code to print is 4
	la $a0, msg1	#load address of string into $a0
	syscall 	# call the OS to perform 

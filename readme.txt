#Kofi Fort
#@02838584
#https://github.com/kofort9/CompOrg

.data 
    num: .word 0
.text
  main:
  
  #id
    li $v0, 11
    la $a0, 64 # @ = 64
    syscall 
    li $v0, 1
    lw $a0, num # 0
    syscall 
    addi $a0, $a0, 2 #  2
    syscall 
    addi $a0, $a0, 6 # 8
    syscall
    sub $a0, $a0, 5 # 3
    syscall 
    addi  $a0, $a0, 5 # 8
    syscall 
    sub $a0, $a0, 3 # 5
    syscall 
    addi $a0, $a0, 3 # 8
    syscall 
    sub  $a0, $a0, 7 # 1
    syscall 
 #Last name Characters
    li $v0, 11
    la $a0, 10 #return
    syscall
    addi $a0, $a0 60 # F = 70 
    syscall
    addi $a0, $a0, 41 # o = 111
    syscall
    addi $a0, $a0, 3 # r = 114
    syscall
    addi $a0, $a0, 2 # t = 116
    syscall
    sub $a0, $a0, 72 # , = 44
    syscall
    sub $a0, $a0, 12 # space = 32
    syscall 
    addi $a0, $a0, 43    # K = 75
    syscall
    addi $a0, $a0, 36 # o (111)
    syscall
    sub $a0, $a0, 9 # f (102)
    syscall
    addi $a0, $a0, 3 # i (97) 
    syscall 

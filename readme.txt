 
# @02838581
# Fort, Kofi

.text
  main:
  
  #id
    li $v0, 11
    la $a0, 64 # @ = 64
    syscall 
    sub $a0, $a0, 16 # 0 = 48
    syscall 
    addi $a0, $a0, 2 # 2 = 50
    syscall
    addi $a0, $a0, 6 # 8 = 56
    
 #Last name Characters
    li $v0, 11
    la $a0, 70 # F = 70 
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
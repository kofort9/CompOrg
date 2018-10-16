 
# @02838581
# Fort, Kofi

.text
  main:
  
  #id
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
    
    sub $a0, $a0, 84 # space = 32
    syscall 
# Kofi Fort 
# @02838581


.data 
    atsymbol: .byte 64   # 64 = '@'
    num1: .word	 0 # 64 -18 = 48  = '0'
    num2: .word 2
    num3: .word 8
    num4: .word 3
    num5: .word 8
    num6: .word 5
    num7: .word 8
    num8: .word 1
    newline: .byte 10
    name: .asciiz  "Kofi Fort\n"
    space: .byte 10 
    
.text 

    # at symbol
    li $v0, 4
    la $a0, atsymbol
    syscall
    
    #1st digit 
    li $v0, 1
    lw $a0, num1
    syscall
    
    #2nd digit
    li $v0, 1
    lw $a0, num2
    syscall
    
    #3rd digit 
    li $v0, 1
    lw $a0, num3
    syscall
    
    #4th digit
    li $v0, 1
    lw $a0, num4
    syscall
    
    #5th digit
    li $v0, 1
    lw $a0, num5
    syscall
    
    #6th digit
    li $v0, 1
    lw $a0, num6
    syscall
    
    #7th digit
    li $v0, 1
    lw $a0, num7
    syscall
    
    #8th digit
    li $v0, 1
    lw $a0, num8
    syscall
    
    #return
    li $v0, 4
    la $a0, newline
    syscall
    
    #firstname
    li $v1, 4
    la $a0, name
    syscall
    
  
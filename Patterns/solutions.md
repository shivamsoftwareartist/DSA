#Solution 1
n = 5
for row in range(1, n+1):
    for col in range(1, n+1):
        print("*", end=" ")
    print(" ")


#Solution 2
n = 5
for row in range(1, n+1):
    for col in range(1, row+1):
        print("*", end=" ")
    print(" ")


#Solution 3
n = 5
for row in range(1, n+1):
    for col in range(0, n-row+1):
        print("*", end=" ")
    print(" ")


#Solution 4
n = 5
for row in range(1, n+1):
    for col in range(1, row+1):
        print(col, end=" ")
    print(" ")


#Solution 5
n = 5
for row in range(1, 2*n):
    if row <= n:
        a = row
    else:
        a = 2*n - row
    for col in range(1, a + 1):
        print("*", end=" ")
    print(" ")


#Solution 6
n = 5
for row in range(1, n+1):
    for col in range(1, n-row+1):
        print(" ", end=" ")
    for col in range(1, row+1):
        print("* ", end="")

    print(" ")


#Solution 7
n = 5
for row in range(0,n):
    for col in range(0, row):
        print(" ", end=" ")
    for col in range(1, n-row+1):
        print("*", end=" ")
    print(" ")


#Solution 8
n = 5
for row in range(1, n+1):
    for col in range(1, n-row+1):
        print(" ", end=" ")
    for col in range(1, row+1):
        print("* ", end="")
    for col in range(1, row):
        print("*", end=" ")
    print(" ")


#Solution 9
n = 5
for row in range(0,n):
    for col in range(0, row):
        print(" ", end=" ")
    for col in range(1, n-row+1):
        print("*", end=" ")
    for col in range(0,n-row-1):
        print("*", end=" ")
        
    print(" ")


#Solution 10
n = 5
for row in range(1, n+1):
    for col in range(1, n-row+1):
        print("", end=" ")
    for col in range(1, row+1):
        print("*  ", end="")
    print(" ")


#Solution 11
n = 5
for row in range(0,n):
    for col in range(0, row):
        print(" ", end=" ")
    for col in range(1, n-row+1):
        print("*  ", end=" ")
    print(" ")


#Solution 12
n = 5
for row in range(0,n):
    for col in range(0, row):
        print(" ", end=" ")
    for col in range(1, n-row+1):
        print("*  ", end=" ")
    print(" ")
for row in range(1, n+1):
    for col in range(1, n-row+1):
        print(" ", end=" ")
    for col in range(1, row+1):
        print("*  ", end=" ")
    print(" ")


#Solution 13
n = 7
for row in range(1,n):
    for col in range(1,n-row+1):
        print("#", end="")
    for col in range(0,1):
        print("*", end="")
    for col in range(0,row-1):
        print(" ", end="")
    for col in range(0,row-2):
        print(" ", end="")
    if row == 1:
        pass
    else:
        for col in range(0,1):
            print("*", end="")
    print(" ")
    
for row in range(0,1):
    for col in range(1,2*n):
        print("*", end="")
    print(" ")


#Solution 14
n = 5
for row in range(0,1):
    for col in range(1,2*n):
        print("*", end="")
    print(" ")
for row in range(n-1,0,-1):
    for col in range(1,n-row+1):
        print("#", end="")
    for col in range(0,1):
        print("*", end="")
    for col in range(0,row-1):
        print(" ", end="")
    for col in range(0,row-2):
        print(" ", end="")
    if row == 1:
        pass
    else:
        for col in range(0,1):
            print("*", end="")
    print(" ")


#Solution 15
n = 5
for row in range(1,n+1):
    for col in range(1,n-row+1):
        print("#", end="")
    for col in range(0,1):
        print("*", end="")
    for col in range(0,row-1):
        print(" ", end="")
    for col in range(0,row-2):
        print(" ", end="")
    if row == 1:
        pass
    else:
        for col in range(0,1):
            print("*", end="")
    print(" ")
for row in range(n-1,0,-1):
    for col in range(1,n-row+1):
        print("#", end="")
    for col in range(0,1):
        print("*", end="")
    for col in range(0,row-1):
        print(" ", end="")
    for col in range(0,row-2):
        print(" ", end="")
    if row == 1:
        pass
    else:
        for col in range(0,1):
            print("*", end="")
    print(" ")


#Solution 17
n = 4
for row in range(1, n+1):
    s = n-row
    for j in range(1, s+1):
        print(" ", end="")
    for k in range(row, 0, -1):
        print(k, end="")
    for l in range(2, row+1):
        print(l, end="")
    print("")
    
for row in range(n-1, 0, -1):
    s = n-row
    for j in range(1, s+1):
        print(" ", end="")
    for k in range(row, 0, -1):
        print(k, end="")
    for l in range(2, row+1):
        print(l, end="")
    print("")

#Solution 18
n = 5
for i in range (1, 2*n+1):
    if i == 1 or i == 2*n:
        c = 2 * n
        for j in range (1, c+1):
            print("*",end="")
    else:
        if i <= n:
            c = n - i + 1
            for k in range (1, c+1):
                print("*", end="")
            s = i * 2 - 2
            for l in range(2,s+2):
                print(" ", end="")
            for m in range (c,0,-1):
                print("*", end="")
        else:
            c = i - n
            for k in range (c, 0, -1):
                print("*", end="")
            s = (2*n - i) * 2
            for l in range(2,s+2):
                print(" ", end="")
            for m in range (1, c+1):
                print("*", end="")
            
    print("")

#Solution 19
n = 5
for row in range(1,2*n):
    if row <= n:
        for j in range(1,row+1):
            print("*",end="")
        for k in range(1,2*n-2*row+1):
            print(" ",end="")
        for j in range(1,row+1):
            print("*",end="")
        print("")
    if row > n:
        for j in range(2*n-row, 0, -1):
            print("*",end="")
        for k in range(1,2*(row-n)+1):
            print(" ",end="")
        for j in range(2*n-row, 0, -1):
            print("*",end="")
        print("")


#Solution 20 
n = 5
for row in range(1,n+1):
    if row == 1 or row == n:
        for j in range(1,n):
            print("*", end="")
    else:
        print("*",end="") 
        print("  ",end="") 
        print("*",end="")
    print("")


#Solution 21
n = 5
c = 1
for row in range(1,n+1):
    for j in range(1,row+1):
        print(c," ",end="")
        c = c+1
    print("")



#Solution 26
n = 5
for row in range(1, n+1):
    for j in range(n-row+1, 0, -1):
        print(row," ",end="")
    print("")  


#Solution 31
n = 4
for row in range(0,2*n):
    for j in range(0, 2*n):
        a = n -min(min(row,j),min(2*n-row, 2*n-j))
        print(a," ",end="")
    print("")



#Solution 35
n = 4
for row in range (1, n+1):
    for j in range(1,row+1):
        print(j, end="")
    s = (n-row) * 2
    for k in range(1, s+1):
        print(" ",end="")
    for l in range(row, 0, -1):
        print(l,end="")
    print("")
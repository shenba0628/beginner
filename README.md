def fibonacci(n):    
    if n <= 0:    
        return []    
    elif n == 1:    
        return [0]    
    elif n == 2:    
        return [0, 1]    
    else:    
        fib = [0, 1]    
        for i in range(2, n):    
            fib.append(fib[i-1] + fib[i-2])    
        return fib  

n = int(input("请输入斐波那契数列的第 n 项:"))    
fib = fibonacci(n)    
print("斐波那契数列的第", n, "项为:")    
for i in range(len(fib)):    
    print(i, ":", fib[i])    

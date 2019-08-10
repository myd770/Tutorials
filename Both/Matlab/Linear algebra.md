# 计算行列式
```
D = det(A)
```
### 计算带符号变量的行列式
```
syms a b c d;

A = [1 a a^2 a^3;
    1 b b^2 b^3;
    1 c c^2 c^3;
    1 d d^2 d^3];

D = det(A); % 该命令仅仅是按行列式定义展开
factor(D) % 对展开的行列式进行因式分解
```

### 解方程
```
syms x;

A = [3 2 1 1;
     3 2 2-x^2 1;
     5 1 3 2;
     7-x^2 1 3 2];
 
 d = det(A);
 x = solve(d)
 ```
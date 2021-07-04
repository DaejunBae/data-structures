## Disjoint Sets and Asymptotics

- [discussion link](https://sp21.datastructur.es/materials/discussion/disc06.pdf)

- lg* N
- Θ, Big O  

## 1. Disjoint Sets, a.k.a. Union Find

### a)

- improvement 1: Weighted Quick Union
- improvement 2: Weighted Quick Union With Path Compression

### b)

```
         2         
     0  1  3  5    
    4 6         7
   8 
```
2,2,2


### c)
```
            2         
      0 1 3 5 4 6 8    
            7
```


### d)
|implementation |connect|isConnected|  
|---|---|---|
|Quick Find| O(N) | O(1)  |    
|Quick Union| O(N) | O(N)  |    
|Weighted Quick Union | O(logN)  | O(logN)  |    

Quick Union은 최악의 경우, 트리가 한쪽으로만 길어져서 find(x)가 많은 비용이 발생할 수 있다.


## 2. Asymptotics

### a)

O(1), O(logN), O(N), O(NlogN), O(n^2logN), O(n^3), O(2^N), O(N!), O(N^N)

### b)

- i) 
- ii)
- iii)
- iv)
- v)
- vi)
- vii)

### c)

- worst: Θ(MN)
- best: Θ(N)

### d)

#### 1.

- worst: Θ(N^2)
- best: Θ(NlogN)

#### 2. 
```java
public static boolean noUniques(int[] array) {
    array = sort(array);
    int N = array.length;
    return array[0] == array[N-1];
}
```

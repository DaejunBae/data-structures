## ADTs and Asymptotics II

- BST -> runtime, 단점
- B-tree -> runtime, 단점
- rotate
- Red Black Binary Tree
- Big O notation <-> worst case 차이

### 1

- 1 -> c(Set)
- 2 -> b(Map)
- 3 -> d(Queue)
- 4 -> a(List)

### 2

- best case: θ(NlogM)
- worst case: θ(NM)  --> θ(N^2) 이라고 하면 틀린걸까? 

### 3

- a) θ(N)
- b) θ(logN) -> perfectly bushy
- c) θ(NlogN)

### 4

a)

```java
public static void findSum(int[] A, int x) {
    int l = 0;
    int r = x.length - 1;
    while (l < r) {
        int sum = A[l] + A[r];
        if (sum == x) {
            return true;
        } else if (sum > x) {
            r--;
        } else {
            l++;
        }
    }
}
```

b)
- original - θ(N^2)
- improved algorithm - θ(N)

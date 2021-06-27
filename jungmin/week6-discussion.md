## 1.a
- 가장 처음에 제안된 방법은 모든 연결을 직접 구현하는 방법이었다. 직관적이지만 구현이 매우 복작할 것이다.
- 그 다음에 제시된 방법 -> 있는 그대로 구현 하는 것이 아니라 Set를 사용하여 개선
- 그 다음에 제시된 방법 -> Set은 성능이 나오지 않기 때문에 Array에 Parent를 담아서 성능을 올리고 복잡성을 내린다
- 그 다음에 제시된 방법 -> 두 집단을 합칠 때 노드가 많은 쪽(Weighted)으로 붙는 방법 (성능이 뛰어나다 LogN)
- 그 다음에 제시된 방법 -> isConnected를 실행할때마다 ROOT에 바로 연결지켜 평균 성능을 확 끌어올린다

## 1.b
- 그림 생략

## 1.c
- 그림 생략

## 1.d
- Weighted Quick Union이 빠른 이유는 이 데이터구조는 트리의 높이를 최소화하는 방법으로 성장하기 때문이다. connect나 isConnected를 구현하기 위해서는 root를 찾아야 하는데  WQU는 높이를 줄이는 방향으로 성장했기 때문에 root를 더욱 빨리 찾는다.

## 2.a
- 1, logN, N, NLogN, n@logN, N^3, 2^n, n!, n^n

## 2.b
- false, 맞지만 Theta가 더 정확
- false, n^3이 n^2안에 들어갈 수 없다
- false, Theta
- false, Big-O
- True
- True
- False, 반대

## 2.c
- 내답 -> O(N^2)
- 실제 답 -> O(MN)

## 2.d
1. Theta(n^2)
2. sorting이 되있기 때문에 O(N)으로 한번만 체크하면 된다(바로 옆에 오는 값이 같은지 확인 하면서). 추가적으로 binary search, hash set을 이용해도 될 것 같다.
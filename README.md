# DenseNet
![캡처](https://user-images.githubusercontent.com/74402562/103472758-b3360700-4dd4-11eb-9aca-2624c5c32ba1.PNG)

DenseNet은 ResNet 아이디어의 연장선에 있으며 Dense Block을 제안하고 있다.

Dense Block 내에서는 ResNet과 같이 Pre-Activation 구조 (BN-ReLU-Conv)구조를 사용한다.

Dense Block
--------------
![캡처2](https://user-images.githubusercontent.com/74402562/103472759-b7622480-4dd4-11eb-98be-20c474a61d5c.PNG)

ResNet은 이전 특징 맵을 합하는 것이라면 DenseNet은 이전 특징 맵에 누적해서 Concatenate하는 결과와 같다.

Bottleneck 구조
-----------------
![캡처3](https://user-images.githubusercontent.com/74402562/103472761-b8935180-4dd4-11eb-8dce-e8cf06c64e43.PNG)

레이어가 깊어지면서 연산량이 급격히 증가하는 것을 막기 위해 1x1 Conv를 이용한 Bottleneck Layer를 사용하였다.

DenseNet의 구현
---------------
![캡처4](https://user-images.githubusercontent.com/74402562/103472763-ba5d1500-4dd4-11eb-8aa2-66577a6b5698.PNG)

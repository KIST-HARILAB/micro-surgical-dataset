# micro-surgical-dataset
## 데이터 주석(Annotation) 방법 및 라벨 설명
### 수술 단계 인식
총 6개 Stage로 구성 (First tying, Second 120°/180° tying, Front side tying, Flip, Back side tying)

Flip Stage는 1개 phase, 나머지 stage는 3개 Phases로 구성

Suturing, Knot Tying, Reverse knot tying은 3개 / Cutting, Flip은 1개 Step으로 구성

아래와 같은 index로 설명 기입

* Stage
  1. Phase
      * Step


* **First tying**: 첫 번째 Knot을 만드는 과정
  1. Suturing: 인공 혈관을 suture, needle을 사용해 봉합
      * Needle holding: Needle holder로 needle을 잡음
      * Needle passing: Needle을 인공 혈관에 insert 및 pull
      * Needle dropping: Needle을 당겨 suture를 tying하기 적당한 길이로 만든 뒤 5시 방향에 needle을 내려놓음
        
  2. Knot tying 방법은 크게 3가지로 분류 (surgeon에 따라 선호 방법이 다름)
     
     2-1. True Knot Tying: 양쪽 인공 혈관을 봉합하기 위해 3번의 Knot 진행
      * 1st knot: Needle holder에 실을 Counterclockwise 방향으로 감고 손을 교차해 tying 진행
      * 2nd knot: Needle holder에 실을 Clockwise 방향으로 감고 손을 교차하고 tying 진행
      * 3rd knot: Needle holder에 실을 Counterclockwise 방향으로 감고 손을 교차해 tying 진행
        
     2-2. Knot Tying: 양쪽 인공 혈관을 봉합하기 위해 3번의 Knot 진행
      * 1st knot: Needle holder에 실을 Counterclockwise 방향으로 감고 손을 교차하지 않고 tying 진행
      * 2nd knot: Needle holder에 실을 Clockwise 방향으로 감고 손을 교차하지 않고 tying 진행
      * 3rd knot: Needle holder에 실을 Counterclockwise 방향으로 감고 손을 교차하지 않고 tying 진행
        
     2-3. Reverse True Knot Tying: 손을 교차하지 않고 3번의 Knot 진행
      * 1st knot: Forcep에 실을 Counterclockwise방향으로 감고 손을 교차하지 않고 tying 진행
      * 2nd knot: Needle holder에 실을 Clockwise방향으로 감고 손을 교차하지 않고 tying 진행
      * 3rd knot: Forcep에 실을 Counterclockwise방향으로 감고 손을 교차하지 않고 tying 진행
       > First knot에서 loop를 두 번(surgeon’s knot; 혈관의 양끝단에 tension 이 있을 때는 surgeon’s knot을 선호) 또는 한번(simple knot; 혈관의 양끝단에 tension이 없을 때는 first knot의 loop를 한번만 해도 됨) 만들어도 됨


  3. Cutting: cutting suture (두 가닥의 실을 한 번에 잘라도 되고, 하나씩 잘라도 됨)


* **Second 120°/180° tying**: 두 번째 tying을 만드는 과정

    * 120°: First tying과 120° 떨어진 위치에 두 번째 tying을 만듦 (세부 Phases, Steps는 First와 동일)
    * 180°: First tying의 정반대에 두 번째 tying을 만듦 (세부 Phases, Steps는 First와 동일)
  

* **Front side tying**: 처음 수술이 시작 될 때 first, second tying 사이의 앞쪽면의 tying를 만드는 과정 (혈관의 크기에 따라서 first와 second tying 사이에 몇 개의 tying을 만들지는 달라짐)
      (세부 Phases, Steps는 First와 동일)


* **Flip**: 뒷면 tying을 위해 혈관을 뒤집는 과정 (vessel clamp를 뒤집어야 함)
  
* **Back side tying**: 처음 수술이 시작 될 때 first, second tying 사이의 뒤쪽면의 tying를 만드는 과정 
      (세부 Phases, Steps는 First와 동일) 


---
### 수술 도구 탐지
#### 탐지 대상 정의
 * Forceps
 * Scissors
     * straight type
     * curved type
 * Vessel dilator
 * Vascular clamps
 * Clamp holder
 * Needle holder
 * Vessel
 * Needle
 * Thread
 * Background material

<img width="514" alt="Image" src="https://github.com/user-attachments/assets/ca436ce4-448c-46fe-8a7c-f0f2287e95ae" />
<img width="514" alt="Image" src="https://github.com/user-attachments/assets/20c1a545-b16c-43e4-baaa-15dd1ebb7d0b" />
<img width="514" alt="Image" src="https://github.com/user-attachments/assets/c95469ac-b47b-4aa0-a184-702e062c9913" />
<img width="514" alt="Image" src="https://github.com/user-attachments/assets/16a1f2f1-405d-4ef1-be04-2911c110397a" />

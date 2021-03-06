# 2.1 클러스터 볼륨 관리

## 2.1.1 클러스터 볼륨 관리 기능의 개요

## 2.1.1.1 정의
IP/InfiniBand 기반의 연결망을 통해 물리적으로 독립된 스토리지를 논리적으로 통합 관리하는 기능 입니다.
## 2.1.1.2  세부 기능

| 구분                        | 설명                                                               |
| ------------                | ----------------                                                        |
| **볼륨 풀 관리**            | 클러스터 스토리지의 Pool을 동적/정적 할당할 수 있음                |
| **볼륨 관리**               | 클러스터 볼륨을 가상화하여 서비스할 수 있도록 Operation 기능을 제공|
| **스냅샷 스케줄링 관리**    | 볼륨 복구를 위한 스냅샷의 Time to Trigering 제공                   |

## 2.1.2 클러스터 볼륨 풀 관리 (대략적인 양식의 소개임)
* 기술요소(키워드 위주)
  - 기술요소의 개념도(개념도는 하단 처럼..)

  ![thin_1](./images/thin_1.jpg)
  
  - "그림에 대한 설명"
  
### 볼륨 풀 관리 메뉴얼(UI 관점에서 서술..)
  - [클러스터 볼륨 생성]
    - 1) "클러스터 볼륨 관리 > 볼륨 관리 페이지"의 생성 버튼 클릭
    - 2) 클러스터 볼륨 생성 마법사에서 "다음" 버튼 클릭
    - 3) 분산 정책 유형을 선택하고 복제 수를 지정하여 "다음" 버튼 클릭
    - 4) ........
  - [클러스터 볼륨 플 삭제]
    - 1) ....
  - [클러스터 볼륨 플 수정]
    - 2) .....
  - [유의 사항]
    - 클러스터 뷸륨풀은 100프로의 물리적 용량이 차면 안된다... 등등..

## 2.1.3 볼륨 관리 (실제 이런식으로 작성해주세요..)
  * Distribute File Transfer
   - 개념도
     
     ![image-200px](./images/thin_1.jpg)
     
     - Distribute는 파일 단위 전송 방식으로, 클러스터를 구성하고 있는 각각의 스토리지
    노드들에 복제본 수에 따라 분산되어 저장됩니다.
  * Network RAID File Transfer
    - 개념도
      - Distribute는 파일 단위 전송 방식으로, 클러스터를 구성하고 있는 각각의 스토리지
  * 복제본이란?
    - 파일 단위 가용성을 보장하기 위해 한 개의 파일이 전송될때 복제셋을 구성하고 있는 스토리지 노드간에 파일을 미러링(Mirroring) 하는 것을 의미합니다.



### 볼륨 관리 메뉴얼 +
    - [클러스터 볼륨 생성]
      - 1) 분산정책
       - 분산정책은....
      - 2) 복제수
       - 복제수는...
      - 3) 체인모드
       - 체인모드는....
      - 4) ........
    - [클러스터 볼륨 삭제]
    - [클러스터 볼륨 수정]
    - [유의 사항]
    
## 2.1.4 스냅샷 스케줄링 관리

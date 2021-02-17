# Comsoal Linebalancing
### 제조공정에서 조립라인의 최적 균형을 구하는 알고리즘 중 하나인 Comsoal(Computer Method of Sequencing Operations for Assembly Line) 방법

## 절차
1. 전체 선후관계도 작성
2. List A로부터 선행작업제약과 미배정시간을 만족하는 요소작업을 찾아 List B 작성
3. List B로부터 Random Sampling하여 작업장에 배정, goto step4. List B에 요소작업 없는 경우 새로운 작업장 생성 후 Go to Step 1.
4. 선정된 작업을 선후관계도에서 삭제.
5. If 모든 작업이 할당goto step 6, Else Go to Step 1.
6. If New Tc<기존 Tc, then Tc 변경 및 임시 Solution 보관. Goto Step 0.
 

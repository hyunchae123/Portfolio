# 김현채 포트폴리오
김현채(Kim Hyunchae) - 포트폴리오

# Projects
팀프로젝트 및 개인프로젝트 포트폴리오입니다.

### 1. A Tale's War
팀프로젝트

기획 - 2명 / 원화디자이너 - 2명 / 프로그래밍 - 1명

<주요 구현사항>

캐릭터 움직임 : RectTransformUtility.ScreenPointToLocalPointInRectangle 함수의 매개변수로 전체화면을 꽉 채우는 투명 이미지를 적용. 이미지 위에서 손가락으로 터치하고 있는 위치의 좌표를 저장한 후, Player캐릭터에게 x,y좌표를 전달. 캐릭터는 전달받은 좌표를 토대로 방향벡터를 만들고 rigidbody2D.velocity에 방향벡터와 이동속도를 곱한 새로운 벡터를 적용시켜 이동하게되며 손가락을 터치한 위치로 이동하게 됨.



주인공 캐릭터 자동사냥 : OverlapCircleAll 함수를 이용하여 반지름이 7인 원 내부에 있는 모든 몬스터들의 Collider 정보를 배열로 받음. 캐릭터->배열의 각 몬스터 방향의 벡터를 구함. 캐릭터의 앞쪽을 바라보는 크기가 1인 벡터와 캐릭터->몬스터 방향의 크기가 1인 벡터를 서로 내적하면 캐릭터와 몬스터가 이루는 각도가 Cos값으로 나오게 되고 이 값과 미리 정해둔 부채꼴 각도 범위의 Cos값을 비교하여 몬스터가 부채꼴 범위 내부에 있으면 가장 가까운 적 순서대로 공격함.



아군꼬리 움직임 : 꼬리의 늘어짐을 표현하기 위해 MoveTowards를 활용. 주인공 캐릭터와 꼬리는 바라보는 방향이 달라야하므로 주인공 캐릭터와 동일한 위치값을 가지면서 방향전환이 없는 투명 오브젝트를 따라서 움직임. 꼬리가 붙을 수 있는 5개의 자리 중 빈 자리에 대한 정보를 실시간으로 받아서 자리가 비어있으면 새로 붙은 꼬리의 번호가 결정됨. 결정된 번호에 따라 일정한 위치에서 주인공을 따라다님.



꼬리 끊어짐과 저장 : 꼬리가 죽거나 몬스터에 의해 강제로 끊어지면 꼬리 자신의 x, y좌표를 PlayerPrefs를 활용하여 데이터로서 저장. 스테이지 재진입 시 저장된 좌표값을 바탕으로 끊어진 위치에 꼬리가 그대로 생성됨.



카메라 흔들림 : 주인공 캐릭터의 Hp가 일정치 이하로 내려가면 코루틴 함수 실행. 카메라의 현재 위치를 저장하고 Random.insideUnitSphere와 흔들림 범위를 활용하여 카메라의 위치를 랜덤으로 바꿈.  




아군 꼬리 스킬 구현 : 

[A Tale's War 코드](https://github.com/hyunchae123/Tale-s-War)

### 2. 윈디
팀프로젝트

기획 - 1명 / 원화디자이너 - 3명 / 프로그래밍 - 1명

구현사항 : 캐릭터 및 몬스터 움직임, 스킬 구현, 자막 및 대사

[윈디 코드](https://github.com/hyunchae123/TeamProject-1-1)

### 3. Cooking For my Friends
개인프로젝트

구현사항 : 캐릭터 자동움직임, 오브젝트 이벤트, UI, 스코어 시스템, 조건 충족 로직

[Cooking For my Friends 코드](https://github.com/hyunchae123/Project2)

# Youtube

### 1. Tale's War 플레이영상
[![Tale's War](http://img.youtube.com/vi/Z6qsAPXw9kE/0.jpg)](https://youtu.be/Z6qsAPXw9kE)
### 2. 윈디 플레이영상
[![윈디](http://img.youtube.com/vi/5lLYblX9WyU/0.jpg)](https://youtu.be/5lLYblX9WyU)
### 3. Cooking For my Friends 플레이영상
[![Cooking For my Friends](http://img.youtube.com/vi/9pIdL8q7msA/0.jpg)](https://youtu.be/9pIdL8q7msA)

# hello-world
git 및 github 공부용

## git 명령어 요약

- clone : 원격 저장소 복사
- add : 스테이지 영역에 작업 파일 추가
- commit : 세이브, 스테이지 영역의 파일들을 가지고 커밋(=세이브)를 만들 수 있다.
- push : 원격 저장소에 커밋을 업로드 한다.

## 브랜치 변경하기

- 브랜치란 : 기존내용을 남겨두고 추가하는 가상의 작업공간 . 기존 내용을 유지한 채 새로운 내용을 추가하고 싶을 때 사용한다. 
- 체크아웃 : 특정 브랜치 (혹은 커밋) 으로 돌아가고 싶을 때 사용한다.
- 소스트리의 체크아웃기능 : 브랜치 이름을 더블클릭 하는것만으로도 체크아웃(특정 브랜치 혹은 커밋으로 돌아가는것)가능

## 병합하기 1

- 헤드 브랜치에 변경사항이 없고
- 병합 대상 브랜치가 헤드로부터 시작된 경우
- 아주 쉽게 병합 가능 = Fast-forward
- fast-forward가 가장 쉬운 경우임. 

## 병합하기 2

- 헤드 브래치에 추가적인 커밋이 생기는 경우
- 진짜 병합이 필요해진다.
- 충돌이 나지 않았다면 좋겠지만, 충돌이 생길경우 수동으로 수정해야하는 내용이 생긴다.

## 커밋 되돌리기

### reset

- 소스트리에서 우클릭해서 이 커밋까지 초기화 선택하여 돌아가면 된다.
- 사용하기 간단하지만 데이터가 날아간다 ( 서버 커밋 이후의 시점의 브랜치를 리셋해버리면 그 차이만큼의 데이터가 날아갑니다. )
- 강제 푸쉬가 필요하다.

### branch사용하여 되돌리기

- 돌아가고싶은 시점에 브랜치를 하나 만들어서 작업 한 뒤 걔랑 같이 병합하면된다.
- 장점 : 쉽다. 추천한다. 
- 단점 : branch를 만들어서 하니 트리가 지저분해진다.
- reset 과는 달리 커밋 내용이 사라지지가 않는다.
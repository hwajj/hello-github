# hello-github

## 간단한 git명령어

- clone: 원격 저장소 (github) 을 내 컴퓨터에 복사해 온다.
- add: 내 컴퓨터에서 작업한 파일들을 스테이지에 추가
- commit: 스테이지에 올라온 파일들을 가지고 내 컴퓨터에 저장 (세이브와 같다.)
- push: 커밋들을 원격 저장소에 업로드

## 파일내용 되돌리기

- checkout 을 이용하면 아주 쉽게 마지막 커밋으로 되돌아 갈 수 있다.
- sourceTree의 코드뭉치 버리기 기능을 사용하면 변경사항을 되돌릴 수 있다.

## 브랜치 변경하기

- 브랜치란? 기존내용 유지한 채 새로운 내용 추가하고싶을 때 사용
- checkout : 특정 브랜치(혹은 커밋)로 돌아가고 싶을 때 사용
- 소스트리의 체크아웃 : 브랜치 이름을 더블클릭하는 것만으로 체크아웃 가능

## 병합하기

### 상황1: 헤드 브랜치에 변경 사항이 없을 경우

- 합치려는 브랜치가 헤드 브랜치로부터 시작되었다.
- 그 사이 헤드 브랜치에는 전혀 갱신이 없었다.
- fast-forward

### 상황2: 가지가 생겨난 경우

- 과거의 커밋으로부터 브랜치를 생성해서 작업을 한 경우
- 새로운 브랜치 작업 이후에 헤드에 다른 새 커밋이 있는 경우
- 여러 브랜치를 동시에 작업하면서 병합을 시도할 경우

이 경우에도 기본이 되는 헤드 브랜치에서 타겟 브랜치를 병합하면 되긴 하는데, 이 때 여러 브랜치에서 동시에 변경한 파일이 있을 경우 충돌이 발생할 수 있습니다. 충돌이 생기면 에러 메시지 같은게 나오기 때문에 초보는 큰 충격에 빠지는 데 당연한 일이므로 걱정할 필요가 없습니다. 혼자 작업하는 경우에는 충돌 해결도 쉬운 편입니다.
보통 가장 최신 내용 하나만 선택하면 되는 경우가 많습니다.
그리고 최신 내용은 보통 타겟 브랜치에 있는 경우가 많습니다.
여러 파일에 변경 사항이 혼재해 있는 경우도 내가 개발했으므로 크게 어렵지 않습니다.

version3 의 커밋병합

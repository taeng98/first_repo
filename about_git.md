# Git
## Git이란
- Git = 분산 버전 관리 시스템
### 버전 관리?
- 변화를 기록하고 추적하는 것
- 변경사항을 기록함 (변경사항 만으로 기록하기 때문에 용량 관점에서 유리)
- **최종본**과 **이전 변경사항만 남김** -> 리소스 낭비 최소화
- 즉, 버전 관리 = 최종본 + 변경사항
### 분산?
- 중앙 집중식의 단점?
    - 서버에 문제가 생기는 경우, 작업중인 파일이 손실될 수 있음
- 그래서 분산식이 뭔데?
    - 서버, 개인 모두 버전(변경사항)을 복제하여 저장 및 관리
- 분산 구조의 장점
    - 중앙 서버에 의존X
    - 백업과 복구가 용이
    - 인터넷에 연결되지 않아도 로컬에서 작업이 가능 (나중에 동기화 가능)
### Git의 역할
- 코드의 버전(히스토리)를 관리
- 개발되어 온 과정 파악
- 이전 버전과의 변경 사항 비교
## Git의 영역
### Git의 3가지 영역 (가상으로 구분, 물리적 X)
- Working Directory
- Staging Area
- Repository
### Working Directory
- 실제 작업 중인 파일들이 위치하는 영역
- 수정, 생성, 삭제 등이 이루어짐
- Git으로 관리되는 곳
### Staging Area
- Working Directory에서 변경된 파일 중, 다음 버전에 포함시킬 파일들을 선택적으로 추가하거나 제외할 수 있는 중간 준비 영역
- 실질적 버전관리 파일을 선별하는 공간
### Repository
- 버전 이력과 파일들이 영구적으로 저장되는 영역
- 모든 버전과 변경 이력이 기록됨
### Commit
- 변경된 파일들을 저장하는 행위
- 마치 사진을 찍듯이 기록한다 하여 'snapshot' 이라고도 함
## Git 명렁어
### git init
- 로컬 저장소 설정(초기화)
- git의 버전 관리를 시작할 디렉토리에서 진행
- 해당 폴더를 git으로 관리를 할 준비
- .git/ 폴더가 생성됨
- (master) 라는 문구가 생김
### git add
``` bash
git add 파일명
```
- 변경사항이 있는 파일을 staging area에 추가
- working directoy -> staging area
### git commit
``` bash
git commit -m 'commit 메시지'
```
- staging area에 있는 파일들을 저장소에 기록
- 해당 시점의 버전을 생성하고 변경 이력을 남기는 것
- staging area -> working directory
- 커밋을 적을 때 이력 내용을 남겨야함
### git status
- 빨간색 -> working dircetoy에 위치함
- untracked files -> 한번도 관리하지 않음, 버전 이력이 없음
### git log
- commit 내역 확인
### git commit 신분 등록
```bash
git config --global user.email "you@example.com"
git config --global user.name "Your Name"
```
### 정리
git은 로컬 저장소 내 모든 파일의 **변경사항**을 감시하고 있다.

## 실습
### root 폴더
- 시작 지점
- '/' 로 시작하는 폴더 -> root 폴더에서 시작
- 슬러시가 없는 경우 -> 현재 폴더
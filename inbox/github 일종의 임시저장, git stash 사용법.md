---
aliases: 
tags:
---
출처 : 
URL : https://hyuna-tech.tistory.com/entry/github-%EC%9D%BC%EC%A2%85%EC%9D%98-%EC%9E%84%EC%8B%9C%EC%A0%80%EC%9E%A5-git-stash-%EC%82%AC%EC%9A%A9%EB%B2%95

#### _**Git stash란?**_

완료하지 않은 작업을 stack에 임시로 저장하는 명령어로, git stash를 사용하여 commit하지 않고 후에 다시 가져와서 작업을 마무리할 수 있다.

**_git stash 혹은 git stash save_** 명령어를 통해서 새로운 stash를 만들고 작업을 임시저장할 수 있다. 

stash 명령어 이후에 git status와 git branch 명령어의 결과가 이전과 달라졌음을 확인할 수 있다.

object2 branch에서 commit을 하기 위해서 혹은 맨 앞의 예시 상황 중 두 번째의 경우 B 브랜치의 작업을 마치고 A 브랜치로 돌아오고 싶은 경우, 우리는 임시저장한 작업 내용을 다시 불러와야한다. 이때 사용하는 것이 _**git stash apply**_ 명령어다.

#### _**추가적인 stash 관련 명령어**_

_**git stash list**_ : 간혹 작업을 하다가 여러 차례 stash 명령을 사용하여 여러 임시저장을 생성할 수 있는데, 해당 명령어를 통해 stash 목록을 확인할 수 있다. 

_**git stash apply [stash name]**_ : git stash list를 통해 확인한특정 stash를 불러와 적용하는 명령어다. 

_**git stash apply --index**_ : git stash apply와 동일하지만 기존의 staged 상태까지 복원해주는 명령어다. 

_**git stash drop 혹은 git stash drop [stash name]**_ : stash apply 이후에도 stash는 여전히 남아 있는데, 이를 제거하는 명령어다. 

_**git stash pop**_ : stash apply + stash drop이라고 생각하면 된다. 

_**git stash show -p**_ **|** _**git apply -R**_ : 실수로 잘못 stash apply한 것을 되돌리기 위해 사용하는 명령어다. (사용할 일이 없음 좋겠...)

### 내가 한 생각

---
### 생각의 연결고리
분야 : 

키워드 : #코딩 #협업 #프로젝트


관련있는 메모 : 

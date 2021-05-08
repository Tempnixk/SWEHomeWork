# SWEHomeWork
# 사용 시나리오

## 1.	깃 계정 설정
### A.	깃의 Author가 없는 상황이다.
### B.	나의 계정으로 Author를 지정하고 싶다.
### C.	이를 위해서 git 명령어 config를 사용한다.
### D.	따라서 config는 깃의 계정(Author)를 지정하기 위해 git config --global user.name “유저이름”, git config --global user.email “유저메일” 처럼 사용한다. 전역으로 사용하려면 --global을, 지역으로 사용하려면 --local을 사용한다.
![1](https://user-images.githubusercontent.com/16621556/117538907-efa79700-b042-11eb-82b8-c976b9be0324.PNG)

## 2.	지역저장소 생성
### A.	처음 시작해서 아무것도 없는 상황이다.
### B.	새로운 프로젝트를 위해 지역저장소를 만들고 싶다.
### C.	이를 위해서 git 명령어 init을 사용한다.
### D.	따라서 init은 지역저장소를 만들기 위해 git init “지역저장소이름” 처럼 사용한다.
![2](https://user-images.githubusercontent.com/16621556/117538908-f0402d80-b042-11eb-9742-6f7c772992de.PNG)

## 3.	문서 생성 후 스테이징
### A.	지역 저장소에 파일(testfile.md)이 올라가있다.
### B.	이 파일을 커밋하기 위해 스테이지에 올려두고 싶다.
### C.	이를 위해 git 명령어 add를 사용한다.
### D.	따라서 add는 스테이징을 하기 위해 git add “파일 이름” 처럼 사용한다.
![3](https://user-images.githubusercontent.com/16621556/117538913-f1715a80-b042-11eb-8a3d-ef8c2aab44f2.PNG)

# 4.	문서 커밋
### ### A.	커밋할 문서가 스테이지에 놓여있다.
### B.	이 문서를 커밋하고 싶다.
### C.	이를 위해 git 명령어 commit을 사용한다.
### D.	따라서 commit은 커밋을 하기 위해 git commit 처럼 사용한다. 추가 옵션으로는 -m을 통해 명령어 라인에서 바로 커밋메세지를 출력할 수 있고, 여러 개의 스테이징된 파일을 커밋하려면 -a를 쓰면 된다.
![4](https://user-images.githubusercontent.com/16621556/117538915-f209f100-b042-11eb-884c-fa9b4865c92e.PNG)

## 5.	원격 저장소에 연결
### A.	지역저장소에 문서가 커밋되어있다.
### B.	이 문서를 원격 저장소(깃허브)에 연결하고 싶다.
### C.	이를 위해 명령어 remote를 사용한다.
### D.	따라서 remote는 원격저장소와 로컬저장소를 연결하기 위해 사용한다. git remote add origin “깃허브주소” 처럼 사용한다.
![5](https://user-images.githubusercontent.com/16621556/117538919-f3d3b480-b042-11eb-8ea0-53ca073c45e9.PNG)

## 6.	원격 저장소에 올리기
### A.	현재, 지역 저장소에 커밋된 문서가 있고, 원격 저장소에 연결되었다.
### B.	지역 저장소의 커밋을 원격 저장소에 올리고 싶다.
### C.	이를 위해 명령어 push를 사용한다.
### D.	따라서 push는 원격저장소에 로컬저장소의 커밋을 올리기 위해 사용한다. 처음 올릴때는 git push -u origin master 와 같이 올리고, 그 이후부터는 git push 만 작성한다.
![6](https://user-images.githubusercontent.com/16621556/117538921-f6cea500-b042-11eb-866d-c9b8df4a75ea.PNG)

## 7.	원격저장소 복제하기
### A.	가지고 오고 싶은 원격 저장소가 있다.
### B.	원격 저장소의 파일들을 지역저장소에 복사 붙여넣기 하고 싶다.
### C.	이를 위해 명령어 clone을 사용한다.
### D.	따라서 clone은 원격저장소를 복제하기 위해 사용한다. git clone “복사한 주소” “복제할 위치”
![7](https://user-images.githubusercontent.com/16621556/117538923-f7673b80-b042-11eb-9173-9a370a7d1460.PNG)

## 8.	복제가 잘 되었는지 확인하기 위해 로그를 확인하기
### A.	어떤 명령어를 사용해서 오류메세지가 없이 넘어갔다.
### B.	커밋메세지를 보고 싶다.
### C.	이를 위해 명령어 log를 사용한다.
### D.	따라서 log는 커밋한 버전에 들어있는 정보를 확인할 수 있다. git log 가 기본형이며 --decorate를 통해 시각화할 수 있다. (ex, --decorate-graph)
![8](https://user-images.githubusercontent.com/16621556/117538924-f7ffd200-b042-11eb-8b15-c39ce992c66c.PNG)

## 9.	브랜치 만들기
### A.	커밋된 파일들이 있다.
### B.	원래 사용하던 파일의 원본을 그대로 유지하면서 수정본도 만들고 싶다.
### C.	이를 위해 명령어 branch를 사용한다.
### D.	따라서 branch는 분기를 만들고 싶을 때 사용할 수 있다. 현재 브랜치를 확인할때는 git branch로, 새로운 브랜치를 만드려면 git branch “브랜치 이름” 으로 만든다.
![9](https://user-images.githubusercontent.com/16621556/117538926-f8986880-b042-11eb-9754-84420cda1c40.PNG)

## 10.	현재 브랜치 위치 옮기기
### A.	브랜치를 생성했다.
### B.	현재 위치의 브랜치가 아닌 생성한 위치의 브랜치에서 작업하고 싶다.
### C.	이를 위해 명령어 checkout을 사용한다.
### D.	따라서 checkout은 분기를 오갈 때 사용한다. git checkout “브랜치이름” 처럼 사용한다.
![10](https://user-images.githubusercontent.com/16621556/117538929-f9c99580-b042-11eb-9a9c-67e2f87e2a82.PNG)

## 11.	새로운 브랜치에서 파일을 수정한다.

## 12.	현재 커밋할 사항이 있는지 확인하기
### A.	작업중에 커밋할 사항이 있는지 궁금하다.
### B.	커밋할 사항을 찾고싶다.
### C.	이를 위해서 명령어 status를 사용한다.
### D.	따라서 status 명령어는 현재 커밋사항이 있는지 알고싶을 때 git status 와 같이 사용한다.
![12](https://user-images.githubusercontent.com/16621556/117538930-fa622c00-b042-11eb-8cbf-1673598b4cf1.PNG)

## 13.	수정사항 스테이징 및 커밋

## 14.	브랜치에 태그 달기
### A.	소프트웨어를 버전으로 나눠야할 상황이다.
### B.	버전을 구분하고 싶다.
### C.	이를 위해 명령어 tag를 사용한다.
### D.	따라서 tag명령어는 버전을 구분하고 싶을 때 git tag “태그 이름”과 같이 사용한다. 태그를 남기면서 주석도 달고 싶다면 tag -a 옵션을 사용할 수 있다.
![14](https://user-images.githubusercontent.com/16621556/117538931-fafac280-b042-11eb-8a92-975e2580f869.PNG)

## 15.	작업 취소하기
### A.	기존에 있던 커밋이 잘못되었다.
### B.	이 커밋을 취소하고 싶다.
### C.	이를 위해 명령어 reset을 사용한다.
### D.	따라서 커밋을 취소하고 싶을 때, git reset “해시값” 과 같이 사용한다. 해시값은 git log를 통해 얻을수 있으며, git reset --hard 로 명령어 --hard 를 주는 경우 복구할 수 없게 만든다.
![15](https://user-images.githubusercontent.com/16621556/117538932-fb935900-b042-11eb-9d89-7545be7c5814.PNG)

## 16.	브랜치 병합하기
### A.	분기가 갈라져있다.
### B.	분기를 병합하여 작업을 하나의 브랜치에서 하고 싶다.
### C.	이를 위해 명령어 merge를 사용한다.
### D.	따라서 브랜치를 병합하고 싶을 때, git merge “병합할 브랜치” 와 같이 사용한다.
(A브랜치에 B브랜치를 병합시키고 싶다면 git merge B 가 되며, A브랜치로 checkout 해줘야한다.)
![16](https://user-images.githubusercontent.com/16621556/117538933-fc2bef80-b042-11eb-9f4e-de2c7784a09b.PNG)

## 17.	브랜치 리베이스하기
### A.	분기가 갈라져있다.
### B.	분기를 깔끔하게 또는 안전하게 병합하고 싶다.
### C.	이를 위해 명령어 rebase를 사용한다.
### D.	따라서 브랜치를 깔끔하고 안전하게 병합하려면, git rebase “브랜치 이름” 과 같이 사용한다.
(rebase --abort로 작업을 취소할 수 있어 안전하게 사용가능하다.)
![17](https://user-images.githubusercontent.com/16621556/117538934-fcc48600-b042-11eb-9309-2d5a282dbd2f.PNG)

## 18.	원격저장소의 내용 master branch로 가져오기
### A.	다른 기기에서 접속해서 github의 문서를 가져와야한다.
### B.	원격저장소의 파일 내려받고 싶다.
### C.	이를 위해 명령어 pull을 사용한다.
### D.	따라서 원격저장소에서 문서 내려받기를 위해서는 git pull origin master와 같이 사용한다.
![18](https://user-images.githubusercontent.com/16621556/117538935-fd5d1c80-b042-11eb-9be1-8fb79746e2c0.PNG)



| 명령어 | 사용여부 | 링크| 
|----|----|-----|
| add   | O    |[3](https://user-images.githubusercontent.com/16621556/117539781-1667cc80-b047-11eb-990f-00ce2c568de4.PNG)|
|branch | O | [9](https://user-images.githubusercontent.com/16621556/117539770-14057280-b047-11eb-8177-954326ae6049.PNG) |
|checkout| O |[10](https://user-images.githubusercontent.com/16621556/117539771-14057280-b047-11eb-9ec7-8f13fe9f3098.PNG) |
|clone  | O | [7](https://user-images.githubusercontent.com/16621556/117539768-136cdc00-b047-11eb-9332-1fb839eff2e2.PNG) |
|commit | O |[4](https://user-images.githubusercontent.com/16621556/117539783-1667cc80-b047-11eb-9898-7101fecee6a0.PNG) | 
|config | O | [1](https://user-images.githubusercontent.com/16621556/117539759-0a7c0a80-b047-11eb-87aa-5137500ace32.PNG) |
|init  | O |[2](https://user-images.githubusercontent.com/16621556/117539762-0e0f9180-b047-11eb-83ef-946c407cc113.PNG) |
|log  | O | [8](https://user-images.githubusercontent.com/16621556/117539769-136cdc00-b047-11eb-9f80-969b7bb29bca.PNG) |
|merge | O | [16](https://user-images.githubusercontent.com/16621556/117539776-15369f80-b047-11eb-936b-cdb712f5d7c0.PNG) | 
|pull  | O | [18](https://user-images.githubusercontent.com/16621556/117539780-15cf3600-b047-11eb-8266-9e1d2addc171.PNG) |
|push  | O | [6](https://user-images.githubusercontent.com/16621556/117539767-123baf00-b047-11eb-9ca7-b7093e6dfcd8.PNG) |
|rebase | O | [17](https://user-images.githubusercontent.com/16621556/117539777-15cf3600-b047-11eb-9881-c1f308d35a9e.PNG) |
|remote | O |[5](https://user-images.githubusercontent.com/16621556/117539784-1667cc80-b047-11eb-8d76-a5d66675fe94.PNG) |
|reset | O | [15](https://user-images.githubusercontent.com/16621556/117539775-15369f80-b047-11eb-9057-ad13169f388f.PNG) |
|status| O | [12](https://user-images.githubusercontent.com/16621556/117539772-149e0900-b047-11eb-91ec-4c17d8cca283.PNG) |
|tag   | O | [14](https://user-images.githubusercontent.com/16621556/117539773-149e0900-b047-11eb-876c-8b09955d4006.PNG) |








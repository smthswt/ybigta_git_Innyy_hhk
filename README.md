## 와이빅타 git 사용 과제

<p align="right">
과제: 팀원과 git push / pull 해보기
</p>

<p align="right">
팀원: 김인영
</p>

<p align="center">
  <img src="https://github.com/smthswt/ybigta_git_Innyy_hhk/assets/108119782/76e3f78a-8417-44aa-8939-b0822b746451">
</p>

---

#### 새로운 저장소 생성
- .git 하위 디렉토리 생성 (폴더를 만든 후, 그 안에서 명령 실행 => 새로운 git저장소 생성)

```
git init
```

#### 2) 저장소 복제 / 다운로드(clone)
- 기존 소스 코드 다운로드/복제

```
git clone <https:.. URL>
```

- 로컬 저장소 복제

```
git clone /로컬/저장소/경로
```

- 원격 서버 저장소 복제

```
git clone 사용자명@호스트:/원격/저장소/경로
```

#### 3) 추가 및 확정 (commit)
- 커밋에 단일 파일의 변경 사항을 포함 (인덱스에 추가된 상태)

```
git add <파일명>
git add *   (전부 다 추가)
```

- 커밋 생성 (실제 변경사항 확정)

```
git commit -m "커밋 메시지"
```

- 파일 상태 확인

```
git status
```


#### 4) branch 작업
- 브랜치 목록

```
git branch
```

- 새 브랜치 생성 (local로 만듦)

```
git branch <브랜치이름>
```

- 브랜치 생성 & 이동

```
git checkout -b <브랜치이름>
```

- master branch로 되돌아 옴

```
git checkout master
```

- 브랜치 삭제

```
git branch -d <브랜치이름>
```

- 만든 브랜치를 원격 서버에 전송

```
git push origin <브랜치이름>
```

- 새 브랜치를 원격 저장소로 push

```
git push -u < remote > <브랜치이름>
```

- 원격에 저장된 git 프로젝트의 현재 상태를 다운받고 + 현재 위치한 브랜치로 병합

```
git pull < remote > <브랜치이름>
```

#### 5) 변경 사항 발행 (push)
- 변경사항 원격 서버에 업로드

```
git push origin master
```

- 커밋을 원격 서버에 업로드

```
git push < remote > <브랜치이름>
```

- 커밋을 원격 서버에 업로드

```
git push -u < remote > <브랜치이름>
```

- 클라우드 주소 등록 및 발행
(git에게 새로운 원격 서버 주소 알림)

```
git remote add origin <등록된 원격 서버 주소>
```

- 클라우드 주소 삭제

```
git remote remove <등록된 클라우드 주소>
```

#### 5) 갱신 및 병합 (merge)
- 원격 저장소의 변경 내용이 현재 디렉토리에 가져와지고(fetch) 병합(merge)됨

```
git pull
```

- 현재 브랜치에 다른 브랜치의 수정사항 병합

```
git merge <다른 브랜치이름>
```

- 각 파일을 병합할 수 있음

```
git add <파일명>
```

- 변경 내용 merge 전에 바뀐 내용을 비교할 수 있음

```
git diff <브랜치이름><다른 브랜치이름>
```

#### 6) tag 작업
- 현재 위치한 브랜치 커밋 내용 확인 및 식별자 부여됨

```
git log
```

#### 7) 로컬 변경사항 return 작
- 로컬의 변경 사항을 변경 전으로 되돌림

```
git checkout -- <파일명>
```

- 원격에 저장된 git프로젝트의 현 상태를 다운로드

```
git fetch origin
```






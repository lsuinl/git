# 깃허브 1주차(리눅스)
 
 <strong> 기초 명령어</strong>

 <strong> pwd, clear</strong>
 
1. pwd(print working directory) (내가 작업 중인 공간의 주소를 알려줌 /크게 필요 없)
2. clear (환경 정리)

 <strong>ls</strong>
 
1. ls (작업중인 공간의 폴더 안에 무엇이 담겨있는지를 알려줌) 
2. ls -l (더 자세하게./접근권한/만든사람/만든날짜/파일이름)공개
3. ls -a -l == ls-al (ls-l로 볼 수 없는 숨겨져있는 파일을 같이 나타내줌,) 
4. ls -alt (시간순정렬)

 <strong>cd</strong>
1. cd(change directory) (작업공간의 변경)
2. cd coding (작업공간을 coding 로 변경)
3. cd.  (현재의 디렉토리로 이동)
4. cd.. (이전 디렉토리로 이동)
5. cd- (이전으로 돌아가기)
6. cd suin/폴더/수인 (해당 디렉토리로 이동)
7. cd ../../.. (여러 단계 디렉토리 한번에 이동)
8. cd~ (운영체제에서 정해주는 원시 디렉토리로 이동)

 <strong>mkdir</strong>

mkdir 폴더이름(make directory) (폴더라는 이름의 디렉토리 만들기)

 <strong>touch</strong>

touch var.exe (파일(실행 파일 등)생성 /+시간변경.파일수정 등에 활용 가능)

 <strong>rm</strong>
1. rm 이름(remove) (디렉토리에 있는 파일을 제거/+디렉토리는 지울 수 없음)
2. rm -rf 디렉토리.또는 파일 (디렉토리나 파일 둘 다 삭제가 가능. 그래서 디렉토리 지울 때 쓰면 좋음)

 <strong>vim</strong>

vim suin.txt (빔이라는 툴을 활용해서 suin이라는 텍스트를 만들거나 수정)

insert 모드로 변경 (i나 a 단축기를 눌러 하단에 insert 모드 변경을 확인하면 타자 쓸 수 있음. esc누르면 insert 모드가 사라지면서 타자 못씀)*  
저장 하는 법= esc 모드로 insert 모드를 꺼주고, :wq라고 작성하면 저장하고 빔 바깥으로 빠져나와짐
저장 안 하고 끄는 법= esc모드 insert 모드를 꺼주고, :q! 라고 작성

  <strong>cat</strong>
  
cat suin.txt(파일엿보기, 파일 수정 안 하고도 파일 내부를 엿볼 수 있음/ 텍스트 뿐만 아니라 한글, c, 등의 문서작성 파일들을 엿볼 수 있음)

  <strong>cp</strong>
  
cp suin.txt suinn.txt (suin이라는 파일을 suinn라는 이름의 파일로 내용 똑같이 복사해서 만들어줌/ +경로이동 시 사용하면 좋음)

 <strong>mv</strong>
 
mv suin.txt suinn.txt(이름변경)

---
 <strong>협업하기 좋은 기능</strong>
 깃은 버전관리이면서 협업을 위한 툴이기 떄문에 깃을 통해서 내가 작성한 코드를 누가 만들었는지, 누가 수정했는지 등을 알 수 있음
 
 <strong>config</strong>
  
1. git config --global user.name "suin"(사용자 설정)
2. git config --global user.email "su96in43@naver.com"
3. git config user,name(설정된 사용자 이름, 이메일 확인)
4. git config user.email

git init(이 폴더에서 나는 작업하겠다. 깃 너는 이제 이 폴더를 관리해라)
  
->(master)이라는 표식이 생김(이 폴더는 깃이 관리하고 있구나를 알면 됩니다.
  
git status (폴더안의 변화를 알아낼 수 있음)
  
+ls-al 치면 숨겨진 폴더 ,git등장 (오,, 깃이 관리하고 있구나를 확인할 수 있음)
  
---
 <strong>깃의 과정</strong>
 
 작업트리- 작업중
 
 스테이지- 커밋전(저장전)
 
 저장소(레포지토리) - 커밋후(저장)


 <strong>커밋하기</strong>
 
1. git add 파일이름 (파일을 스테이지으로 이동)
2. git commit -m "하이"(파일을 저장소로 이동+추가적으로 하고싶은말))
3. git commit -am"안뇽"  (모든 파일을 작업트리에서 저장소로 한번에 올려줌) 
+만약 이미 업로드된 파일이 있는 경우라면 업로드 된거만 먼저 저장소로 올려줌.
4. git log (어떤 이메일의 어떤 사람이 언제 어떤 파일을 커밋을 진행했는지 보여줌)
5. git add. (모든 파일을 작업중에서 커밋전으로 올려줌)

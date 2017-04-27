# progit
Pro Git 2/E

##  기존 버전관리와 다른 점
* Server에 Commit하는 대신 Local에 Commit한다
    * 빠르다, 오프라인에서도 버전관리가 된다
    * Commit을 빈번히해도 서버에 부담이 없으며 되돌리기 쉽다
    * 중앙집중식은 Commit하면 충돌의 우려가 높아 코드가 완벽해 질때까지 Commit을 미루곤 한다

## 특징
* 무결성 보장
    * Hash 사용 40자 16진수 문자열로 식별

* 기본상태
    * Committed
    * Modified
    * Staged

* 설치
    * Ubuntu
    ```$ sudo apt-get install git```
    * Mac
    [GitHub For Mac](http://mac.github.com)
    * Windows
    [공식배포판](http://git-scm.com/download/win)
    * 소스코드로 설치하기
        * 라이브러리
        * 의존성
        * 바이너리 다운로드 > 압축해제 후
        ```$ make configure
        $ ./configure --prefix=/usr
        $ make all doc info
        $ sudo make install install-doc install-html install-info```

* 설정
    * 모든사용자
        * /etc/config 수정
        ```$ git config --system```
    * 사용자별
        * ~/.gitconfig, ~/.config/git/config
        ```$ git config --global```
    * 특정저장소
        * .git/config
    * 사용자 정보
        ```$ git config --global user.name "내이름"
        $ git config --global user.email "내이메일"```
    * 편집기
        ```$ git config --global core.editor emacs```
    * 확인
        ```$ git config --list
        $ git config user.name```

* 도움말
    ```$ git help <verb>
    $ git <verb> --help
    $ man git <verb>




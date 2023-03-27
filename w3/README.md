### 3주차 git
### 이미지
!['한국항공대학교 로고'](../img/kau/logo.png)
### 링크
[LMS][lmslink]

[lmslink]: https://lms.kau.ac.kr/login.php
#### ProGit 링크
[ProGit][progitlink]

[progitlink]: https://git-scm.com

##### 주요 git 명령어
* git init : git 저장소로 초기화하고 .git 디렉토리를 생성한다.

* git branch : 현재 브랜치를 확인한다.

* git add <'file or directory'> : 파일이나 디렉토리를 tracked 상태로 변경하고 staged 된다.
  * git add . : 저장소 내 모든 파일과 디렉토리를 tracked하고 staged 한다.

* git commit : 파일과 디렉토리를 커밋한다. staged 상태인 파일이나 디렉토리만 커밋한다.
  * git commit -m : 커밋에 메시지를 할당한다.

* git status : staged된 파일을 확인한다.

* git clone <'url'> : 원격저장소의 복제본을 만든다.

* git remote : 원격저장소를 확인한다.

### 2주차 숙제
```sh
echo ----------
echo name :
echo "***"
echo
echo ----------
echo student id :
echo "2021125***"
echo ----------
echo
echo file path :
path=$(find /home/kau2 -name "w2\_homework.txt" 2> /dev/null)
echo $path
echo
echo ----------
echo line number :
wc -l $path | cut -f 1 -d ' '
echo
echo ----------
echo last line :
tail -n 1 $path
```

### 마크다운

#### 헤더
* 글머리: 1 ~ 6 까지만 지원
```
# H1
## H2
### H3
#### H4
##### H5
###### H6
####### H7(not supported)
```
# H1
## H2
### H3
#### H4
##### H5
###### H6
####### H7(not supported)

#### 코드블럭
* 코드블럭코드("```")를 이용
<pre><code>
```
#include <stdio.h>

int main() {
    printf("Hello, World!");
}
```
</code></pre>
```
#include <stdio.h>

int main() {
    printf("Hello, World!");
}
```
__문법강조__(Syntax highlighting)
<pre><code>
```c
#include <stdio.h>

int main() {
    printf("Hello, World!");
}
```
</code></pre>
```c
#include <stdio.h>

int main() {
    printf("Hello, World!");
}
```

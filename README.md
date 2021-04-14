## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/moboong/LinuxAndNetwork/edit/main/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/moboong/LinuxAndNetwork/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.



<details markdown="1">
<summary>### 문제1 커널</summary>

운영체제의 핵심임.<br>
커널에서 (보안, 자원관리, 추상화) 역할을 수행함.<br>
자원관리 -> 메모리를 얼마나 CPU에 할당해줄 것인가에 대한 처리.<br>

커널의 구성: (안정, 메인라인, 프리패치) 버전<br>

리눅스 구성 그림 그리기.<br>
</details>

<details markdown="1">
<summary>### 문제2 가상머신</summary>
가상머신: PC 1대만으로 여러 대의 PC를 운영하는 것처럼 만드는 방법<br>
호스트 운영체제, 게스트 운영체제<br>

일반 환경 & 가상머신 환경 그림 그리기.<br>

가상머신 사용의 장점:<br>
1. 컴퓨터 1대로 실무와 비슷한 네트워크 환경 구성<br>
2. 운영체제 특정 시점을 저장하는 스냅숏 기능 -> 필요시 저장 시점으로 롤 백.<br>
3. 여러 개의 하드웨어를 장착하여 테스트 가능<br>
4. 현재 상태를 저장했다 추후에 이어서 작업하게 해주는 suspend 기능<br>


가상머신을 사용하기에 적합한 경우:<br>
1. 실무와 비슷한 네트워크 환경을 구성하여 여러 대의 서버를 구축하려 할 때<br>
2. 여러 가지 운영체제를 설치하여 학습하려 할 때<br>
3. 새로운 시스템을 도입하기 전에 테스트해보려 할 때<br>

</details>

<details markdown="1">
<summary>### 문제3 디렉토리summary>

사용자 list: /etc/passwd
그룹 list: /etc/group

</details>

<details markdown="1">
<summary>### 문제4 하드링크&심볼릭링크</summary>
하드 링크를 생성하는 명령은 ln 원본파일 링크파일명<br>
심벌릭 링크를 생성하는 명령은 ln -s 원본파일 링크파일명<br>

그림그리기<br>

하드링크는 같은 노드를 가리키고 원본데이터를 복사해서 갖는다.<br>
심볼릭링크는 다른 노드를 갖고 원본데이터의 포인터를 갖는다.<br>
원본삭제 시 하드링크는 살아있지만 심볼릭링크는 사용불가다.<br>
파악하지 못한 하드링크가 있는 경우 불필요한 저장소 낭비<br>
원본이 이동되어도 사용가능<br>

심볼릭링크는 원본삭제시 사용 불가. but 원본이름만 같으면 다른 파일이어도 동작.<br>

</details>


<details markdown="1">
<summary>### 문제5 프로세스</summary>
하드디스크에 저장된 실행 코드(프로그램)가 메모리에 로딩되어 활성화된 것<br>
Foreground process:<br>
실행하면 화면에 나타나서 사용자와 상호 작용을 하는 프로세스<br>
사용자와 상호작용을 해야만 하는 작업<br>

Background process:<br>
화면에 나타나지 않은 채 뒤에서 실행되는 프로세스<br>
오래 걸리는 작업, 상호작용을 하지 않아도 되는 작업 실행<br>

</details>

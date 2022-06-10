어제 오늘에 걸쳐서 본격적으로 프로그래밍 공부를 시작했다.
누가 시켜서 하는 것이 아닌 내 스스로 결심을 하고 나니 막연했던 해결 과정들이
귀찮은 것들이 아닌 꼭 내 손으로 해결해내고 싶은 수수께기가 된 느낌이다.
당초 git에 공부 과정을 업로드 할 생각까지는 없었는데 이것도 하나의 공부라는 생각으로 업로드 하기로 했다.
블로그를 만드는 것도 방법이긴 한데 겸사 겸사 시작한 것이다.
이렇게 하는 것이 맞나, 남들과 비교해서 모르는 것이 너무 많지만 그렇다고 가만히 있는 건 아무것도 나아지지 않는다는 생각이 이제서야 들었다

06/09
java에 대해 알아보고, 설치하고 기본적인 실습과제를 실행했다.
그런데 이 과정을 실행하고 git에 업로드 하는 것까지 무수한 error를 겪었는데, error 문구만 뜨면
인터넷 개발자 밈이 떠올랐다. "아니 해달라는데로 다 해줬는데 왜이러는거야"
아무튼, 각설하고

JAVA는 프로그래밍 언어로, 객체지향 언어이다.
객체지향 언어는 Objec-Oriented-Programming (OOP)라고도 불리며 객체지향은
프로그램 소스코드를 기계어로 변환하는 과정에서 언어를 어떤 관점으로 해석할 것인가에 대한 방식이다.  
소스코드들을 단순한 명령어들의 집합으로만 보지 않고, 하나의 객체와 객체간의 상호작용으로 보는 것이다.

즉 Object를 data(variation) + method (function)의 집합체로 보는 것이다.

JAVA는 애초 개발 목적이 가전제품에 탑재될 SW었는데, C++ 언어를 확장해서 개발하려 했지만, 장점만 도입해 개발되었고
그 이름은 OAK이다. 그러나 인터넷의 등장으로 운영체제에 독립적인 OAK가 프로그래밍의 적합성에 강점을 보이자
당초 개발 목적인 가전제품 SW에서 인터넷 SW 으로 개발방향이 선회되었다.
웹브라우저인 Hot java 공개 이후 1년만에 JAVA가 공식 발표되었고, JAVA APPLET은 정적인 WEB에서 유일한 Multimedia 컨텐츠를
제공했기에 많은 인기를 얻었다. 그러나 보안문제로 인해 최신 브라우저에서 applet을 지원하지 않고
java는 현재 서버 프로그래밍을 위한 servlet, jsp(java server pages)에서 많이 사용되고 있다.
구글의 android 또한 java를 사용한다.

앞으로 java의 원래 목표인 소규모 가전제품이나 대규모 기업 환경을 위한 SW 개발 분야에서 활발히 사용될 예정이다.

JAVA의 장점으로는

1. 운영 체제에 독립적이다. (JVM, Java Virtual Machine, 단 JVM은 OS에 종속적이고 SUN은 OS에 따른 JVM을 보급한다.)
2. 객체 지향
3. 자동 메모리 관리 (garbage collection)

그외 내가 잘 이해하지 못하는 부분이지만 장점으로는

1. 네트워크 분산 처리
2. 멀티쓰레드 지원
3. 동적 로딩 지원

내가 학위가 있는 것도 아니고 다 알 수는 없는 노릇이기에 후반부까지 공부해보고도 모르면 다시 찾아오겠다.
다만 네트워크 분산처리와 멀티쓰레드 지원을 가능하게 하는 것은 java API라는 것 정도는 알면 되겠다.

다른 프로그래밍 언어가 직접 OS와 소통하는 것과 달리 JAVA는 JVM과 소통하고, JVM이 OS와 소통한다는 점 또한 중요하다.

JAVA 개발환경 구축 // 혼자 하려니 쉽지 않다..

JDK란 Java Development Kit 의 줄임말로
JDK는 다시 JRE + 개발에 필요한 실행 파일 (javac.exe, java.exe ..., 해당 파일들은 bin directory에 저장되어 있다.)
JRE(Java Runtime Environment)는 다시 JVM + JAVA API로 구성된다.

java 프로그래밍을 시작하고 싶다면 막연히 java를 다운받아야지! 가 아니라 JDK 를 받아야 한다. (당연한 말인가)
내가 다운받은 JDK 버전은 8.0 버전으로 jdk1.8로 불린다.

설치하고 이것저것 둘러보는데 나를 위한 공부가 아니었다면 그냥 넘어갔을 것들이 궁금했다.
bin directory path 설정?은 왜 하는걸까 절대경로 상대경로? bin directory? 곁가지로 빠지기 시작하니 내용이 끝이 없다만.. 그래도 알고 싶었다.

path 설정이란 OS가 파일의 경로 필요 없이, 파일 이름만으로 실행시키기 위한 작업으로
방법은 시스템 환경 변수 편집 > 고급 > 환경변수 에서 편집하면 되겠다.

그래도 진도를 나가고 싶기 때문에 일단은 세부적을 완전히 이해할 수는 없어서 부분 포기를 하기로 했다.

파일의 절대경로와 상대경로
절대경로는 파일의 주소를 가장 최상위 Directory에서부터 기준 삼아 경로를 안내하고
상대경로는 비교하고자 하는 파일을 기준경로 삼아서, 해당 기준경로로부터의 경로를 안내하는 것이다.

ex> FileA(C:\User\wowns\FileA), FileB(C:\User\wowns\FileB)가 각각의 절대경로일 때,

FileB의 FileA에 대한 상대 경로는 python 기준(FileA를 작성 중 FileB를 참조하고 싶을 때)
./FileB인 것입니다. (Python에서 ./는 해당 파일이 있는 현재 디렉토리의 위치를 나타낸다.)

절대경로는 최상위 디렉토리로부터 파일을 탐색해 속도가 느리고 상대경로는 빠르다.
하지만 파일의 경로가 자주 바뀌거나 협업을 하는 과정에서 파일을 찾는 일은 상대경로가 더 용이하기에
두 가지 경로를 때에 따라 적절하게 사용해야 하는 것이다.

즉 bin directory path 설정은 bin directory의 실행 파일을 파일의 이름만으로도 사용할 수 있게끔 만들어주는 것이다.
절대경로를 모두 알 필요 없이, 단축키 같은 느낌인 것 같다.

여기서 bin directory란 "단일 사용자에게나 다중 사용자에게 모두 기본적으로 필요한 User 유틸리티" 라고 한다.

자 다시 돌아와서, JDK 설치를 완료했고, 이젠 JAVA API를 설치한다.
JAVA API는 역시 SUN 홈페이지에서 다운받으며, 자신이 다운 받은 JDK 종류에 맞게 다운받으면 되겠다.
jdk1.8\docs\api\index.html에서 java api에 대한 설명들을 읽을 수 있다고 해 북마크에 추가해 두었다.

06/10
eclipse 설치를 마치고 본격적인 실습을 시작했다. (나중에는 eclipse와 vsc를 연동할 수도 있다고 한다.)
eclipses는 프로그래밍 언어 편집기(IDE,Integrated Development Environment)로, C언어 편집기인 Visual Studio와 같은 역할을
해주는 프로그램으로 보인다. 다만 intelij라는 IDE도 있다고 하는데, 유료 버전이고 아직 내가 고민할 수준의 문제가 아닌 것
같아서 우선 eclipse 설치를 끝냈다. 역시, 누군가의 도움 없이는 과정 하나하나가 힘들다는 생각이 드며, 실습을 시작했다.

Hello.java 를 작성하고 컴파일 해보았다.
먼저 eclipse를 실행하고 새 java project를 만들어 낸 다음
src에서 Hello.java class를 생성했다.

모든 java 프로젝트에는 하나 이상의 main method를 포함한 class를 포함해야 한다고 한다.
main method의 처음과 끝까지 수행하는 것이 java application의 동작 과정이기에,
main method가 없는 class는 실행될 수가 없는 것이다. app 또한 실행될 수 없는 것이다.

여기서 나의 eclipse-workspace는 나의 wowns directory에 저장되어 있었고,
해당 디렉 안에는 "hello"라를 하나의 java project가 있었고, src 안에 Hello.java 라는 java 파일이
bin 안에는 Hello.java라는 class 파일이 있었다.

"어째서 class 파일이 bin directory에 있는 것일까?"
"eclipse에서 src 하위에 Hello.java라는 클래스를 생성했었늗네 어째서 src 안에 있는 파일은 java 파일인 것일까?"

아직 용어 구분이 확실하지 않기에 구글링 해보았고

bin = binary
compiled files from the eclipse는 bin 파일에 .class 확장자 파일로 저장된다.
src = source
우리가 작성한 코드는 src 파일에 저장된다 >> .java 확장자 파일

즉, eclipse-workspace\hello/_(java 프로젝트)_/\src\hello.java는 source 코드 자체 확장자
C:\jdk1.8\bin\java.exe는 컴파일된 class 파일을 interpret 하기 위한 JDK인 것이다. //아닐 수도 있다. 그러나 지금은 그렇게 생각하기로 결정했다..

// Hello.java라는 src 코드에는, Hello.class가 선언되어 있고, 프로젝트 내 유일한 class인 Hello.class에는 main method 또한 선언되어 있다.
java.exe에 의해 main method가 호출된다고 한다. 아래의 형식을 지켜야 java.exe에 의해 호출된다고 한다.

public class Hello {

    public static void main(String[] args) {
    	System.out.println("Hello, world."); // 화면에 글자 출력
    }

}

다시한번 말하지만, 모든 class가 main method를 가지고 있을 필요 없다.
다만 java app의 실행 과정은 main method의 처음부터 끝까지의 수행이기에 적어도 하나의 class 에는 main method가 필요한 것이다.

하나의 src에 하나의 class만 정의하는 것이 보통이지만, 둘 이상의 class를 지정하는 것도 가능한데,
이때 public class는 한개를 초과할 수 없다.

0<=public class<=1

public class가 0개일 때는 src 파일 이름인 .java가 어떤 class와의 이름과도 같아도 된다. (적어도 하나는 같아야겠지)
public class가 1개일 때는 해당 public class의 이름과 src 파일의 이름이 반드시 같아야 한다.

하나의 프로젝트에 여러개의 src 파일이 있을 수도 있겠는데, 해당 파일은 src directory 안에 다른 이름의 .java로 저장하면 되겠다. (윗부분의 나의 예상이 맞은듯)

하나의 소스파일에 2개 이상의 public class가 존재할 수는 없다. (public이 아니라면 상관 없음)

하나의 src에서, main method<=1
하나의 java app 안에 main method가 선언된 class가 적어도 한개 이상 존재해야 한다.

즉 하나의 src에서 main method가 없다는 것은, 다른 src 안의 class 중에서 main method가 하나는 존재해야만 한다는 것이고

모든 main method는 public 상태여야 하기 때문에 하나의 src 파일에서는 1개 이하의 main 함수가 존재해야 한다.

src 파일이 1개인 경우 해당 src 안에는 main method가 선언된 class가 1개 존재해야만 하고

src 파일이 2개 이상인 경우 같은 프로젝트 내의 src 파일 중의 그것이 1개만 존재하면 된다는 것이다.
이와 같은 경우 main이 2개일 수도 있겠지 (src 마다 main 포함한 class가 1개씩 있는 경우)

public class가 선언된 경우 해당 src 파일의 이름은 해당 class 이름과 일치해야만 하고,
public class가 선언되지 않은 경우 해당 src 파일의 이름은 내부 class 중 임의로 설정해도 무방하다.
ㄴ 이말은 역시 main method가 선언되지 않았다는 것이기에 같은 프로젝트의 다른 src에 main이 있어야 한다!!!!! (후....)

여기까지가 hello project를 진행하면서 배운 것이다.
참.. 정말 간단한 내용일 수 있지만 내것으로 만드려 하니 참 어렵다. 하지만 내가 사용할줄 알려면 이정도는 해야겠지!!

많은 error들을 (git 원격 저장소에 commit 하는 것까지) 수행하며 봐왔는데 그 내용들은 06/11 내용에 정리하도록 하겠다.
오늘은 여기까지...

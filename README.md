# 컴퓨터구조 (Computer Architecture) 2018 가을학기

*  *  *
## [알림] 기말고사 12월 19일 (수요일) 오후 1시 강의실 1145

## QnA는 [여기](https://github.com/jeonggunlee/Computer_Arch_2018_Fall/blob/master/QnA.md)를 눌러 작성해주세요!

## (DONE!)[알림] 보강 수업 --> 19일 월요일 오후 6시 1163-7 에서 진행합니다!!! 꼭꼭꼭 참석해주세요~!

## (DONE!)[알림] 중간고사 10월 22일 (월요일) 오후 1시 강의실 1163-7

## [기출문제](https://github.com/jeonggunlee/Computer_Arch_2018_Fall/tree/master/ex_exam) 참조하세요!

*  *  *

>컴퓨터 시스템을 이루는 프로세서, 메모리, 버스, 주변 장치 등의 각 요소를 중심으로, 기본 구조와 동작 원리를 배우고, 이를 통해 하드웨어 및 소프트웨어의 개발에 필요한 깊이 있는 지식을 익힌다. 이 과정에서는 기초적인 요소 기술의 소개는 물론, 상용 기술의 사례 연구를 통해 수강자들이 최근의 기술 동향을 파악하게 하고 향후에 이를 활용할 수 있는 기반 지식을 제공한다.
>
> 이 과정에서는 또한 MIPS 프로세서 기반의 하드웨어를 중심으로 프로세서 구조, 어셈블리 프로그래밍 등을 실습함으로 이론을 확인, 심화하는 과정을 제공한다. 본 교과목은 <임베디드 시스템 개론> 및 <임베디드 하드웨어>의 권장 선수과목이다.

## 강의 스탭
### 담당교수: 이정근
   - 연구실:(성호관 1306호실) / Email: Jeonggun.Lee (AT) gmail.com
   - 전화번호: 033-248-2312 (연구실)
   - 홈페이지: [www.onchip.net](www.onchip.net)
   
### 담당조교: 정다운
   - (데이터베이스 연구실, Email: kozer9@gmail.com)
   
## 교재
   - 주교재: "[디지털논리와 컴퓨터설계](http://www.yes24.com/24/goods/3311366)," 데이비드 해리스,사라 해리스 공저/조영완 등역, 사이텍미디어
   - 부교재: "컴퓨터 구조 및 설계 : 하드웨어/소프트웨어 인터페이스 ARM 버전," 데이비드 패터슨,존 헤네시 공저/박명순,김병기,하순회,장훈 공역, 비제이퍼블릭(BJ퍼블릭)   
   
## 평가방법
   - 중간 35%, 기말 35%, 실습 20%, 숙제 & 퀴즈 10%
   - 결석 4회 이상 "F", 사유가 있어도 결석임!
   - 결석 1회를 만회하기 위해서는 "추가로 숙제를 제출"해야함
   - 실습 숙제의 경우 smart campus를 통하여 수집 및 

## 강의노트
   - Chapter 6 :: MIPS 어셈블리 언어와 명령어 포맷, [PPT](https://github.com/jeonggunlee/Computer_Arch_2018_Fall/blob/master/DDCA_Ch6%20-%201.pptx)
      - 6.1 소개
      - 6.2 어셈블리 언어
      - 6.3 기계어
      - 6.4 어셈블리를 이용한 프로그래밍 구조
      - 참조 동영상
          - [ISA 1.1 Introduction to the ISA](https://www.youtube.com/watch?v=PlavjNH_RRU)
          - [ISA 1.2 MIPS Instructions](https://www.youtube.com/watch?v=ykI9nwSNFfM)
   - Chapter 7 :: Microarchitecture: MIPS 프로세서의 구조, Pipelining
      - 7.1 소개
         - 7.1.1 아키텍쳐의 상태 및 명령어 집합(Instruction Set)
         - 7.1.2 설계 과정 (데이터패스, 제어패스)
         - 7.1.3 MIPS 마이크로아키텍쳐
      - 7.2 성능 분석
      - 7.3 Single-Cycle 프로세서
         - 7.3.1 Single-Cycle 데이터패스
         - 7.3.2 Single-Cycle 제어
         - 7.3.3 추가적인 명령어 지원
         - 7.3.4 성능 분석
   - Chapter 8 :: Memory Systems: 메모리 계층, 캐쉬메모리 구조
      - 8.1 소개
      - 8.2 메모리 시스템 성능 분석
      - 8.3 Caches (캐시 메모리)
         - 8.3.1 어떤 데이터를 캐시 메모리에 넣을것인가?
         - 8.3.2 캐시 메모리에서 데이터를 어떻게 찾을 것인가?
         - 8.3.3 어떤 데이터를 바꿀 것인가?
         - 8.3.4 고급 캐시 설계

## 실습
   - QtSpim 을 이용한 MIPS 어셈블러 프로그래밍 ([Youtube](https://www.youtube.com/results?search_query=Qtsim+PCSIM+MIPS))
   - [요기-한국어!!!](https://www.joinc.co.kr/w/Site/Assembly/Documents/Spim) : SPIM에 대한 자세한 한글 설명을 볼수 있습니다.
   - [조기](http://chortle.ccsu.edu/AssemblyTutorial/index.html) : 위 사이트의 영문 원본 문서를 볼수 있습니다.
   - Spim 공부를 위한 [좋은 곳](http://www.cs.ccsu.edu/~markov/ccsu_courses/254syllabus.html)!
   
   > SPIM은 오픈소스 SW로 구현된 MIPS 프로세서 시뮬레이터입니다. [MIPS 시뮬레이터](http://spimsimulator.sourceforge.net/)
   > 관심있는 학생들은 SPIM 시뮬레이터의 소스코드를 분석하고 수행시켜봄으로써 보다 자세히 명령어의 수행 구조 및 프로세서 구조에 대해서 이해할수 있습니다.
   > 컴퓨터구조 교과목은 오픈소스 SW에 대한 이해도 함께 증진시키는 것을 목적으로 합니다.
   
   ![Alt text](https://github.com/jeonggunlee/Computer_Arch_2018_Fall/blob/master/img/openss.png "오픈소스교과목")

## 참조 사이트
   - [MIPS 프로세서 위키백과사전](https://ko.wikipedia.org/wiki/MIPS_%EC%95%84%ED%82%A4%ED%85%8D%EC%B2%98) : 밉스 프로세서에 대한 자세한 설명을 한글로 볼수 있습니다.

   
   
   

# 메모장

# 이클립스 ini 수정 사항

- 14줄 아래에
- -vm
- C:/Program Files/Java/jdk-11.0.14/bin (역슬래쉬 -> 슬래쉬)

개발도구설치
https://github.com/callor/Reference/blob/master/%EA%B0%9C%EB%B0%9C%EB%8F%84%EA%B5%AC%EC%84%A4%EC%B9%98.md

# 04-26

- 오라클 -> db xe 11 버전 (https://www.oracle.com/database/technologies/xe-prior-release-downloads.html)
- 오라클 -> MySQL (https://dev.mysql.com/downloads/installer/)

* 오라클 -> SQL Developer JDK 8 included (https://www.oracle.com/tools/downloads/sqldev-downloads.html)

sys / 12341234

# 이클립스에 lombok jar 추가하기.
* [메이븐](https://mvnrepository.com/artifact/org.projectlombok/lombok) 에서 최신 lombok.jar 파일을 다운받기
* 다운받은 폴더에서 관리자 권한으로 cmd 실행해서
```
java -jar lombok.jar
```
하여 설치 진행
* 경로를 이클립스 폴더로 지정하고 설치하면 끝

# mybatis-context 설정하기 (Spring 에 DB 연결 작업)
* [링크](https://github.com/dosunggil/Spring/tree/master/SpMVC_003_SchoolV6)
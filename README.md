# VI_Earth_raspberryPI
상명대학교 임베디드 시스템 3조 Vi Earth - 라즈베리파이

[실행 영상](https://youtu.be/bR5_IRo4VVs)

실시간 서버 구현!
1. 라즈베리파이에 mariadb를 설치 후 db의 저장 내용을 보기 쉽게 하기 위해 윈도우에 HeidiSQL을 설치하였다.

2. 라즈베리파이의 설치된 mariadb 서버를 열기 위해 라즈베리파이의 ip주소와 미리 만들어둔 사용자 아이디인 ‘root’, 비번을 HeidiSQL 입력 후 서버를 연다.

3. HeidiSQL를 통해 라즈베리파이의 mariadb에 'userdata'(데이터베이스 명)을 생성 후  ‘users’(table 명)을 생성

4. 라즈베리파이 터미널창에서 node app7.js 파일을 실행하여 소켓 서버를 연다.

5. test를 위해 만들어둔 http://localhost:3000/public/adduser2.html에 접속하여 사용자 추가란에 입력한다.

6. nodejs를 통해 mariadb의 데이터 저장을 수행한다.
 *해당 사진은 nodejs의 데이터 저장시 상태를 나타낸다.
 
 ![캡처](https://user-images.githubusercontent.com/54584364/94412629-f91b7780-01b4-11eb-9b94-564f9491e1ff.PNG)
 
 7. 이후 유니티 프로그램과 연동하여 실시간 소켓 데이터 전달을 구현

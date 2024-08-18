# Systme_Architecture
![image](https://github.com/user-attachments/assets/be72cd45-9d6c-490c-8df1-5b77eb5c0f24)

# scenario
![image](https://github.com/user-attachments/assets/113a34cb-2c78-47ed-8d36-efe5ec192fad)
1. 유저가 spring 서버에 회원가입을 진행.
2. 사용자 정보를 mysql DB에 저장
3. Return Result
---

![image](https://github.com/user-attachments/assets/ac6061f2-02cb-4d08-bc95-7cc8d54e45cc)
1. 유저가 spring 서버에 로그인을 진행.
2. 서버에서 로그인 정보를 확인, 세션키 저장
3. 세션 키 반환
---
![image](https://github.com/user-attachments/assets/7a6c02e6-0ba8-4c38-8e97-5672bcabc1b6)
1. 유저가 spring 서버에 자신의 흥미 정보를 전송.
2. 세션키 검증
3. 사용자 카테고리 정보 저장 (ex : [0.1,0.8,1.0,0.6,0.3,0.2])
4. Return Result
---
![image](https://github.com/user-attachments/assets/b3c01166-e1e8-4566-8bdb-2e5ef5e18653)
1. 유저가 spring 서버에 자신의 정보와 읽은 뉴스 id를 전송.
2. 세션키 검증
3. 사용자 카테고리 정보 read (ex : [0.1,0.8,1.0,0.6,0.3,0.2])
4. Spring 이 fastAPI서버에 연산을 요청 및 결과 반환받음. (ex : [0.1,0.8,1.0,0.6,0.3,0.2])
5. 사용자 카테고리 정보 업데이트
6. Return Result
---

![image](https://github.com/user-attachments/assets/b607eb0b-0edf-4384-bff5-940d456b3ea8)
1. newStore에서 news 정보를 읽고, 전처리
2. 데이터를 mongoDB에 저장
---

![image](https://github.com/user-attachments/assets/fc53fae3-63dc-4243-9c3f-4e03f110ea19)
1. 유저가 spring 서버에 자신의 정보를 저장
2. 세션키 검증
3. 사용자 카테고리 정보 read (ex : [0.1,0.8,1.0,0.6,0.3,0.2])
4. Spring 이 fastAPI 메소드 요청처리 parameter : (ex : [0.1,0.8,1.0,0.6,0.3,0.2])
5. mongoDB에서 read data, ex) 유사도 계산, elastic search
6. Return Result
7. Return Result



<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->


### MariaDB 시작하기
![Maraidb](https://github.com/user-attachments/assets/dd46324b-7c6b-466f-9e36-bd61a875a490)

노션 링크: https://wind-dewberry-ca7.notion.site/db-bed229466fb5478ebbc17b3a5c356b63?pvs=4


- mysql을 기반으로한 오픈소스 데이터베이스
- mysql 과 거의 흡사한 아키텍처를 가지고 있다

### 서평

```jsx
특이하게도  입문서 치고는 실습 예제가 리눅스위주이다.
한 번 정도 또는 마리아db가 처음이라면 읽어볼만한 책이다.
```

### 설치하기 (centos)

---

- vi /etc/yum.repo.d/MariaDB.repo

```jsx
# MariaDB 10.5 CentOS repository list - created 2024-09-06 19:39 UTC
# https://mariadb.org/download/
[mariadb]
name = MariaDB
# rpm.mariadb.org is a dynamic mirror if your preferred mirror goes offline. See https://mariadb.org/mirrorbits/ for details.
# baseurl = https://rpm.mariadb.org/10.5/centos/$releasever/$basearch
baseurl = https://tw1.mirror.blendbyte.net/mariadb/yum/10.5/centos/$releasever/$basearch
module_hotfixes = 1
# gpgkey = https://rpm.mariadb.org/RPM-GPG-KEY-MariaDB
gpgkey = https://tw1.mirror.blendbyte.net/mariadb/yum/RPM-GPG-KEY-MariaDB
gpgcheck = 1

```

- yum update
- yum -y install MariaDB
- systemctl start MariaDB
- mysql -u  root -p

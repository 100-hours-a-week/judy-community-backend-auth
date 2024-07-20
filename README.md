### `auth README.md`

#### `judy-community-backend-auth`

# Judy Community Auth Backend

사용자 인증 및 권한 관리를 담당하는 백엔드 서비스입니다.

## 구조

```
judy-community-backend-auth/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/
│   │   │       └── judycorp/
│   │   │           └── auth/
│   │   │               ├── config/
│   │   │               ├── controller/
│   │   │               ├── dto/
│   │   │               ├── entity/
│   │   │               ├── exception/
│   │   │               ├── repository/
│   │   │               ├── security/
│   │   │               ├── service/
│   │   │               └── ApplicationAuth.java
│   ├── resources/
│   │   └── application.properties
├── Dockerfile
├── build.gradle.kts
└── settings.gradle.kts
└── .github/
    └── workflows/
        └── ci-cd.yml
```

## 기능

- 사용자 등록
- 사용자 로그인
- JWT 기반 인증

## 설치 및 실행

### 사전 요구 사항

- [Docker](https://www.docker.com/get-started)
- [JDK 17](https://adoptopenjdk.net/)

### Docker 이미지 빌드 및 실행

```bash
./gradlew build
docker build -t your_dockerhub_username/judy-community-backend-auth .
docker run -p 8081:8080 your_dockerhub_username/judy-community-backend-auth
```

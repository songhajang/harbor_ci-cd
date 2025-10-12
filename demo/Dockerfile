# 1️⃣ Base image
FROM eclipse-temurin:17-jdk-alpine

# 2️⃣ 작업 디렉터리 생성
WORKDIR /app

# 3️⃣ Maven 빌드 결과 JAR 복사
# GitHub Actions에서 ./mvnw clean package로 JAR 빌드 후
COPY target/*.jar app.jar

# 4️⃣ 컨테이너 포트 설정
EXPOSE 8080

# 5️⃣ 실행 명령
ENTRYPOINT ["java", "-jar", "app.jar"]

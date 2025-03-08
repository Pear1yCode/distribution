# distribution

## 1. 도커 설치

## 2. 젠킨스 설치

## 3. 도커 파일 작성 (프론트, 백엔드 전부)
.env 파일의 경우 실행 시 외부 주입 방식으로 보안 강화

## 4. docker ignore 확인

## 5. docker image builde
3번의 docker file이 있는 경로 터미널에서 이미지 빌드

프론트엔드
docker buildx build -t ukki-front .
ukki-front 이름으로 해당 경로에 이미지 빌드함

백엔드
docker buildx build -t ukki-back .
ukki-back 이름으로 해당 경로에 이미지 빌드함

## 6. 컨테이너 실행
docker run -d -p 80:80 --name ukki-front-container ukki-front   
docker ps를 통해서 제대로 실행됐는지 (어느 포트에서 실행됐는지) 확인

docker run -d -p 8080:8080 --name ukki-back-container ukki-back
docker ps

## 7. 컨테이너 돌아갔으므로 들어가서 확인하기
프론트엔드 : http://127.0.0.1

백엔드(API 확인용) : http://127.0.0.1:8080/api

## 8. env파일 및 yml 파일 확인

## 9. docker compose로 프론트 엔드와 백엔드 합쳐줄 수 있음 (yml파일)

## 10. aws 로그인

## 11. ec2 인스턴스 생성

## 12. 컨테이너와 이미지
powershell에서 docker desktop 켜져있어야 명령어 실행됨

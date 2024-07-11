# Development Container

웹 개발을 위한 개발 컨테이너입니다.



## 실행 방법

1. Docker Desktop 실행
2. 터미널에 커맨드 입력
  ```sh
  # project root 위치에서 실행

  # docker-compose로 실행
  docker-compose -f docker/docker-compose.yml up -d

  # Dockerfile로 실행
  docker build -t dev-container docker/.
  docker run --name dev-container -dit --rm dev-container
  ```

3. VSCode 열기 

4. 익스텐션 **Remote Development** 설치

5. 다음을 통해 컨테이너 환경 접속

   - `Ctrl` / `CMD` + `p`
   - `> Dev Containers: Attach to Running Container... `선택
   - `/dev_container` 선택



## 버전 정보

- Python 3.8.13

- node v16.20.2

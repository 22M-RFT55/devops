# ---------------------------------------------------------------
# 학생 과제: 아래 각 줄이 무엇을 하는지 주석으로 설명을 달아보세요.
# ---------------------------------------------------------------

# 기반 이미지 설정
FROM python:3.12-slim

# 작업 디렉터리 설정
WORKDIR /app

# 캐시 재사용을 위해 라이브러리 목록 먼저 복사
COPY requirements.txt .
# 라이브러리 설치, 이미지 만들때 한 번 실행
RUN pip install --no-cache-dir -r requirements.txt

# 나머지 코드들 이미지 안으로 복사
COPY . .

# 사용자로 실행
RUN useradd -m appuser
USER appuser

# 환경 변수 설정
ENV APP_TITLE="InhaTC DevOps 6주차 방명록" \
    THEME_COLOR="#FF9329"

# 포트 번호 명시
EXPOSE 5000

# 컨테이너 시작 시 실행할 명령, 컨테이너 실행할 때마다 실행
CMD ["python", "app.py"]

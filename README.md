# Fullstack GPT
Langchaing 기반 Chat 서비스 구현

## Run server
```
streamlit run Home.py --server.port 8501
```

## Issue
##### 1. Streamlit, OSError: [Errno 28] inotify watch limit reached
```
# 파일 열기
sudo vim /etc/sysctl.conf
# 마지막 라인에 추가
fs.inotify.max_user_watches = 1100000
# 변경사항 적용
sudo sysctl -p
```
##### 2. playwright._impl._api_types.Error: Executable doesn't exist at /home/lab021/.cache/ms-playwright/chromium-1084/chrome-linux/chrome
```
playwright install
sudo apt-get install libnss3 libnspr4 libatk1.0-0 libatk-bridge2.0-0 libcups2 libxkbcommon0 libatspi2.0-0 libxcomposite1 libxdamage1 libxrandr2 libpango-1.0-0 libcairo2
```

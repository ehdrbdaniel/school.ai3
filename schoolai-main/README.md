# SchoolAI

## OpenWeather API 키 설정

로컬에서 실행할 때 프로젝트 루트에 `.streamlit/secrets.toml` 파일을 만들고 다음처럼 설정하세요.

```toml
OPENWEATHER_API_KEY = "발급받은_API_키"
```

`.streamlit` 폴더가 없다면 먼저 만드세요. 키를 저장소에 올리거나 다른 사람에게 공유하지 마세요. 이 파일은 `.gitignore`에 포함되어 있습니다.

Streamlit Community Cloud에서 실행한다면 앱의 **Settings → Secrets**에 같은 항목을 추가하세요.

키가 없으면 앱은 안내 메시지를 표시하고 날씨 정보 없이 예측합니다. HTTP 401 메시지가 나오면 키 값을 확인하고, OpenWeather에서 새로 발급한 키라면 활성화될 때까지 기다린 뒤 다시 시도하세요.
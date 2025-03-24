### Path parameter:
http://localhost:8000/get_transcript/abc123/en 
(to identify specific resources, i.e. /cars)

### Query parameter:
http://localhost:8000/get_transcript/?video_id=abc123&lang=en
(sort/filter resources, i.e. /cars?color=red)

### API Reference:
[YouTube Transcript API](https://pypi.org/project/youtube-transcript-api/)

### Steps to run the server:

0. Create a virtual environment:
    ```bash
    python3 -m venv <ENV_NAME>
    ```
    (Skip if you already have an `env` folder)

1. In terminal, run:
    ```bash
    source <ENV_NAME>/bin/activate
    ```
    (Type `deactivate` to exit)

2. Install dependencies:
    ```bash
    pip install fastapi
    pip install youtube_transcript_api
    pip install "fastapi[standard]"
    ```

3. Start the server:
    ```bash
    fastapi dev main.py
    ```

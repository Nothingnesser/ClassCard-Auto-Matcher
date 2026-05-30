# ClassCard-Auto-Matcher

Python과 Selenium을 활용하여 ClassCard 매칭 학습을 자동화하는 프로젝트입니다.

프로그램은 학습 세트의 단어, 뜻, 음성 데이터를 수집하여 JSON 데이터베이스를 생성한 후, 매칭 게임에서 자동으로 정답을 찾아 클릭합니다.

## Features

* 자동 로그인
* 학습 세트 데이터 수집
* 단어 ↔ 뜻 자동 매핑
* 음성 파일 ↔ 뜻 자동 매핑
* JSON 기반 데이터 저장
* 자동 매칭 수행
* 실시간 점수 확인

## Tech Stack

* Python 3
* Selenium
* Chrome WebDriver
* JSON

## Project Structure

```text
project/
│
├── main.py
├── cardbot_Source.json
├── classcard_audio.json
├── requirements.txt
└── README.md
```

## How It Works

1. ClassCard 로그인
2. 학습 세트(set) 페이지 진입
3. 단어·뜻·음성 데이터 수집
4. JSON 형태로 저장
5. Match 게임 진입
6. 저장된 데이터를 기반으로 자동 매칭 수행

## Installation

### 1. Clone Repository

```bash
git clone https://github.com/your-id/classcard-match-bot.git
cd classcard-match-bot
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Install Chrome

Chrome 브라우저가 설치되어 있어야 합니다.

Chrome 버전에 맞는 ChromeDriver가 필요할 수 있습니다.

## Usage

프로그램 실행

```bash
python main.py
```

실행 후

```text
ID :
PWD :
```

순서대로 입력합니다.

로그인 후 학습 세트 페이지에 접속하면 데이터가 자동으로 수집됩니다.

이후 Match 게임 페이지로 이동하면 자동으로 정답을 찾아 매칭을 수행합니다.

## Output Files

### cardbot_Source.json

```json
{
    "apple": "사과",
    "banana": "바나나"
}
```

### classcard_audio.json

```json
{
    "audio_url_1": "사과",
    "audio_url_2": "바나나"
}
```

## Learning Outcomes

* Selenium 기반 웹 자동화 구현
* DOM 요소 탐색 및 제어
* JSON 데이터 저장 및 활용
* 웹 서비스 데이터 수집
* 객체지향 프로그래밍(OOP) 활용
* 자동화 알고리즘 설계

## Disclaimer

This project was created for educational and personal learning purposes.

Users are responsible for complying with the terms of service of any platform they use with this software.

본 프로젝트는 교육 및 개인 학습 목적으로 제작되었습니다.

사용자는 해당 소프트웨어를 사용하는 과정에서 각 플랫폼의 이용 약관을 준수해야 합니다.

## License

MIT License

## Requirments

- Python 3.10+
- Google Chrome
- Selenium 4+

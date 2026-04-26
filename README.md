# 🌻 언니에게 — 30일 응원 앱

---

## 📁 폴더 구조 (GitHub에 이렇게 올려줘!)

```
프로젝트 폴더/
├── app.py
├── requirements.txt
└── media/
    ├── photos/
    │   ├── photo_01.jpg   ← Day 8  사진
    │   ├── photo_02.jpg   ← Day 13 사진
    │   ├── photo_03.jpg   ← Day 16 사진
    │   ├── photo_04.jpg   ← Day 20 사진
    │   ├── photo_05.jpg   ← Day 27 사진
    │   ├── photo_06.jpg   ← Day 28 사진
    │   └── photo_07.jpg   ← Day 30 사진
    └── videos/
        ├── video_01.mp4   ← Day 19 영상
        ├── video_02.mp4   ← Day 23 영상
        ├── video_03.mp4   ← Day 24 영상
        └── video_04.mp4   ← 영상 모음 탭 보너스
```

---

## 🖼️ 날짜별 사진/영상 배치표

| 날짜 | 파일 | 내용 |
|------|------|------|
| Day 8  | photo_01.jpg | 연말 파티 사진 |
| Day 13 | photo_02.jpg | 동성 배경 사진 |
| Day 16 | photo_03.jpg | 언니가 준비해준 날 사진 |
| Day 19 | video_01.mp4 | 인생네컷 타임랩스 1 |
| Day 20 | photo_04.jpg | 맛있는 거 먹은 사진 |
| Day 23 | video_02.mp4 | 인생네컷 타임랩스 2 |
| Day 24 | video_03.mp4 | 인생네컷 타임랩스 3 |
| Day 27 | photo_05.jpg | 글씨 색 속이는 그거 사진 |
| Day 28 | photo_06.jpg | 언니 예쁜 사진 |
| Day 30 | photo_07.jpg | 피크닉 사진 |

---

## ⚙️ 파일 이름 규칙

- 사진: `photo_01.jpg` 형식 (숫자 두 자리, 소문자)
- 영상: `video_01.mp4` 형식
- JPG, PNG, MP4 모두 가능
- 확장자가 다르면 app.py 안 DAY_DATA에서 파일명 수정해줘

예) PNG라면: `"photo": "photo_01.png"` 으로 바꾸면 돼

---

## 🚀 배포 방법

### 1단계: GitHub에 올리기
1. GitHub에서 새 레포지토리 만들기 (예: `love-for-unni`)
2. 위 폴더 구조 그대로 파일 업로드
   - `app.py`, `requirements.txt` 루트에
   - `media/photos/` 안에 사진 7장
   - `media/videos/` 안에 영상 4개

### 2단계: Streamlit Cloud 배포
1. [share.streamlit.io](https://share.streamlit.io) 접속
2. GitHub 계정으로 로그인
3. **"New app"** 클릭
4. Repository: 방금 만든 레포 선택
5. Main file path: `app.py`
6. **"Deploy!"** 클릭

### 3단계: 언니한테 링크 공유
`https://xxx.streamlit.app` 링크 카톡으로 보내주면 끝! 📱

---

## ✏️ 메시지 수정하는 법

`app.py` 파일의 `DAY_DATA` 딕셔너리에서 원하는 날짜 찾아서 `"message"` 부분 수정하면 돼!

```python
3: {
    "emoji": "🙏",
    "photo": None,
    "video": None,
    "message": (
        "여기 내용 바꾸면 돼!\n"
        "줄바꿈은 \\n 으로 해줘"
    ),
},
```

---

## ❓ 문제 생기면

**사진이 안 보여요** → 파일 이름 확인! 소문자, 숫자 두 자리인지 체크  
**영상이 느려요** → MP4가 맞는지 확인. 용량이 너무 크면 압축해줘  
**배포가 안 돼요** → requirements.txt가 루트 폴더에 있는지 확인

---

언니 꼭 이겨내길 바라요 💛🌻

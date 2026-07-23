# 또잉이 영단어 대작전

사진 한 장으로 단어를 등록하고, 다마고치를 키우며 단어를 외우고, 듣기 퀴즈를 풀고 채점까지 되는 가족용 영어 학습 앱입니다.

## 사용 전 준비물

1. **GitHub Personal Access Token** (이 저장소에 대한 읽기/쓰기 권한)
   - GitHub → 우측 상단 프로필 → Settings → Developer settings → Personal access tokens → Fine-grained tokens → Generate new token
   - Repository access: "Only select repositories" → 이 저장소 선택
   - Permissions → Repository permissions → **Contents: Read and write**
   - 생성된 토큰은 **앱의 설정 화면에만** 붙여넣으세요 (다른 곳에 공유하지 마세요).

2. **Anthropic API Key**
   - https://console.anthropic.com/settings/keys 에서 발급

## 기기 설정

부모님 기기와 또잉이 기기 양쪽 모두에서 앱을 처음 열면 설정 화면이 나옵니다.

- GitHub 저장소: `owner/repo명` (예: `suhyun/ttoing-english`)
- 브랜치: `main`
- Personal Access Token, Anthropic API Key, 모델을 동일하게 입력해주세요.
- "이 기기는 누구 것인가요?"에서 부모님 기기는 **부모님(관리자)**, 또잉이가 쓰는 기기는 **또잉이**를 선택하세요.

두 기기 모두 같은 GitHub 저장소를 데이터 저장 창고로 사용하기 때문에, 또잉이의 학습 진도와 오답이 부모님 기기에도 그대로 보입니다.

## 사용 흐름

1. (부모) 단어장 사진 업로드 → 단어 추출/저장 → 활성화
2. (또잉이) "단어 외우기" 탭에서 매일 10개씩 신규 + 이전 단어 복습, 다마고치에게 밥 주기
3. 30개(활성 단어장 전체)를 다 외우면 "퀴즈 풀기" 탭 잠금 해제
4. (또잉이) 듣기 문제를 듣고 공책에 답 작성 → 사진 업로드 → 자동 채점 + 오답노트 저장
5. (부모) "진도 현황" 탭에서 또잉이의 학습 상태와 틀린 단어 확인

## 주의

- GitHub Personal Access Token은 이 저장소에만 쓰기 권한이 있는 fine-grained 토큰을 권장합니다.
- Anthropic API 호출마다 소량의 비용이 발생합니다.

# 잇다(IT DA) - Vercel 배포 가이드

## 방법 1: Vercel CLI (가장 빠름)

```bash
# 1. Vercel CLI 설치
npm install -g vercel

# 2. 이 dist 폴더 안에서 실행
cd itda-dist
vercel

# 3. 설정 질문에 답변
# - Set up and deploy? → Y
# - Which scope? → 본인 계정 선택
# - Link to existing project? → N
# - Project name? → itda-app (원하는 이름)
# - In which directory is your code located? → ./ (현재 폴더)
# - Want to modify settings? → N
```

## 방법 2: Vercel 대시보드 (드래그 앤 드롭)

1. https://vercel.com 접속 후 로그인
2. "Add New Project" 클릭
3. "Upload" 탭 선택
4. 이 ZIP 파일을 통째로 드래그 앤 드롭
5. Framework Preset: **Other** 선택
6. Deploy 클릭

## 방법 3: GitHub 연동

1. 이 dist 폴더 내용을 GitHub 저장소에 push
2. Vercel에서 해당 저장소 연결
3. Framework: Other, Output Directory: `.` (루트)
4. Deploy

## 배포 후 접속

배포 완료 시 `https://itda-app-xxxx.vercel.app` 형태의 URL이 생성됩니다.
커스텀 도메인(예: itda-gold.vercel.app)은 Vercel 대시보드 Settings > Domains에서 설정 가능합니다.

## 포함된 화면

- 스플래시 / 로그인 / 팀 선택
- 홈화면 (팀 전환 바텀시트)
- 메모 (집중모드 스와이프)
- 채팅 목록 / 채팅방 / 채팅 상세정보
- 알림 / 내 정보 / 메뉴창
- 일정 / 게시판 / 설정

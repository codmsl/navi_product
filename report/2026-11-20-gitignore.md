# .gitignore 작성

## 체크리스트
- [x] `.gitignore` 생성: `.DS_Store`, 영상 파일 확장자 무시
- [x] 이미 추적 중이던 `.DS_Store` 3개를 저장소 추적에서 제외 (`git rm --cached`, 로컬 파일은 유지)

## 요약
- **무엇을**: macOS가 만드는 `.DS_Store`와 영상 파일이 저장소에 올라가지 않도록 `.gitignore`를 추가했습니다.
- **왜**: 개발과 무관한 시스템 파일과 용량이 큰 영상 파일이 커밋에 섞이는 것을 막기 위해서입니다.
- **어떻게**: 영상 확장자는 mp4, m4v, mov, avi, mkv, webm, wmv, flv, f4v, mpg, mpeg, 3gp, 3g2, ogv, mts, m2ts, vob, asf, rm, rmvb를 넣었습니다. `.ts`는 TypeScript 파일과 겹쳐서 제외했습니다. 이전부터 추적되던 `.DS_Store`(루트, `reference/`, `research/`)는 추적만 해제했습니다.

# github flow
**github flow**는 github를 기반으로 한 워크플로우 방법중 하나이며 다음과 같은 단계를 따른다
- branch생성: 기존 프로그램에서 기능 추가/ 버그 수정을 위해 기지를 친다.
-commit: 코드 변경 후 기록한다.
-pull request: 변경한 내용들을 모두 branch에 병햡한다.
-리뷰 및 피드백: 다른 개발자들이 이를 보고 피드백한다.
- 병합: 본래 브랜치로 병햡한다.

git flow보다 훨씬더 간단하고 직관적이며 빠르다는 장접이 있다.
그러나 대규모 프로젝트에 제한적이고 배포에 위험성이 따른다는 단점도 존재한다.
[github flow](https://velog.io/@gmlstjq123/Git-Flow-VS-Github-Flow).

# commit convention
규격화된 커밋 메세지로 질서를 추구함으로써 조금 더 수월한 협업이 될 수 있게 한다.
```
1. 제목(Type: subject): 제목으로 최대한 간단히 적어야 하며, 
첫글자 대문자와 동사 원형을 원칙으로한다.

2. body:
변경 이유를 자세히 설명한다.

3. footer:
이슈 번호에 대해 서술할 때 작성한다.
```
예시는 다음과 같다.
```
Feat: 회원 가입 기능 구현

SMS, 이메일 중복확인 API 개발

Resolves: #123
Ref: #456
Related to: #48, #45
```

### tag
- Feat:추가
- Fix:수정
- Design:디자인 변경
- !BREAKING CHANGE: 큰 api 변경
- !HOTFIX: 급한 버그 수정
- Style: 단순 코드 정리
- Refactor:프로덕션 코드 리펙토링
- Comment: 코멘트 추가
- Docs: 문서수정
- Test: 테스트 코드 추가
- Chore: 빌드 업무 수정, 패키지 매니저 수정, 패키지 관리자 구성 등 업데이트, Production Code 변경 없음
- Rename: 이름 또는 경료 변경
- Remove: 파일 삭제

### Footer
- Fixes: 이슈 수정중 (아직 해결되지 않은 경우)
- Resolves: 이슈를 해결했을 때 사용
- Ref: 참고할 이슈가 있을 때 사용
- Related to: 해당 커밋에 관련된 이슈번호 (아직 해결되지 않은 경우)

[commit convention](https://velog.io/@archivvonjang/Git-Commit-Message-Convention).
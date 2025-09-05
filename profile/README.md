## 팀원

### PM
<table>
  <tbody>
    <tr>
      <td align="center">정진영*</td>
      <td align="center">박정한</td>
    </tr>
  </tbody>
</table>


### Product Designer
<table>
  <tbody>
    <tr>
      <td align="center">임건형*</td>
      <td align="center">고수정</td>
      <td align="center">전승리</td>
    </tr>
  </tbody>
</table>

### Frontend 개발
<table>
  <tbody>
    <tr>
      <td align="center"><a href="https://github.com/SeeunJung">정세은*</a></td>
    </tr>
  </tbody>
</table>

### Backend 개발
<table>
  <tbody>
    <tr>
      <td align="center"><a href="https://github.com/Ogu1208">이우창*</a></td>
      <td align="center"><a href="https://github.com/EndlessMilkyway">김영렬</a></td>
      <td align="center"><a href="https://github.com/Altair5869">김태훈</a></td>
    </tr>
  </tbody>
</table>

_*파트 리더_

## Commit 규칙

<details>
  <summary>Commit 규칙</summary>

### label

| feat | 새로운 기능 추가 |
| --- | --- |
| fix | 버그 수정 |
| env | 개발 환경 관련 설정 |
| style | 코드 스타일 수정 |
| refactor | 코드 리팩토링 |
| test | 테스트 코드 추가/수정 |

### Commit message

`<label>: <작업 내용 설명> (#<issue_number>)` 형식을 지켜주세요.

ex) `feat: 메인 레이아웃 추가 (#1)` 

- 제목을 보고 어떤 작업을 했는지 파악할 수 있게 짧게 작성
- 제목 끝에 마침표 생략
- 현재 시제, 명령형 사용 (예시 : Added login endpoint(X), Add login endpoint(O))

</details>

## Git 브랜치 전략

<details>
  <summary>Git 브랜치 전략</summary>

### Branch naming

| 유형 | 브랜치명 | 예시 |
| --- | --- | --- |
| 배포 브랜치 | main |  |
| 개발 브랜치 | develop |  |
| 기능 개발 | feat/이슈 번호-기능 설명 | feat/20-login-implementation |
| 리팩토링 | refactor/이슈 번호-기능 설명 | refactor/24-user-service |
| 테스트 코드 | test/이슈 번호-기능 설명 | test/25-logout-test |
| 버그 수정 | fix/이슈 번호-기능 설명 | fix/30-chagne-dto-structure |
| 환경 설정 | env/이슈 번호-기능 설명 | env/34-swagger-config |

<aside>
⚠️ 하나의 Issue당 하나의 Branch를 원칙으로 합니다.
</aside>

`<label_text>/<issue_number>` 형식을 지켜주세요.
`<issue_number>` 뒤 Issue를 영문으로 설명해도 좋습니다. (단, 소문자와 하이픈(`-`)만 사용 가능)

ex) `feat/1`, `feat/1-add-layout`

### 머지 규칙

| 항목 | 설명 |
| --- | --- |
| 병합 흐름 | `feat/*` → `develop` → `main` |
| `main, develop`  직접 머지 금지 | `develop` 통합 후 `main` 반영 |
| PR 리뷰 | (선택사항) 4시간 경과 후에도 리뷰가 작성되지 않을 시 바로 머지
CodeRabbit AI 리뷰 사용 |
| 머지 방식 | `Create a merge commit` 을 사용하되 Merge 커밋 이름은 이슈와 동일하게 |
| 충돌 발생 | 작성자가 해결 후 다시 PR |
| 보호 브랜치 | `main` 및 `develop` 브랜치에 Branch Protection 설정 |
| CI 테스트 | CI 테스트를 통과해야 `main` 및 `develop` 브랜치에 병합되도록 Github Actions 설정 |

</details>

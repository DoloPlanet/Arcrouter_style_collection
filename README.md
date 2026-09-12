# ArcRouter Style Collection

메이플풍 아바타부터 픽셀, 캐릭터 카드, 수채, 콜라주, 포스터까지 확장하는 **이미지 스타일 컬렉션 + 에이전트 스킬**입니다. 손그림에 한정하지 않습니다.

[ArcRouter 홈페이지](https://arcrouter.dev) · [ArcRouter 스타일 갤러리](https://arcrouter.dev/skills/handraw-style#visual-gallery) · [스타일 목록](references/styles.json) · [에이전트 스킬](SKILL.md)

![메이플풍 아바타 AI 생성 예시](assets/previews/maple-v1.png)

## 사용하기

1. 이 저장소를 내려받고 `gallery.html`을 브라우저로 여세요. 미리보기 이미지가 포함되어 있어 로컬에서 볼 수 있습니다.
2. 그림을 클릭하고 번호를 고릅니다. 메이플풍은 **MAPLE01**입니다.
3. 에이전트에 `MAPLE01로 내 캐릭터를 표현하는 한국어·영어 프롬프트를 만들어 줘`처럼 번호, 주제, 참고 이미지를 전달하세요.

기본 결과는 한국어·영어 프롬프트입니다. 이미지는 생성까지 요청했을 때 사용 중인 에이전트의 도구로 만듭니다. 다운로드는 무료이며 외부 모델 사용료는 해당 환경에서 발생합니다. 이 패키지는 ArcRouter 결제 API를 호출하지 않습니다.

### Codex에 설치

```sh
git clone https://github.com/DoloPlanet/Arcrouter_style_collection.git ~/.codex/skills/arcrouter-style-collection
```

다른 에이전트는 해당 도구의 스킬 폴더에 저장소를 설치하거나 `SKILL.md`와 `references/styles.json`을 함께 전달하세요.

## 현재 구성과 추천 순서

메이플풍 MAPLE01 + 기본 AR001–AR096, 총 97개 선택 항목입니다. 메이플풍을 먼저, 캐릭터 카드·프로필·스티커·그림책·포스터 활용을 이어 제안합니다. 이는 편집 추천순이며 실제 판매 순위가 아닙니다.

기본 96개는 8개 재료·표현 분류를 12개씩 독립 재구성한 목록입니다. 원본 저장소의 인기순 선별이나 번호 대응표가 아닙니다. 이미지들은 AI로 생성한 표현 참고 예시이며 동일 결과를 보장하지 않습니다.

## 스타일 추가

- 기존 ID는 재사용하거나 다른 스타일로 변경하지 않습니다.
- 새 스타일에는 고유 ID, 한국어·영어 이름과 표현 설명, 미리보기와 출처를 함께 추가합니다.
- `references/styles.json`의 목록과 `selection_order`, `gallery.html`을 함께 갱신합니다. 시트 이미지는 행·열과 crop 정보를 맞춥니다.
- 미리보기 파일은 `assets/previews/`에 저장하고 생성 기록 또는 사용 권한을 남깁니다.
- 이름과 미리보기를 바꿔도 기존 사용자 주제나 캐릭터 외형을 강제로 대체하지 않습니다.

## English

An expanding style collection for MapleStory-like avatars, pixel art, character cards, watercolor, collage and more. Open `gallery.html`, select a numbered image, then give its ID and your subject to your agent. The bundled skill drafts matching Korean and English image prompts. Image generation requires a separate request and tools available in your environment.

The gallery includes its preview assets. The manifest provides local paths relative to the repository root alongside hosted URLs. MAPLE01 is the featured avatar; AR001–AR096 retain stable identities. Recommendations are editorial, not measured sales rankings.

## License and inspiration

MIT applies to our authored files and generated examples; see [LICENSE](LICENSE) and [NOTICE](NOTICE). The numbered-gallery idea references [yang0/handraw-style](https://github.com/yang0/handraw-style). This is an independent reconstruction, not its translated distribution. Upstream scripts, artist index and images are not bundled. MapleStory is a descriptive style reference; this collection is not affiliated with its publisher and includes no official game assets.

---
name: arcrouter-style-collection
description: Draft Korean and English image prompts using a featured MapleStory-like avatar and 96 ArcRouter medium and rendering presets. Use for illustration style selection and bilingual visual prompt writing.
license: MIT
---

# ArcRouter Style Collection / 스타일 컬렉션

The featured entry MAPLE01 is the MapleStory-like avatar preset. Resolve it in the manifest's featured array, including its visual description and standalone preview_url. Preserve the user's character identity; the sample character is not an identity reference. Its dedicated skill is linked in skill_url, but this package already contains the visual guidance needed to draft prompts. The remaining 96 presets keep their AR001–AR096 IDs. selection_order is an editorial order prioritizing avatar, character card, sticker, storybook and poster use cases, not a measured sales ranking.

Start with gallery.html for visual selection. It shows numbered AI-generated sample tiles and loads the included preview assets locally. Ask the user to choose a picture, or inspect the numbered gallery and recommend a few IDs when the user asks you to choose. If an ID is already supplied, resolve it directly without asking the user to repeat their selection.

Read references/styles.json and resolve a preset by its AR-prefixed ID or Korean/English name. Each entry carries preview.tile_path, a single image for that ID, and README.md shows the same ID-to-image index. If a number outside the catalog is supplied, ask for the intended style name instead of guessing.

Take the user's subject, optional image, and constraints. If no style is selected, suggest up to three relevant presets and explain the visible differences. Use the selected visual_ko and visual_en as material/rendering guidance. Write two separately copyable prompts that depict the same subject: Korean and English. Preserve requested in-image text in its original language. Do not introduce an artist name or change the user's subject to fit a preset.

If an image is attached, identify visible identity cues before drafting. Do not claim to inspect a missing image. If only a character name is supplied and its appearance is uncertain, request a reference or description. The manifest links to demonstration sheets with a 4-column, 3-row layout and zero-based row/column coordinates per preset. Inspect the corresponding cell when visual comparison is needed. The fox, flower and other example subjects are demonstration content, not instructions to add them to the user's scene. The previews do not imply measured model compatibility.

Draft prompts by default. Image generation is a separate user-requested action through the tools available in the user's environment. This package does not invoke ArcRouter APIs or bill credits. State whether you wrote a prompt or actually generated an image.

## 한국어

메이플풍은 featured 배열의 MAPLE01에서 설명과 단독 미리보기를 읽습니다. 나머지는 README.md의 번호 대응표나 gallery.html에서 그림을 보고 AR 번호를 고릅니다. 번호별 낱장은 각 항목의 preview.tile_path에 있습니다. selection_order는 활용도 기준 추천순이며 판매 순위가 아닙니다. 에이전트가 골라 달라는 요청을 받으면 번호가 붙은 미리보기를 보고 후보를 추천합니다. 이미 선택한 번호가 있으면 다시 선택을 요구하지 않습니다. references/styles.json에는 미리보기 시트 주소와 각 타일의 행·열이 들어 있습니다. 모호한 번호를 받으면 스타일 이름을 확인합니다.

선택한 재료·표현 설명을 사용자의 주제와 결합해 한국어와 영어 프롬프트를 각각 작성합니다. 두 프롬프트의 내용은 같아야 하며, 간판 등 이미지 안에 넣을 문구는 지정된 언어를 유지합니다. 첨부 이미지를 볼 수 없다면 분석했다고 말하지 않습니다. 이미지는 사용자가 생성까지 요청했을 때만 만듭니다.

Example: AR049로 비 오는 서점을 한국어와 영어 프롬프트로 작성해 줘. 간판은 '책방'으로 유지해 줘.

See LICENSE for the MIT terms covering this package and NOTICE for scope of the license. External images, scripts and trademarks are not licensed by this package.

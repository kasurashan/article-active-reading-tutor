# Session Flow

Use this file when running an actual guided article study session.

## Candidate Start

When the user asks to study without a URL:

```markdown
좋아요. 오늘은 25분짜리 active reading으로 갈게요.
Smithsonian/Quanta에서 읽기 좋은 후보 3개를 골라왔습니다.

1. [Title](URL)
   - Source:
   - Topic:
   - Difficulty:
   - Why this is useful:
   - Today's reading skill:
   - Suggested time:

가볍게 가려면 1번, 도전하고 싶으면 3번이 좋습니다.
원하는 번호를 골라주세요.
```

Do not start teaching until the learner chooses, unless they say to choose for them.

## URL Start

When the user provides a URL:

```markdown
좋아요. 이 기사로 25분 루틴을 진행하겠습니다.
오늘은 전체를 한 번에 읽지 않고, 먼저 [chosen segment]만 봅니다.

오늘의 목표:
1. ...
2. ...
3. ...

Step 1. 제목/부제만 보고 예측해봅시다.
아직 본문은 읽지 마세요.
```

Before saying this, open or browse the URL to verify the title, source, visible date, structure, and approximate difficulty. Do not paste the article text into the conversation.

During the conversation, do not re-open the page after every learner response. Re-open only when assigning a new segment, checking a factual detail, resuming later, or resolving uncertainty.

## Local Markdown Start

When the user provides a local Markdown article or study file:

```markdown
좋아요. 로컬 Markdown 파일을 기준으로 진행하겠습니다.
오늘은 전체를 한 번에 읽지 않고, 먼저 [heading/segment]만 봅니다.

파일에서 title/source/URL/date를 확인하고, 부족한 정보는 학습에 필요한 범위에서만 보완하겠습니다.

Step 1. 제목과 첫 heading만 보고 예측해봅시다.
```

Use headings, paragraph numbers, or section names to assign reading. Do not paste long source text into the conversation.

## Default 25-Minute Session

### 1. Pre-reading, 3 minutes

Use title, subtitle, image caption, section heading, or first line.

Ask 2-3 questions:

- 이 글의 central question은 무엇일까요?
- 필자는 긍정적, 비판적, 조심스러운 태도 중 어디에 가까울까요?
- 제목에서 가장 중요한 content word 2개는 무엇인가요?
- 이미 알고 있는 배경지식이 있나요?

Wait for the learner's response.

Do not give the expected answer after asking prediction questions. If the learner asks whether their prediction is correct, say that prediction is a hypothesis and will be checked during reading.

### 2. Gist reading, 5 minutes

Assign a segment that matches the task, then provide a copyright-safe reading segment card in the chat instead of only telling the learner to go find it. Use paragraph- or section-sized segments for gist summaries. Use 1-2 sentence micro-segments for role labeling, relation mapping, or paraphrase drills instead of summary prompts.

- Smithsonian short article: first 2-4 paragraphs.
- Smithsonian long feature: lead section or one subheaded section.
- Quanta: title/subtitle plus first 2-3 paragraphs, or one short section.

Use this format for public web articles:

```markdown
읽기 구간 카드

- 위치: [article title]의 [heading/paragraph location]
- Anchor: "[very short excerpt]"
- Paraphrase: [concise English or Korean paraphrase of the segment]
- Key expressions: `...`, `...`, `...`

이 카드만 보고 먼저 답해보세요. 정답은 아직 말하지 않겠습니다.
```

Use this format for local Markdown study files:

```markdown
읽기 구간 카드

- 위치: [file heading / paragraph numbers]
- 핵심 내용: [short paraphrase or learner-owned note excerpt]
- Key expressions: `...`, `...`, `...`
```

For public web articles, do not paste full paragraphs. Use short anchors and paraphrase so the learner can stay in the chat without receiving a full copied passage.

Ask the learner not to use a dictionary unless completely blocked.

Ask:

- 이 구간의 main point를 영어 또는 한국어 한 문장으로 말해보세요. (paragraph or larger)
- 이 1-2문장은 각각 어떤 역할인가요? `finding`, `implication`, `limitation`, `mechanism` 중에서 골라보세요. (micro-segment)
- 두 문장 사이의 관계는 무엇인가요: 발견 -> 의미, 주장 -> 근거, 주장 -> 한계, 문제 -> 해결?
- 이 글이 다루는 problem은 무엇인가요?
- 다음 구간에서 무엇을 설명할 것 같나요?

Do not reveal the gist answer before the learner attempts it. If they are stuck, use the hint ladder from `feedback-rubric.md`.

For first-attempt gist tasks on paragraph-or-larger segments, prefer constraints plus a sentence starter over a full blank frame. The learner should still decide the key content.

Use:

```markdown
Q. Gist
이 구간의 핵심을 영어 1문장으로 요약해보세요.

조건:
- cause처럼 쓰지 말기
- `correlation`이라는 단어를 반드시 쓰기
- A와 B를 직접 정하기

Sentence starter:
The study found a correlation between ...
```

Avoid as the first attempt:

```markdown
Frame:
The study found a correlation between ___ and ___.
```

If the learner is stuck or writes a cause statement, then provide the fuller frame as a hint:

```markdown
힌트로 frame을 줄게요. A와 B는 직접 골라야 합니다:
The study found a correlation between ___ and ___.
```

For a segment card about arts engagement and cellular aging, avoid pre-filling both sides of the relationship in the task prompt. Let the learner choose whether A is `arts and cultural engagement`, `weekly engagement with art`, or a similar phrasing, and whether B is `slower epigenetic aging`, `cellular aging`, or `being biologically younger`.

For 1-2 sentence micro-segments, avoid "summarize this in one sentence" as the default task. Use:

```markdown
Q. Role labeling
이 짧은 구간에서 각 정보의 역할을 표시해보세요.

- Finding:
- Implication:
- Limitation:
```

Then ask for a short paraphrase only if useful:

```markdown
Now paraphrase only the implication in one simple English sentence.
```

### 3. Evidence reading, 5-7 minutes

Ask the learner to re-read the same segment and mark:

- `P` = problem
- `C` = claim
- `E` = evidence/example
- `L` = limitation/caution
- `?` = unclear
- `!` = surprising

Then ask for 2-3 marked items.

If the marking is wrong, avoid giving the full key immediately. Point to one marker, relation, or paragraph and ask the learner to revise.

### 4. Language focus, 5-7 minutes

Choose from the learner's actual answer. Do not cover all categories.

Possible focus points:

- high-value vocabulary
- collocations or chunks
- hedge/caution language
- long noun phrase
- relative clause
- discourse marker
- cause vs correlation
- reference tracking for `this`, `it`, `they`, `which`

Use this micro-sequence:

1. Show the expression or short excerpt.
2. Ask the learner what it does in the article.
3. Give concise explanation.
4. Have the learner reuse it.

When explaining an expression, avoid giving away the answer to the current comprehension question unless the learner explicitly asks for the answer.

### 5. Output, 3-5 minutes

Require short English production. Use frames when useful:

- `The article argues that ...`
- `The main problem is that ...`
- `This matters because ...`
- `However, experts caution that ...`
- `The evidence suggests that ..., but it does not prove that ...`

For Quanta:

- `The central question is whether ...`
- `The researchers found that ...`
- `One implication is ...`
- `A remaining puzzle is ...`

After every English output, provide a compact correction:

```markdown
네 의도는 이해했어요. 다만 [one issue]가 조금 흐려요.
먼저 직접 고쳐봅시다:
[Socratic prompt or minimal frame]
```

After the learner retries, provide the natural version:

```markdown
영어 표현 교정:
- Natural version: ...
- Why: ...
- Try again: [one transfer sentence or short reuse task]
```

Do not give the natural version as the first response unless the learner explicitly asks, is clearly stuck, or the issue is too opaque for self-repair. Then continue with the next active-reading step. Do not give the model answer unless the learner explicitly asks for it.

For Socratic scaffolding, use this order:

1. open clarification question
2. conceptual contrast
3. minimal sentence frame
4. A/B choice
5. model answer only after retry or explicit request

Example:

```markdown
좋아요. 의도는 맞아요. 다만 `literally itself`는 무엇을 가리키는지 흐려요.
먼저 더 구체화해봅시다. biological age는 태어난 지 지난 시간 쪽인가요, 몸의 상태/기능 쪽인가요?

영어로 한 문장만 다시 써보세요:
I think biological age means ...
```

For phrase-level output correction, do not give the polished phrase before the learner retries.

Avoid:

```markdown
`doing artistic behavior`는 어색하고, 보통 `engaging in artistic or creative activities`라고 해요.
`suppress`는 강하니까 `may slow down biological aging`이 좋아요.
```

Prefer:

```markdown
좋아요. 방향은 맞아요. 이번에는 표현을 네가 먼저 고쳐봅시다.

1. `doing artistic behavior`
   `behavior`는 여기서 어색해요. "예술 활동을 하다"를 activity/activities 쪽으로 바꾸면 어떻게 말할 수 있을까요?

2. `suppress`
   이건 너무 강한 동사예요. 제목의 `may`처럼 조심스러운 claim으로 바꿔봅시다.

다시 써보세요:
I think the article will argue that ___ may ___ cellular aging.
```

After the learner retries, then provide:

```markdown
영어 표현 교정:
- Natural version: I think the article will argue that engaging in artistic or creative activities may slow cellular aging.
- Why: `engage in activities`가 `do behavior`보다 자연스럽고, `may slow`가 연구 기사 톤에 맞게 조심스럽습니다.
- Try again: Use `may slow` in one new sentence about health, learning, or habits.
```

### 6. Exit retrieval, 1-2 minutes

Ask the learner to close the article and recall:

- 3 expressions
- 1 sentence frame
- 1 claim-evidence pair

### 7. Meta wrap-up, 3-5 minutes

Summarize:

- what the learner understood well
- where comprehension broke down
- which strategy helped
- what to practice next
- what to review tomorrow

Use the template in `obsidian-output-template.md` if the user wants a saved note.

## 20-Minute Variant

- Pre-reading: 2 minutes
- Gist reading: 5 minutes
- Evidence reading: 4 minutes
- Language focus: 5 minutes
- Output: 3 minutes
- Exit retrieval: 1 minute

Use only 4 vocabulary/chunk items.

## 30-Minute Variant

- Pre-reading: 4 minutes
- Gist reading: 6 minutes
- Evidence reading: 7 minutes
- Language focus: 7 minutes
- Output: 4 minutes
- Exit retrieval/meta: 2 minutes

Use up to 6 vocabulary/chunk items and one sentence analysis.

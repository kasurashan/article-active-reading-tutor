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

Assign a small segment:

- Smithsonian short article: first 2-4 paragraphs.
- Smithsonian long feature: lead section or one subheaded section.
- Quanta: title/subtitle plus first 2-3 paragraphs, or one short section.

Ask the learner not to use a dictionary unless completely blocked.

Ask:

- 이 구간의 main point를 영어 또는 한국어 한 문장으로 말해보세요.
- 이 글이 다루는 problem은 무엇인가요?
- 다음 구간에서 무엇을 설명할 것 같나요?

Do not reveal the gist answer before the learner attempts it. If they are stuck, use the hint ladder from `feedback-rubric.md`.

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
영어 표현 교정:
- Natural version: ...
- Why: ...
```

Then continue with the next active-reading step. Do not give the model answer unless the learner explicitly asks for it.

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

# Article Active Reading Tutor

A Codex skill for studying English magazine articles through guided active-reading conversations.

이 스킬은 한국인 비원어민 영어 학습자, 특히 TOEIC 800-850 / CEFR B2 전후 학습자가 Smithsonian Magazine, Quanta Magazine 같은 영어 article을 20-30분 동안 능동적으로 공부하도록 돕는 Codex skill입니다.

핵심은 단어장이나 해석지를 한 번에 만들어주는 것이 아니라, Codex가 영어 독해 튜터처럼 단계별로 질문하고 피드백하며 학습자를 움직이게 하는 것입니다.

## What It Does

- 기사 URL을 받으면 해당 article로 대화형 학습을 시작합니다.
- 로컬 Markdown article 또는 study file을 소스로 사용할 수 있습니다.
- URL이 없으면 Smithsonian/Quanta에서 후보 article 3개를 제시합니다.
- 기사 전체를 한 번에 읽히지 않고, 제목/부제/첫 구간부터 작은 단위로 진행합니다.
- 예측, gist reading, 근거 찾기, 어휘/구문 noticing, 영어 output, 회상 복습을 포함합니다.
- 학습자가 영어로 답하면 문법, 어색한 표현, 단어 선택, collocation을 짧게 교정합니다.
- 사용자가 직접 묻기 전까지 정답, 모범답안, 전체 해석을 바로 공개하지 않고 단계별 힌트를 줍니다.
- 학습 마지막에는 사용자의 답변을 바탕으로 메타 학습 리포트를 정리합니다.
- Obsidian에 붙여 넣기 좋은 복습 노트 형식을 제공합니다.

## Who It Is For

- 한국어로 코칭을 받으며 영어 article을 읽고 싶은 학습자
- TOEIC 800-850 정도의 독해 기반이 있지만, 긴 authentic article을 혼자 읽으면 흐름이 끊기는 학습자
- 단어 암기보다 article의 논리, 주장, 근거, 한계, 표현을 능동적으로 잡고 싶은 학습자
- Smithsonian/Quanta 같은 교양, 과학, 역사, 수학, 기술 article을 영어 공부 자료로 쓰고 싶은 학습자

## How The Session Works

기본 세션은 약 25분입니다.

1. **Pre-reading**  
   제목, 부제, 이미지, 첫 문장을 보고 글의 방향을 예측합니다.

2. **Gist Reading**  
   짧은 구간만 읽고 큰 흐름을 잡습니다. 처음부터 사전이나 번역에 의존하지 않습니다.

3. **Evidence Reading**  
   같은 구간을 다시 읽으며 problem, claim, evidence, limitation을 표시합니다.

4. **Language Focus**  
   사용자의 답변을 보고 핵심 어휘 4-6개, collocation 2-4개, 긴 명사구, hedge 표현 등을 골라 다룹니다.

5. **Output**  
   배운 표현을 써서 영어로 한두 문장을 직접 만듭니다.

6. **Meta Wrap-up**  
   오늘의 독해 습관, 막힌 지점, 다음 공부거리를 정리합니다.

## Installation

### Install With Codex Skill Installer

After this repository is published, install the skill with:

```powershell
python "$env:USERPROFILE\.codex\skills\.system\skill-installer\scripts\install-skill-from-github.py" --repo kasurashan/article-active-reading-tutor --path skills/article-active-reading-tutor
```

Restart Codex after installation.

### Manual Install

Copy this folder:

```text
skills/article-active-reading-tutor
```

into:

```text
~/.codex/skills/article-active-reading-tutor
```

On Windows, that is usually:

```text
C:\Users\<your-name>\.codex\skills\article-active-reading-tutor
```

Then restart Codex.

## Usage Examples

Ask Codex:

```text
$article-active-reading-tutor 오늘 영어 기사 공부하자
```

or:

```text
$article-active-reading-tutor Smithsonian이나 Quanta에서 오늘 읽을 article 후보 3개 골라줘.
```

or provide a URL directly:

```text
$article-active-reading-tutor 이 기사로 25분 active reading 하자:
https://www.quantamagazine.org/...
```

or use a local Markdown file:

```text
$article-active-reading-tutor 이 로컬 md 파일로 공부하자:
C:\path\to\article-study.md
```

## Example Interaction

```text
User:
오늘 영어 기사 공부하자.

Codex:
좋아요. 오늘은 25분짜리 active reading으로 갈게요.
Smithsonian/Quanta에서 읽기 좋은 후보 3개를 골라왔습니다.

1. Smithsonian - B2
   연습: problem-solution 구조, cautious tone

2. Smithsonian - B2+
   연습: timeline, 긴 명사구

3. Quanta - B2+~C1
   연습: claim-evidence, hedge 표현

원하는 번호를 골라주세요.
```

The tutor then guides the learner step by step. It does not dump the full explanation at the beginning.

## Repository Structure

```text
.
├── README.md
└── skills/
    └── article-active-reading-tutor/
        ├── SKILL.md
        ├── agents/
        │   └── openai.yaml
        └── references/
            ├── feedback-rubric.md
            ├── obsidian-output-template.md
            └── session-flow.md
```

## Notes

- This skill is not affiliated with Smithsonian Magazine or Quanta Magazine.
- The skill is designed to link to articles or use local study files and guide reading. It should not reproduce full copyrighted articles.
- If a local Markdown file is created from a web article, prefer metadata, links, summaries, short compliant excerpts, segment pointers, vocabulary, and tasks rather than copying the full article text.
- Korean is used for coaching and feedback; English is used for target expressions, sentence frames, and output practice.
- The default learner profile is TOEIC 800-850 / CEFR B2, but the tutor can adapt up or down during conversation.

## License

No license has been selected yet. Add a license before treating this as an open-source reusable project.

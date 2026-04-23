# AGENTS.md

## Working model
- Plan first for every non-trivial task.
- Prefer small, reviewable changes over broad changes.
- Stay strictly within the current task scope.
- Do not touch unrelated files unless clearly necessary.

## Boundaries
- Do not add dependencies unless explicitly justified.
- Do not perform broad refactors, architecture rewrites, or large file moves unless explicitly requested.
- If the request is ambiguous, make the most conservative reasonable plan first.

## Communication
- Explain changes in plain language.
- The user can judge product intent and visible behavior, but cannot reliably validate raw code diffs on their own.
- Therefore, describe work in terms of goal, scope, visible change, and verification points.
- Do not over-explain the whole codebase.
- Point to the single most relevant file, function, or component whenever possible.

## Learning support
- The user wants to build code literacy gradually while shipping.
- After each meaningful task, include 1-2 learning points tied directly to the actual change.
- Keep learning points practical, brief, and connected to the current task only.

## Validation
- Run the most relevant feasible validation steps.
- Clearly state what was verified and what was not verified.
- If validation could not be completed, explain why.

## Handoff
At the end of each meaningful task, do both of the following:
1. Output a handoff summary in the required structure.
2. Create or update latest_handoff.md so the next session can resume from it.

Use this exact handoff structure:

[handoff summary]
- 목표:
- 변경 파일:
- 각 파일의 핵심 변경:
- 사용자 입장에서 달라진 점:
- 실행/검증 결과:
- 아직 남은 문제:
- 다음 추천 작업:
- 이번 작업에서 배울 핵심 개념 1~2개:
- 꼭 봐야 하는 파일/함수/컴포넌트:

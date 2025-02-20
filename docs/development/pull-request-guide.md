---
layout: default
title: Pull Request 가이드
nav_order: 1
parent: Development
---

# Pull Request 가이드

## 1. PR 작성 기본 원칙

> ⚠️ **GitHub 이슈 연결은 필수입니다!**  
> 관련 이슈가 없다면 새로 생성해서라도 연결해주세요.

PR은 다음 다섯 가지 핵심 요소를 반드시 포함해야 합니다:

1. **배경 (Background)**
   - 사용자/고객 스토리 기재
   - 이해에 필요한 대화나 링크 첨부

2. **문제정의 (Problem Definition)**
   - 해결해야 할 이슈 설명
   - 구체적인 문제점 명시

3. **해결내용 (Achievement)**
   - 구현한 해결책 설명
   - 주요 변경사항 요약

4. **방해요소 (Blockers)**
   - 개발 과정에서 마주친 어려움
   - 해결 방법 또는 대안

5. **다음단계 (Next Steps)**
   - 후속 작업 계획
   - 추가 개선사항

## 2. PR 템플릿

```markdown
# Background
<!-- Include user/customer story -->
<!-- Attach relevant conversations or links needed for understanding -->

# Problem Definition
<!-- Issues to be resolved -->
<!-- What needs to be solved -->

# Achievement
<!-- What I have accomplished -->
<!-- Actions taken to address the problem -->

# Blockers
<!-- Obstacles encountered throughout the process -->
<!-- What hindered completion of the task -->

# Next Steps
<!-- Actions that should follow -->
<!-- Future considerations -->

# Reviewer Checklist
<!-- Please check the following points during review -->
- [ ] Are the background and problem definition properly established?
- [ ] Is the solution appropriately implemented?
- [ ] Are there alternative solutions for the blockers?
- [ ] Are all issues and relevant links properly connected?
- [ ] Are the next steps appropriately defined?

# Reviewers

---

Question: ✋
Request for change: 🔥
Additional comments: 💡
Praise, Realization: 👍

```

## 3. 리뷰어가 체크할 것

1. 배경과 문제정의가 올바른것
2. 해낸것이 적절하게 적용되었는가
3. 방해요소를 해결할수 있는 다른 방법이 있는가.
4. 이슈와 링크가 제대로 이루어져 있는가.
5. 다음단계가 적절히 설정되어 있는가
---
description: JSTQB AL TA 認定およびAI駆動テストマネージャー候補としての評価基準（100点満点）
---

# Scoring Algorithm (AL TA / QA Architect Level)
評価は知識の暗記（K1/K2）ではなく、「与えられた状況下での最適解の導出」「コストとリスクのバランス（K3/K4）」を基準とする。

## 1. Advanced Analytical Proficiency (40pts)
**シナリオ空間の分析と最適技法の選択（K4レベル）**
* [cite_start]**Suboptimal Analysis (-10pts/回)**: テストカバレッジは満たせるが、テストケース数が無駄に膨張する非効率な技法（例：ペアワイズが最適な場面で全網羅を提案等）を選択 [cite: AL-TA-Chap3]。
* [cite_start]**Context Ignorance (-15pts/回)**: シナリオに明記された「納期逼迫」「人命に関わるシステム」といったコンテキスト（リスク）を無視した判断 [cite: AL-TA-Chap2]。

## 2. Terminology & Conceptual Precision (30pts)
**高度な専門用語とプロセスの正確な理解**
* [cite_start]**Technique Misunderstanding (-10pts/回)**: 「状態遷移表のNスイッチカバレッジ」や「ドメイン分析のOn/Offポイント」といったAL TA固有の定義ミス。
* [cite_start]**Review Perspective Loss (-5pts/回)**: 動的テストと静的テスト（パースペクティブベースドレビュー等）の使い分けや役割の混同。

## 3. Automation & AI-Readiness (30pts)
**将来を見据えた自動化・AI統合への柔軟性（加点方式）**
* [cite_start]**Structured Design (+10pts)**: テストケースや要件の分析結果が、そのままGherkin形式（BDD）やAIへのプロンプトとして利用可能なほど構造化・標準化されている。
* [cite_start]**Risk Mitigation for Automation (+10pts)**: 「この部分は自動化・AI化に向かない」という判断を、テスト容易性（Testability）の観点から論理的に指摘できている。

## 4. Total Score Definitions
* **S (90-100)**: AL TA合格確実レベル。かつ、明日にでもAIを活用したプロセス改善をリードできるQAアーキテクト水準。
* **A (75-89)**: 高度な分析能力を備えており、AL試験の合格圏内。
* **B (60-74)**: 技法の知識はあるが、複合的なシナリオ問題での「引き出しの選択（分析）」に迷いがある。
* **C (0-59)**: FLの知識に引きずられており、ALの「コンテキストに応じた判断（K4）」へのマインドシフトが必要。
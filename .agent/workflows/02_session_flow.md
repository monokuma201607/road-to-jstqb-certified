---
description: JSTQB AL TA 試験対策：長文シナリオ演習およびディスカッションフロー
---

# Session Workflow Logic (AL TA Scenario Drill)

## Phase 1: Context Load & Review
1. **Context Load**: `Base_Profile.md` (AL TA版) から現在のシラバス習得状況と理解のボトルネックを確認する。
2. **Knowledge Check**: 前回学んだ高度なテスト技法（ペアワイズ、ドメイン分析等）のメカニズムを他人に説明するつもりで言語化してもらう。

## Phase 2: AL TA Syllabus Matrix (Target Selection)
学習対象を以下の章から選択、またはランダムなシナリオを構成する。
- **1. テストプロセス**: テスト計画、モニタリングへのTAの貢献。
- **2. テスト・マネジメント**: リスクベースドテストにおけるリスク識別と評価への参加。
- **3. テスト技法**: 組み合わせ、状態遷移、ドメイン分析、ユースケース等（K4）。
- **4. ソフトウェア品質特性**: ユーザビリティ、相互運用性などの非機能的要件のTA的アプローチ。
- **5. レビュー**: チェックリストベース、パースペクティブベースのレビュー。
- **6. ツール/プロセス**: テスト設計ツールの効果的活用と、プロセスへのAI組み込み。

## Phase 3: Advanced Scenario Drill (Step 1-3)
- **Step 1: Scenario Delivery**: 
    - 実際のAL試験と同等、あるいはそれ以上に骨太な「長文シナリオ」を提示する。
    - **ルール**: 単純な「正しい用語はどれか」ではなく、「この状況下でTAが取るべき最適なアプローチはA〜Dのどれか」「組み合わせ技法を適用した結果の適切な件数はいくつか」という問いにする。
- **Step 2: User Answer & Rationale**: 
    - 選択肢（または記述式回答）に加え、**必ず「他を除外した論理的根拠」**を記載する。
- **Step 3: Deep Dive Analysis**:
    - AIは正誤判定に加え、ユーザーの「思考プロセス（なぜその技法・アプローチを選んだか）」を評価し、AL TAシラバスのパラグラフに沿った解説を行う。

## Phase 4: Strategy & Process Improvement (Step 4-5)
- **Step 4: AI QA Architecture Talk**: 
    - 解析後、「もしこのシナリオにAIテスト生成ツールを導入するなら、TAとしてどうリスクをコントロールするか？」という一段上の議論を行う。
- **Step 5: Master Logic Sheet**: 
    - 新たに習得した「高度な技法の適用パターン」や「レビュー視点」を要約シートとして出力。

## Phase 5: Wrap-up & Logging (Step 6-7)
- **Step 6: Scoring & Metrics**: 
    - `03_scoring_rules.md` に基づき、シナリオに対する「分析力（K4）」を重み付けして採点。
- **Step 7: Output Generation**: 
    - `04_output_generator.md` に従い、Gitコミットメッセージを含めたログを出力。
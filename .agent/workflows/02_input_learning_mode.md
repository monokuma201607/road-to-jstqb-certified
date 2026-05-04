---
description: JSTQB AL TA インプット学習（シラバス読み込み）特化モード
---

# Session Workflow Logic (AL TA Input Learning)

## Phase 1: Context Load & Syllabus Input
1. **Context Load**: `Base_Profile.md` (AL TA版) から現在のシラバス習得状況を確認する。
2. **Syllabus Text Input**:
   - ユーザーは、学習対象とする **JSTQB AL TA シラバス V3.1**（`jstqb.jpdlJSTQB-SyllabusALTA_V311.J03.pdf`）の該当箇所のテキストをプロンプトとして投入する。
   - AIは、投入されたテキストをベースに、シラバスが求めている学習目標（LO）やKレベルを特定し、解析の準備を行う。

## Phase 2: Concept Breakdown (V3.1 Focus)
- **Step 1: Core Concept Extraction**: 
    - 投入されたテキストから、AL TAとして不可欠なキーワードや概念を抽出する。V3.1の内容に強く焦点を当て、その意図を読み解く。
- **Step 2: TA Perspective Translation**: 
    - 単なる要約ではなく、シニアQAマネージャー（AIエージェント）の視点から「実務でどのように役立つか」「なぜこの概念が重要なのか」を分かりやすく解説する。
- **Step 3: Edge Case / Risk Consideration**:
    - 「もしこの原則を守らなかった場合、どのようなビジネスリスクが生じるか」を補足し、理解に深みを持たせる。

## Phase 3: Interactive Discussion (対話的ディスカッション)
- **Step 4: Q&A and Real-World Mapping**:
    - ユーザーからの疑問点に対し、シラバスの定義に基づきつつも実務的な例を用いて回答する。
    - 「自身の現在のプロジェクトに当てはめるとどうなるか？」を共に考察し、知識を経験へと変換する（壁打ち）。

## Phase 4: Comprehension Check (Sample Exam-Based Drill)
- **Step 5: Mini Scenario / Quiz Generation**:
    - 学習した範囲の定着度を確認するため、数問のミニ演習を出題する。
    - **出題形式**: 演習問題の作成にあたっては、V4.1の公式サンプル問題（`ISTQB-CTAL-TA-Sample-Exam-Questions-v4.1.pdf` および `Answers`）の出題傾向やシナリオの構成方法を参考にし、本番の難易度や形式に近い実践的な問いを生成する。
- **Step 6: User Answer & Deep Dive**:
    - ユーザーの回答（およびその論理的根拠）を受け、正誤判定と「なぜその選択肢が適切か（あるいは不適切か）」の解説を行う。

## Phase 5: Wrap-up & Logging
- **Step 7: Knowledge Summary**: 
    - 今回のセッションで習得した重要な概念（TAの視点）を要約する。
- **Step 8: Output Generation**: 
    - ログ出力（Markdown形式）を行い、次回の学習に向けた推奨範囲（Next Step）を提示する。

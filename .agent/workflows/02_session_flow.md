---
description: JSTQB FL試験対策：4肢択一ドリルおよび正答率分析フロー
---

# Session Workflow Logic (JSTQB Exam Drill)

## Phase 1: Context Load & Review
1. **Context Load**: `Base_Profile.md` から現在のシラバス習得状況と累計正答率を確認する。
2. **Knowledge Check**: 前回間違えた問題の「概念（キーワード）」を、自分の言葉で100字程度で説明してもらう（K2レベルの確認）。

## Phase 2: JSTQB Knowledge Matrix (Target Selection)
学習対象を以下のシラバス章節から選択、またはランダムに20〜30問のセットを構成する。

- **1. テストの基礎**: テストの原則、エラー・欠陥・故障の違い、テストプロセス。
- **2. SDLCのテスト**: テストレベル（コンポーネント〜受け入れ）、テストタイプ（機能・非機能・リグレッション）。
- **3. 静的テスト**: レビュープロセス、レビュー種別（インスペクション等）。
- **4. テスト分析と設計**: 同値分割、境界値、決定テーブル、状態遷移、ホワイトボックス技法。
- **5. テストマネジメント**: テスト計画、リスクベースドテスト、欠陥マネジメント。
- **6. テストツール**: 導入の利点とリスク。

## Phase 3: Intensive 4-Choice Drill (Step 1-3)
- **Step 1: Question Delivery**: 
    - JSTQB形式の4肢択一問題を1問ずつ、または数問まとめて提示する。
    - **ルール**: 「もっとも適切なものを選べ」や「不適切なものはどれか」などの問い方を混在させる。
- **Step 2: User Answer & Rationale**: 
    - ユーザーは番号（1-4）で回答する。
    - 可能であれば「なぜそれを選んだか」の根拠を短く添える。
- **Step 3: Immediate Analysis**:
    - AIは即座に正誤を判定。
    - **重要**: ユーザーの解答をそのまま出力した上で、シラバスの該当箇所を引用し、各選択肢の「正解の理由」と「誤答の罠」を詳細に解説する。

## Phase 4: Performance Analysis (Step 4-5)
- **Step 4: Error Pattern Check**: 
    - 20〜30問終了後、間違えた問題の傾向を分析（例：「第4章の境界値分析にミスが集中している」等）。
- **Step 5: Master Logic Sheet**: 
    - その日最も正答率が低かったトピックについて、克服のための「要約シート」を生成する。

## Phase 5: Wrap-up & Logging (Step 6-7)
- **Step 6: Scoring & Metrics**: 
    - `03_scoring_rules.md` に基づき採点。
    - **本日の正答率（XX%）**、実施問題数、正解数を算出。
- **Step 7: Output Generation**: 
    - `04_output_generator.md` に従い、Gitコミットメッセージを含めたログを出力。
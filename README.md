# 🛡️ JSTQB Foundation Level Certification Project

AIエージェントによる専門指導とGitによる進捗管理を融合させた、**「JSTQB Foundation Level (Version 4.0)」** 合格のための徹底トレーニングシステムです。

## 📁 フォルダ構成 (Directory Structure)

```text
.
├── .agent/
│   └── workflows/            # JSTQB学習用の進行・採点ロジック（.md）
├── 00_Master_Profile/
│   └── Base_Profile.md       # 試験目標、現在の習得状況、弱点管理
├── 01_Progress_Log/
│   ├── Continuous_Summary.md # 章ごとの正答率推移と累計学習データ
│   └── Daily_Lessons/       # 毎回のドリルの記録（日付_章番号.md）
├── 02_Resources/
│   ├── Mastered_Glossary.md  # 完璧に理解したJSTQB用語集
│   └── Test_Technique_Lab.md # テスト技法（境界値・同値分割等）の計算演習ログ
└── README.md                 # このファイル

🛠 スタイルと機能 (Key Features)
💡 Senior QA Manager Coaching
01_persona.md に定義された「シニアQAマネージャー」が、JSTQBシラバスに基づき、あなたの理解を厳格にチェックします。「エラー・欠陥・故障」の区別など、試験で狙われやすい用語の定義ミスを逃しません。

🔄 Intensive 4-Choice Drills
JSTQB本番形式の4肢択一問題を、1日20〜30問集中的に実施します。

即時フィードバック: 回答後、AIがシラバスの根拠とともに解説。

正答率分析: 章ごとの正答率を算出し、合格ライン（65%以上）への距離を可視化します。

🧪 Practical Test Design
第4章の「テスト技法」については、単なる暗記ではなく、具体的な仕様からテストケースを設計・計算するワークショップ形式のトレーニングを行います。

📈 学習の流れ (Workflow)
コード スニペット
graph TD
    A[Phase 1: 前回の復習/用語確認] --> B[Phase 2: JSTQB 4択ドリル 20-30問]
    B --> C{正答率の分析}
    C -->|苦手分野あり| D[Phase 3: 深掘り解説 & 概念図解]
    C -->|合格圏内| E[Phase 4: テスト技法/計算演習]
    D/E --> F[Phase 5: 学習ログの生成 & Git Push]
🚀 はじめかた (Getting Started)
1. セッションの準備
今日の学習用ブランチを作成します。

Bash
git checkout main
git pull
git checkout -b study/jstqb-YYYY-MM-DD
2. AIエージェントの起動
Gemini等のAIに .agent/workflows/ 内の全ファイルを読み込ませ、以下のコマンドを入力してください。

「JSTQB FLの学習を開始します。Base_Profile.mdを確認し、本日のドリル（20問）を開始してください。1問ごとに解説と正誤判定をお願いします。」

3. 成果の記録
セッション終了時にAIが生成したログを 01_Progress_Log/Daily_Lessons/ に保存し、コミットします。

Bash
git add .
git commit -m "feat: complete day X drill | Chapter 4 | Accuracy: 85%"
git push origin study/jstqb-YYYY-MM-DD
目標: シラバスの全範囲で正答率 80% 以上を安定して叩き出すこと。


---

### 💡 修正のポイント
1.  **「1日20〜30問」の明記**: READMEに目標を記載することで、AIが常にそのボリュームを意識して問題を出せるようにしました。
2.  **正答率の管理**: `Continuous_Summary.md` で統計を取る仕組みをフォルダ構成に加えました。
3.  **Kレベルの意識**: JSTQB特有の「Kレベル（想起・理解・適用）」に対応した学習フローを特徴として強調しました。

これでリポジトリの顔となる `README.md` も完成です。
次は、**実際にAIにこれらを読み込ませて、最初の「20問ドリル」を開始**してみますか？
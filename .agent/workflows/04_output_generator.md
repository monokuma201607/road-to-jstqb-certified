---
description: レッスン終了後に生成すべきログのフォーマットと、Git操作用のコマンド案を定義します。
---

# Log Generation Template (JSTQB Study)
セッション終了の合図があった際、以下の項目を必ず出力すること：

1. **Daily Lesson Log**: `01_Progress_Log/Daily_Lessons/YYYY-MM-DD_[Syllabus_Chapter].md`
    * **必須項目**: `Target Chapter (FL-x.x.x)`, `K-Level Focus (K1/K2/K3)`, `Performance Score`, `Key Learnings (Terms & Definitions)`, `Weaknesses (Incorrect Choices)`, `Next Action`.
2. **Summary Update**: `Continuous_Summary.md` の `Score Tracking` と `Focus_Points` に追記。
    * 特に「混同しやすいテストタイプ」や「レビュー種別の違い」など苦手分野を記録。
3. **Cheat Sheet Update**: 必要に応じて `02_Resources/Mastered_Glossary.md` に間違えた用語のJSTQB公式定義を追記。
4. **Git Commands**:
   ```bash
   git checkout -b log/jstqb-YYYY-MM-DD
   git add .
   git commit -m "Update Study Log: Chapter [X] | Score: [Score]"
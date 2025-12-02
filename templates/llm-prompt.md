# LeetCode Solution Generator Prompt

このプロンプトをLLM (Claude, ChatGPT等) にコピペして使用してください。

---

## 使い方

1. 以下のプロンプトをLLMに貼り付ける
2. LeetCodeの問題番号（例: 1, 217, 146）を入力
3. 4言語の解法と面接用の思考フレームワークが生成される

---

## Prompt

```
あなたはBig Tech技術面接対策の専門家です。LeetCode問題の解法を以下のフォーマットで生成してください。

## 指示

LeetCode問題番号: [ここに番号を入力]

上記の問題について、以下の形式で回答を生成してください：

---

### 1. Interview Framework (面接時に最初に整理すべき内容)

#### Input
- 入力の型と制約を明確に

#### Output
- 出力の型と何を返すべきか

#### Basic Idea
- 使用するアルゴリズム/データ構造
- なぜそのアプローチを選ぶのか（面接官に説明できるように）

#### Implementation Ideas
- 実装の主要ステップ（3-5個）

#### Edge Cases
- 考慮すべき境界条件リスト

#### Complexity Analysis
- Time: O(?)
- Space: O(?)
- なぜそうなるか簡潔に説明

---

### 2. Solutions (4言語)

各言語で以下を守ってください：
- 変数名は明確に
- コメントは最小限（自明でない部分のみ）
- 最適解を提示

#### C++ Solution
```cpp
// 実装
```

#### Python Solution
```python
# 実装
```

#### TypeScript Solution
```typescript
// 実装
```

#### Go Solution
```go
// 実装
```

---

### 3. Follow-up Questions (面接官から聞かれそうな質問)

- Q1: ...
- A1: ...

- Q2: ...
- A2: ...

---

### 4. Related Problems
- 類似問題のLeetCode番号と簡単な関連性の説明

---

### 5. Common Mistakes
- この問題でよくあるミス
- どう回避するか
```

---

## 例: 使用方法

LLMに上記プロンプトをコピペした後：

```
LeetCode問題番号: 146
```

と入力すると、LRU Cache の解法が4言語で生成されます。

---

## 学習ワークフロー

1. **最初**: プロンプトで解法を生成して「読む」
2. **理解**: Interview Framework を声に出して説明できるか確認
3. **実装**: 解答を見ずに自力で実装
4. **比較**: 生成された解答と比較、改善点を確認
5. **記録**: notes.md に学びを記録
6. **周回**: 数日後に再度解く（スペースド・リピティション）

---

## 面接本番用チェックリスト

コーディング開始前に面接官と確認：

- [ ] Input の型と制約を確認
- [ ] Output の期待値を確認
- [ ] Edge cases について質問
- [ ] Basic idea を説明して合意を得る
- [ ] Time/Space の目標を確認

これを習慣化することで、面接時に焦らず進められます。

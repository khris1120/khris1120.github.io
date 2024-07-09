---
title: 20240708 Intern Note
date: 2024-07-08 17:01:03
tags:
---

### 閱讀 SLERP 文獻

Detail：
[Paper Link](https://dl.acm.org/doi/abs/10.1145/325334.325242)

### 進行 MMLU 評分

![](img1.png)
嘗試了以上五個種類，但運行時間超過兩個多小時還沒有結果

_Update_

|                    | accuracy | time      |
| ------------------ | -------- | --------- |
| anatomy            | 0.422    | 4570.370  |
| clinical_knowledge | 0.400    | 11009.895 |
| college_biology    | 0.472    | 5888.956  |
| college_medicine   | 0.312    | 7652.638  |
| medical_genetics   | 0.530    | 2989.634  |

### 查閱其他的 merge methods

[evolutionary model merge](https://github.com/sakanaai/evolutionary-model-merge)
[paper link](https://paperswithcode.com/paper/evolutionary-optimization-of-model-merging)

由於原先的 model merge 需要自己選擇模型與演算法，因此就會添加許多不必要的人為因素。此種方法自動尋找不同的開源模型進行組合，以避免上面提到的問題。

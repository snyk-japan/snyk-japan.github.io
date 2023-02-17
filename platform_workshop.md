---
layout: page
title:  "Snyk ハンズオンワークショップ"
parmalink: /hands-on-workshop/
categories: Snyk Japan
---

# Snyk ハンズオンワークショップ

## アジェンダ：

### Snyk紹介＆製品概要
* 所要時間：10分

### [Snyk Code & OSS](https://github.com/snyk-japan/snyk-sca-sast-workshop)
* 所要時間：40分 (まとめ10分ふくむ）

### [Snyk Container](https://github.com/snyk-japan/snyk-container-workshop)
* 所要時間：30分 (まとめ5分ふくむ）

### [Snyk IaC](https://github.com/snyk-japan/snyk-iac-workshop)
* 所要時間：30分 (まとめ5分ふくむ）

### Q&A
* 所要時間：10分


## 補足情報

### 複数 Organization に所属している場合

* Snyk では各ユーザーは 1 つ以上の Organization に所属しています
* 複数の Organization に所属している場合は、ご自身でサインアップした Free Plan に紐づく Organization を、このワークショップではご利用ください
* Snyk Web UI の左上の `Group` から `Ungrouped` を選択し、その下の `Organization` からご自身の Organization 名を選択してください (申し込み状況により `Group` と `Organization` の選択肢は異なります)
* 複数の Organization に所属している場合、デフォルトで利用する Organization を指定することができます。Snyk Web UI の左下のドロップダウンメニューより、Account settings を選択した上で、`Preferred Organization` に適切なものを指定してから、`Update Preferred Org` ボタンを選択してください。
* CLI 実行時にはスキャンを実行する際の Organization をコマンドラインオプションで指定することができます。(実行例 `snyk test --org=xxx000000-0000-0000-xxxx-0000xxxx0000`)
* `--org=` に続く引数には Organization ID を指定します。Organization ID　は Web UI 画面左上の Organization → Settings → General より取得できます。

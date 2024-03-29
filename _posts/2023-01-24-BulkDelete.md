---
layout: post
title:  "ProjectのBulk Delete"
date:   2023-01-24 09:00:00 +0900
categories: Snyk Japan, Bulk delete
---

# SnykのProjectsをまとめて削除する方法（Bulk Delete)

Snykの有償版では以下のような構成でGroup - Organization - Projectが成り立っています。

- **Group**: Groupには多くのOrganizationを持つことができます。多くのケースでは企業毎にGroupを作成し、その下にプロジェクト単位やチーム単位でOrganizationを作成して管理します。
- **Ornaization**: Organizationは、複数のProjectを管理するユニットで、それらのProjectにアクセスできるチームメンバーの管理も行えます。Ornanization毎にWeb UIやCLIの設定を変更できますので、Organizationを切り替えて使用することも可能です。
- **Project**: Projectは、特定ターゲットに対しての解析の構成情報や解析結果を管理するユニットです。

<img src="https://3099555661-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F-MdwVZ6HOZriajCf5nXH%2Fuploads%2Fgit-blob-fdccc3f1f2fc4e8b4bfefd8e22c90346e8ee277c%2FGroup%20Onboarding%20Session%20v2.0.png?alt=media&token=8dd35e7f-a91f-44cd-a632-cd4c5602f636">

もう解析を行わなくなったProjectや、不要なProjectを一度に削除するにはBulk Deleteが便利です。

Projectの含まれているOrganizationの左側のコントロールペーンから `Setting` → `Usage` をクリックします。

<img width="503" alt="image" src="https://user-images.githubusercontent.com/45160975/214208431-68ecd440-abc6-4762-bc04-f5ff4d64b78f.png">

下の方にスクロールすると `Projects` というセクションがあります。

<img width="1239" alt="image" src="https://user-images.githubusercontent.com/45160975/214208784-bcc62691-0e6c-4d85-bd4a-0c0d0f8e64de.png">

ここで `Search projects` で対象となるProjectのフィルタリングを行います。
今回は例として、 `itmstm/snyk-juice-shop` という文字列を `Search projects` に入力して、対象となる `juice-shop` のProjectをリストアップします。

<img width="1239" alt="image" src="https://user-images.githubusercontent.com/45160975/214209237-7e3ef44c-8ad2-427d-b090-f43b11903042.png">

削除したいProjectにチェックを入れて、 `Bulk actions` から `Delete` をクリックします。

<img width="1239" alt="image" src="https://user-images.githubusercontent.com/45160975/214209424-0fdf84c1-d9d7-47d0-a53b-393b68e156ad.png">

ブラウザから確認のボックスが開きますので、`OK` をクリックしてください。

<img width="441" alt="image" src="https://user-images.githubusercontent.com/45160975/214209484-c7af9408-eb73-4456-8b16-937b6a475465.png">

これでBulk Deleteができました。

一度に多くのProjectをUIから削除したい場合にどに活用ください。

また、上記の方法以外にもAPIでプログラマティックにProjectを削除することも可能です。
その場合は、[こちらのAPI](https://snyk.docs.apiary.io/#reference/projects/individual-project/delete-a-project)をご利用ください。

---
title: "BRIDGE教育AI"
layout: single
permalink: /
toc: true
toc_label: "目次"
toc_sticky: true
excerpt: "教育向けAIモデルの構築と、人と協調するエージェントAI教育支援エコシステムの開発"
---

## プロジェクト概要

**BRIDGE教育AI**は、内閣府[「研究開発とSociety 5.0との橋渡しプログラム（BRIDGE）」](https://www8.cao.go.jp/cstp/bridge/saitaku_r8.html)の採択施策である、
文部科学省の**「教育向けAIモデルの構築と人と協調するエージェントAI教育支援エコシステムの開発」**に関する取り組みです。

国立情報学研究所（NII）を主体として、京都大学、大阪教育大学が連携し、教育関連企業や実証校とともに、
日本の教育制度に適合した透明性・信頼性の高い**教育特化型AIモデル**と、それを中核とする**3種のエージェントAI**
（学習者支援・教員支援・教育改善）からなる教育支援エコシステムを開発します。

詳しくは[研究概要のページ]({{ "/research/" | relative_url }})をご覧ください。

## 最新ニュース

<ul class="news-list">
{% for post in site.posts limit:3 %}
  <li>
    <span class="news-date">{{ post.date | date: "%Y.%m.%d" }}</span>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>

[ニュース一覧を見る →]({{ "/news/" | relative_url }})

## 実施機関

本プロジェクトは、以下の研究機関が中核となって推進しています。

- [**国立情報学研究所（NII）**]({{ "/organizations/nii/" | relative_url }}) — 教育特化型AIモデル・汎用エージェント基盤の開発、データ収集（プロジェクト主体）
- [**京都大学**]({{ "/organizations/kyoto/" | relative_url }}) — ラーニングアナリティクス、教育改善メタエージェントの研究開発
- [**大阪教育大学**]({{ "/organizations/osaka/" | relative_url }}) — 学習者支援・教員支援エージェントの研究開発・実証研究

実施体制の全体像は[実施体制のページ]({{ "/organizations/" | relative_url }})をご覧ください。

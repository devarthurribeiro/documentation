---
title: Datadog クリップボード
kind: documentation
disable_toc: true
description: インシデントの作成と管理
---
**Datadog クリップボードは、現在、公開ベータ版です**

# 概要

Datadog クリップボードは、さまざまなコンテキストを収集して共有するためのクロスプラットフォーム型ツールです。各ユーザーが個別に使用でき、コピーしたすべてのグラフを保存したリンクと一緒に保存できます。また、シグナルは分類して、ダッシュボード、ノートブック、インシデントにエクスポートできます。

{{< img src="monitors/incidents/clipboard-full.png" alt="クリップボード">}}

## クロスページ検索

クリップボードは Datadog のすべてのページに対応しており、各ユーザーがコピーしたすべてのグラフの記録がクリップボードに保持されます。ただし、クエリテキスト、イベント JSON、その他のテキストベースのコンテンツは自動的にクリップボードにコピーされません。

## クリップボードを開く

クリップボードを開くには、いずれかのグラフをコピーして、トースト内で “Open Clipboard” をクリックします。

{{< img src="monitors/incidents/open-clipboard.png" alt="クリップボードでグラフを開く"  style="width:80%;">}}

または、最小化されたクリップボード上で “`Cmd/Ctrl + Shift + X` to open” をクリックします。

クリップボードの開閉には、`Cmd/Ctrl + Shift + X` キーも使用できます。クリップボードを最小化するには、最小化アイコンをクリックします。最小化されたクリップボードは、Datadog の全ページにそのまま残ります。

## クリップの追加

グラフを追加するには、`Cmd/Ctrl + C` キーを押してコピーするか、エクスポートメニューで “Copy” をクリックします。クリップボードが開いた際に、コピーしたグラフが自動的に追加されます。

URL を追加するには、クリップボードを開き、“Add Current URL” をクリクします。

{{< img src="monitors/incidents/add-dashboard.png" alt="クリップボードにダッシュボードを追加"  style="width:80%;">}}

## クリップの管理

クリップボードの各アイテムは、開く、閉じる、削除することができます。シグナルの上にカーソルを置くと、これらの操作を実行できます。アイテムを開くと、元のシグナルのリンクへと移動します。アイテムの下に表示されるタイトルをクリックすると、グラフのソース (クリップ元のダッシュボードなど) が開きます。

{{< img src="monitors/incidents/managing-clips.png" alt="クリップを管理"  style="width:80%;">}}

クリップボードには、最大 20 個のグラフを保存できます。削除する場合は、1 つずつ削除するか、左下の “Clear Clipboard” をクリックします。21 個以上のグラフが追加された場合、一番古いグラフ (一番右側) が自動的に削除されます。

## エクスポート

クリップボードのアイテムは、ダッシュボード、ノートブック、インシデントにエクスポートできます。複数個を選択する場合は、`Shift` キーを押しながらクリックします。エクスポートメニューで、新しいエクスポート先を選択するか、既存のダッシュボード、ノートブック、インシデントから検索します。

{{< img src="monitors/incidents/exporting.png" alt="クリップボードからエクスポート"  style="width:80%;">}}

URL はダッシュボードにエクスポートできません。[サポート対象のグラフ][1]のみ、ノートブックにエクスポートできます。

[1]: https://docs.datadoghq.com/ja/notebooks/#visualization
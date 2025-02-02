# コードレビュー開発者ガイド

## はじめに {#intro}

コードレビューとは、コードの作成者以外の人がコードを調べるプロセスです。

Google ではコードとプロダクトの品質を維持するためにコードレビューを実施しています。

このドキュメントは Google のコードレビューのプロセスとポリシーに関する正規の解説です。

このページでは私達のコードレビュープロセスを概観します。このガイドはさらに二つのドキュメントに分けられます。

- **[コードレビューの仕方](reviewer/)**: コードレビュアーのための詳細なガイド
- **[CL 作成者のガイド](developer/)**: CL をレビューしてもらう開発者のための詳細なガイド

## コードレビュアーはどんな観点でレビューすべきか？ {#look_for}

コードレビューは次の観点で見るべきです。

- **設計**: コードはうまく設計され、そのシステムにとって適切か？
- **機能性**: コードは作成者の意図通りに動作するか？ユーザーにとってコードの挙動は適切か？
- **複雑さ**: コードはもっとシンプルにできるか？コードを作成した開発者があとになってもう一度そのコードに触れたとき、理解しやすく使いやすいか？
- **テスト**: そのコードには、正確で、うまく設計され、自動化されたテストがあるか？
- **命名**: 変数名、クラス名、メソッド名などに明解な名前を選んだか？
- **コメント**: コメントは明解で有益か？
- **スタイル**: コードは[スタイルガイド](http://google.github.io/styleguide/)に準拠しているか？
- **ドキュメント**: 関連するドキュメントも更新してあるか？

詳細は**[コードレビューの仕方](reviewer/)**を確認してください。

### 最高のレビュアーを選ぶ {#best_reviewers}

一般的に、レビュアーを探すとなれば合理的な時間内でレビューに反応してくれる**最高の**レビュアーを見つけたいと思うでしょう。

最高のレビュアーとは、あなたが書いたコードにすみずみまで正確なレビューをしてくれる人です。
多くの場合、最高のレビュアーはコードの所有者です。OWNERS ファイルに記載されていることもありますが、そうでないこともあります。
ときには CL の変更箇所をいくつかに分けて、それぞれ別の人にレビューをお願いするのが相応しい場合もあります。

理想的なレビュアーを見つけたとしても彼らが忙しくてレビューできないこともあります。そういうときでも少なくとも彼らを変更の CC に割り当てるべきです。

### 対面でのレビュー {#in_person}

適切なコードレビューをする資格のある人とペアプログラミングで書いたコードは、レビュー済みとみなせます。

また、対面でコードレビューを受けることもできます。レビュアーが質問をし、コードの作成者が質問に答えるという形です。

## 参考 {#seealso}

- [コードレビューの仕方](reviewer/): コードレビュアーのための詳細なガイド
- [CL 作成者のガイド](developer/): CL がレビューを受けている開発者のための詳細なガイド

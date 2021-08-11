# 自己紹介
## 概略
- 2014年3月：東京工業大学大学院 材料工学専攻修了。火力発電タービンのような、高温で使われる合金材料の研究をしていました。
- 〜2019年3月：金属材料系の会社で製造プロセス設計エンジニアとして従事。在社中に競技プログラミングにハマり、ITエンジニアへの転身を考えるようになりました。
- 2019年7月〜：シェルフィー株式会社にてアプリケーションエンジニアとして従事。チケット駆動開発下で以下の工程を主に担当しました
  - 詳細設計
  - フロント〜バックエンドのコーディング
  - テスト
  - コードレビュー

## 好きな○○
言語：Python, TypeScript  
エディタ：VSCode  
技術書：SQLアンチパターン  
技術者：t_wadaさん  
アルゴリズム : 動的計画法  

## リンク
GitHub : https://github.com/tktk0430  
Qiita : https://qiita.com/tktk0430  
競技プログラミング解説ブログ : https://okina-ichiyaduke.hatenablog.com/  
社内インタビュー記事 : https://www.wantedly.com/companies/shelfy/post_articles/309061

<br>

# Want
- ユーザーの気持ちを考えること、ユーザーについて学ぶことが楽しいと思える業界領域で仕事がしたい
- 長く手入れするプロダクトに関わりたい。長く関わることを意識した仕組みづくり（自動テスト、適切なリファクタリング期間など）の重要性を理解し、実現できているチームで働きたい
- 常にストレッチされたミッションに関わることができ、エンジニアとして停滞を感じることのない環境で働きたい
- 心理的安全性の概念を理解しているメンバーと、役職問わずディスカッションができる環境で働きたい
- 法令遵守意識の高い会社で働きたい

<br>

# 技術の経験
言語：Python, TypeScript, JavaScript, Ruby(独学)  
フレームワーク：Django REST Framework, React, Ruby on Rails(独学)  
DB : PostgreSQL, MySQL  
AWS : Lambda, EC2, RDS, SNS, EKS（インフラ構築は未経験、kubectl等の操作が可能）  
他 : Docker, ElasticSearch  

<br>

# 職歴
## ①-1. 新規プロジェクトの立ち上げ
立ち上げ期 : 2020/7 〜 2021/2  
運用・保守期 : 2021/2 〜 現在

**チーム**  
開発チーム人数: 4 人

**開発環境**  
Python, Django, TypeScript, React, PostgreSQL, ElasticSearch, Amazon EKS

**詳細**  
今後のプロダクト増加を見据えての、アプリ間のハブとなるアプリの設計の立ち上げメンバーとして関わりました。

【フロントエンド】
- 今後の開発を高速化するための基礎コンポーネント設計に従事。TypeScriptがもたらすDI向上を最大限享受できるようにつとめました。
  - [その時の状況について語った社内インタビュー記事](https://www.wantedly.com/companies/shelfy/post_articles/309061)
- React-hook-formの導入。これまでのプロジェクトで問題となっていた「不適切なフォーム管理によるパフォーマンスの低下」を抑制することを目的として導入を決めました。
  - 導入そのものより、ベテランエンジニアの了承をとるまでのプロセスが大変でした。「フォームの値をステート管理しないことによるパフォーマンス向上」「思い思いに実装されていたバリデーションロジックが一本化されることによる見通しの良さアップ」など、メリットやデメリットを説明して導入許可をもらいました
- ライブラリを使うために必要なカスタムフックなどは社内wikiにてドキュメント化し、誰でもすぐに使えるように心がけました。

【バックエンド】
- 「フレームワークの力を使い切って楽に開発する」を個人的なモットーとして、Djangoライクな書き方を心がけました。ファイル保存ロジックやエラーハンドリングなど、開発者が思い思いに実装していた部分を同じようなコードでかけるように共通化しました。
- ORMにおけるクエリチューニングの大切さを社内に浸透させました。リリース直前になって、max10000クエリ走っていたロジックを9クエリで済むように書き直すなどしました。
- 特に難しかった実装は「権限」です。「ユーザーごとに付与される権限」、「ユーザーのリソース状態によって異なる権限」など、さまざまな権限が絡み合う中で、バグなく実装するのが困難でした。
  - 仕様的にも複雑な部分であったため、カスタマーサイドが内容を理解できるよう、ドキュメントを残すなどの周知も徹底しました。
- 手動テストしかなかった会社にテストコード文化を導入しました。ベテランエンジニアと話しながら「どの粒度でテストコードを書くか？」「カバレッジはどのくらいを目指すか」などを決めました。また、github actionsを用いて、テストコードの自動化ができるようにしました。

【その他】
- 上記の功績が認められて、チーム内MVPを2度いただきました。

---

## ①-2. 既存プロジェクトでの機能実装
2019/7 〜 2020/6

**チーム**  
開発チーム人数: 10人超

**開発環境**  
Python, Django, JavaScript, React, PostgreSQL, Amazon ECS

**詳細**  
未経験エンジニアとして、開発のイロハを学びながら業務に取り組みました。

- Pythonは入社前からかけたものの、Reactは苦戦の連続でした。Reduxを理解できたときはとても嬉しかったです。
- 1ヶ月ほど顧客対応も担当しました。「電話の話し方が上手・トンマナがよい」と社内で謎に評判でした。
- 採用活動にも関わりました。業務の合間を縫って、一ヶ月で50通弱スカウトメールを送りました。プロフィールを見ながら「この人はこういうところを見てもらいたいハズ」という仮説のもと文章を練り上げる工程は中々面白かったです。採用面接にもたびたび同席しました。
- 「社内に眠っている知見を掘り起こしたい！」という野望のもと、社内勉強会（ナレッジシェア会）を主催しました。新人からベテランまでみんな登壇するように根回ししたり、勉強会中の司会進行などもしました。
  - 自分が話したトピックは「React.memoを用いたフロントのパフォーマンスチューニング」「VSCodeのデバッグ色々」「N+1問題の解消について」です

---

## ② 副業 [人事AIアシスタント researcHR](https://app.researchr.work/)の開発
副業として業務委託のポジションで参加しました。リモートワーク下で、月平均して30hrほどコミットしていました。  
2020/5 〜 2021/7

**職種**  
アプリケーションエンジニア

**チーム**  
開発チーム人数: 6 人

**開発環境**  
Django, Slack App, MySQL, AWS

**詳細**
- Slackアプリへの機能実装
- 管理画面の実装
- AWS Lambdaと連携しての、Slackチャンネルへのエラーログ収集
- 開発環境のdocker-compose化
- 社内勉強会でのオンライン登壇（テストコードの書き方について）

---

## ③ キャリアチェンジ前（日立金属）
2014/4 〜 2019/3

業種：鉄鋼・金属  
雇用形態：正社員

入社から一貫して航空機部品の開発に携わってきました。GE社やRollsRoyce社といった海外エンジンメーカーからの開発依頼を受け、その製造認定をとるためのプロジェクトに従事しました。

第一発明者として特許の出願などもおこないました。  
熱間鍛造材の製造方法 : http://www.conceptsengine.com/patent/application/2018089695  

<br>

# 資格
AWS Solution Architect Associate 2020年03月取得  
TOEIC 810 2018年12月取得

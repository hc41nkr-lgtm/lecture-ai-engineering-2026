# 第6回 解答

## 演習

<!-- [tool call] の行は、表示された行をそのまま貼り付けてください。終わらなかった STEP は、空欄のままでかまいません。 -->

- STEP 1 のツールの名前：search_materials
- STEP 2 の [tool call]：glossary_search_glossary({'query': '3レベル'})
- STEP 3 の [tool call]：fetch_fetch({'url': 'https://example.com'})
- STEP 4 の [tool call]：aws_aws___search_documentation({'search_phrase': 'Amazon S3 バージョニング 概要', 'topics': ['general']})
- 気づき・疑問：MCPサーバーを追加することで、AIが利用できるツールを増やせることが分かった。ローカルのツールだけでなく、WebやAWSの外部サービスにも接続できた。

## 宿題
- 取り組んだレベル：基礎
- やったこと：app/mcp_server.py に get_lecture_summary をMCPツールとして登録した。
- 結果：glossary_get_lecture_summary がツール一覧に表示された。第2回の講義内容を取得でき、pytestで21件成功した。
- 気づき・疑問：既存のPython関数をMCPツールとして公開することで、AIが必要に応じて呼び出せることが分かった。

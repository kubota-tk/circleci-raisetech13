# circleci-raisetech13
- CircleCIで以下のworkflowを実行するサンプルリポジトリ

## workflowの内容
1. リポジトリにコードをpush
2. CircleCIがリポジトリにpushされたことをイベントトリガーとしてworkflowを実行
3. 最初のjobとしてCloudformationを実行
4. ２番目のjobとしてAnsibleを実行（Cloudformationをトリガー）
5. ３番目のjobとしてServerspecを実行（Ansibleをトリガー）

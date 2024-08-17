# circleci-live-demo15-20240817
- CircleCIで以下のworkflowを実行するサンプルリポジトリです
## workflow
1. リポジトリにコードをpush
2. CircleCIがリポジトリにpushされたことをイベントトリガーとしてworkflowを実行
3. 最初のjobとしてCloudformationを実行
4. 2番目のjobとしてAnsibleを実行(ただしCloudformationのjobをイベントトリガーとする)
5. 3番目のjobとしてServerspecを実行(ただしAnsibleのjobをイベントトリガーとする)

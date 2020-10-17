# メモ書き
## tfenvでTerraformインストール
```
$ sudo yum update

$ sudo yum -y install git

$ git clone https://github.com/tfutils/tfenv.git ~/.tfenv

$ sudo ln -s ~/.tfenv/bin/* /usr/local/bin

$ tfenv list-remote     #インストール可能なバージョン表示

$ tfenv install 0.13.4

$ tfenv use 0.13.4

$ terraform --version

$ tfenv install 0.12.29  # 別バージョンを入れて切り替え可能

$ tfenv list

$ tfenv use 0.12.29

$ terraform --version
```
## 基本的な操作コマンド
```
$ terraform fmt      # 整形する

$ terraform validate # 構文チェック

$ terraform plan     # コードとAWSリソース現状との差分確認

$ terraform apply --parallelism=100  # AWS環境に反映(並列実⾏オプションつき)
```

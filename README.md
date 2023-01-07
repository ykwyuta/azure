# azure

https://docs.microsoft.com/ja-jp/azure/templates/

az cliを使えるようにする

```bash
curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash
```

最新バージョンの Bicep がインストールされていることを確認する

```bash
az bicep install && az bicep upgrade
```

Azureにログインする

```bash
az login --use-device-code
```

既定のサブスクリプションを設定する。環境変数の`AZURE_POC_SUBSCRIPTION`にサブスクリプション名を設定済み。

```bash
az account set --subscription $AZURE_POC_SUBSCRIPTION
```
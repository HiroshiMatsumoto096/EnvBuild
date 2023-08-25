# Python環境回り

# pyenv@windows

https://github.com/pyenv-win/pyenv-win

`Quick start`@`pyenv`に沿って進める

## 手順
Powershell上で以下のコマンド入力し`pyenv-win`をインストール

```
Invoke-WebRequest -UseBasicParsing -Uri "https://raw.githubusercontent.com/pyenv-win/pyenv-win/master/pyenv-win/install-pyenv-win.ps1" -OutFile "./install-pyenv-win.ps1"; &"./install-pyenv-win.ps1"
```

UnAuthorized Access で怒られるので

https://github.com/pyenv-win/pyenv-win/issues/332#issuecomment-1051177852

以下のコマンドを入力し、実行ポリシーを変更し、  
(Restricted --> RemoteSgined)  
`pyenv.ps1`ファイルのセキュリティを解除する

`Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser`

`Unblock-File (Join-Path $env:PYENV 'bin/pyenv.ps1')`

https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.utility/unblock-file?view=powershell-7.3

```
The Unblock-File cmdlet lets you open files that were downloaded from the internet. It unblocks PowerShell script files that were downloaded from the internet so you can run them, even when the PowerShell execution policy is RemoteSigned.
```

あとは`pyenv --version`をPowerShell上に入力しversion情報が表示されればOK

# poetry

To Be Filled
//Windows PowerShell

wsl --install -d Ubuntu
wsl --update
wsl --list -v

//PS C:\> wsl --list -v
//  NAME            STATE           VERSION
//* Ubuntu-20.04    Stopped         2
//  Ubuntu          Running         2

//WSLgを使いたいディストリビューションのVERSIONが「2」となっていればOK
//もしなっていない場合は、wsl --set-version Ubuntu 2を実行します。
//「Ubuntu」の部分は、利用したいディストリビューション名に置き換えてください。
//また、変更の適用にはWSLの再起動が必要なため、管理者権限のコマンドプロンプトかPowerShellからwsl --shutdownを実行します。

//Ubuntu Console
sudo apt update
sudo apt upgrade
sudo apt install x11-apps -y
sudo apt install gedit -y
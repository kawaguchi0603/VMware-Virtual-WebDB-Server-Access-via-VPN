# VMware-Virtual-WebDB-Server-Access-via-VPN

## 1. プロジェクト概要
本プロジェクトは、VMware上のLinux サーバー構築を行っております。
VMware上のサーバーをWebサーバー兼DBサーバーとして運用出来るよう構築し、遠隔でも操作可能にする為VPN接続を有効化しSSH接続にて操作可能にしております。

## 2. システム構成図

* **WebDB Server:** Ubuntu in VMware, Apache2, MySQL,Tailscale
* **Local PC:**Windows11,Tailscale

## 3. 実装した機能
- **VPN接続:** ホスト,クライアント側にTailscaleをインストールしWebconsoleよりユーザー追加し、Jsonエディターを直接編集し接続確認。
- **　　　:** 

## 4. 苦労した点と解決策
- **ssh接続時のエラー対応:** Tailscale側でACLの設定が出来ていないエラーに対し、Consoleより直接Jsonエディターを編集し解決した。
- **　　:** 

## 5. 動作確認エビデンス

## 6. 
- 
- 
- 
- 
## 7. 動作確認エビデンス


## 使用技術
- VM:VMware
- OS: Ubuntu
- 
- 
- 

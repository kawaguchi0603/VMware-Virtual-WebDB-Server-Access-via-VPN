# VMware-Virtual-WebDB-Server-Access-via-VPN

## 1. プロジェクト概要
本プロジェクトは、VMware上のLinux サーバー構築を行っております。
VMware上のサーバーをWebサーバー兼DBサーバーとして運用出来るよう構築し、遠隔でも操作可能にする為VPN接続を有効化しSSH接続にて操作可能にしております。

## 2. システム構成図

* **WebDB Server:** Ubuntu in VMware, Apache2, MySQL,Tailscale
* **Local PC:** Windows11,Tailscale

## 3. 実装した機能
- **VPN接続:** ホスト,クライアント側にTailscaleをインストールしWebconsoleより端末追加。Jsonエディターを直接編集し接続確認。
- **Webページテスト:** LAMP環境を構成し、SQLとPHPの疎通、及び設定反映テストを行い正常動作確認。
- **WebDBサーバー実装:** SQLへテーブルを作成し架空ファイルを格納。PHPからSQLを参照し文字入力検索機能の実装確認。

## 4. 苦労した点と解決策
- **ssh接続時のエラー対応:** Tailscale側でACLの設定が出来ていないエラーに対し、Consoleより直接Jsonエディターを編集し解決した。

## 5. Webページテスト動作確認エビデンス
<img width="453" height="121" alt="スクリーンショット 2026-06-02 093636" src="https://github.com/user-attachments/assets/7f8843c4-4995-4f99-b344-192a3aa7e774" />

## 6. 動作確認エビデンス
<img width="1492" height="585" alt="image" src="https://github.com/user-attachments/assets/0f2b7e2b-560d-4cb5-9902-7265506fe283" />
<img width="1467" height="480" alt="image" src="https://github.com/user-attachments/assets/715ae302-738d-483b-9b4d-3901705da109" />

## 使用技術
- VM: VMware
- OS: Ubuntu
- VPN: Tailscale
- DB: MySQL
- Security: mysql_secure_installation
- APP: PHP

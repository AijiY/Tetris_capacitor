# Tetris

## 作成背景（Background）
　HTML、CSS、Javascriptを使用して作成したテトリスゲームをスマートフォンで気軽に遊びたいと考えて、Capacitorによるネイティブアプリへと移行しました。

## 開発環境（Development Environment）
### 技術（Technologies）
![badge](https://img.shields.io/badge/-HTML5-333.svg?logo=html5&style=flat)
![badge](https://img.shields.io/badge/-CSS3-1572B6.svg?logo=css3&style=flat)
![badge](https://img.shields.io/badge/Javascript-276DC3.svg?logo=javascript&style=flat)

### ツール（Tools）
![badge](https://img.shields.io/badge/Visual%20Studio%20Code-1.95.0-007ACC.svg?logo=visual-studio-code&style=flat)
![badge](https://img.shields.io/badge/Capacitor-6.1.2-119EFF.svg?logo=capacitor&style=flat)
![badge](https://img.shields.io/badge/Microsoft%20Clipchamp-007ACC.svg?logo=visual-studio-code&style=flat)

## 機能（Function）

　以下はゲーム画面における操作についての説明です。

- ↶、↷ボタン：テトリミノを左右に回転します。<br>
  ![rotate ‐ Clipchampで作成](https://github.com/user-attachments/assets/87af9738-0edd-45a1-a11e-d66c0d14ee43)

- ←、→ボタン：テトリミノを左右に移動します。<br>
  ![move ‐ Clipchampで作成](https://github.com/user-attachments/assets/f09e3e99-1ae2-4674-a7a5-426bc9e516b0)

- ↓ボタン：テトリミノを下まで落下させます。<br>
  ![movedown ‐ Clipchampで作成](https://github.com/user-attachments/assets/8b5e7f2a-dc5b-4eeb-b8a9-d5ee22976b60)


### ゲーム終了条件
- ゲームオーバー条件：次のテトリミノを配置できなくなったらゲームオーバーです。<br>
  ![gameover ‐ Clipchampで作成](https://github.com/user-attachments/assets/9214baf8-8f66-4220-8e3f-8cb70433d020)

- クリア条件：Score（ブロック行を消去した数）が1000に到達するとゲームクリアです。

## 工夫した点 (Points to Note)
　テトリミノ操作ボタンを体感的に分かりやすいように配置しました。

## 今後の課題（Future Improvements）
- **非同期処理の改善** ：まれにブロックが適切な位置まで落下しない事態が発生するのを改善
- **タッチ操作の実装** ：ボタンによるテトリミノ操作よりも分かりやすい体感的な操作の導入
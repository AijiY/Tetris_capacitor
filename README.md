# Tetris (Capacitor)

このプロジェクトは、Capacitorを使用して開発されたモバイル用のテトリスゲームです。Capacitorを使用することで、WebアプリをiOSやAndroidでネイティブに実行できます。

## 目次
- [Tetris (Capacitor)](#tetris-capacitor)
  - [目次](#目次)
  - [プロジェクト概要](#プロジェクト概要)
  - [インストール](#インストール)
  - [アプリのビルド](#アプリのビルド)
  - [アプリの実行](#アプリの実行)
  - [ホーム画面](#ホーム画面)
  - [ゲーム画面（ゲーム開始前）](#ゲーム画面ゲーム開始前)
  - [ゲーム画面（ゲーム開始後）](#ゲーム画面ゲーム開始後)
    - [ボタン操作](#ボタン操作)
    - [ゲーム終了条件](#ゲーム終了条件)

## プロジェクト概要

このプロジェクトは、クラシックなテトリスゲームをCapacitorを使って開発したものです。ゲームロジックやUIにはHTML、CSS、JavaScriptを使用しており、Capacitorを利用してデバイスのハードウェア機能を使用し、ネイティブアプリとして動作します。

## インストール

1. **リポジトリをクローン**
   
   ```bash
   git clone https://github.com/AijiY/Tetris_capacitor.git
   cd Tetris_capacitor
   ```

2. **依存パッケージをインストール**
   Node.jsをインストールしていない場合は、まずインストールしてください。その後、以下を実行します。

   ```bash
   npm install
   ```

3. **Capacitorプラットフォームの追加**
   AndroidやiOSでアプリを実行するには、それぞれのプラットフォームを追加します。

   ```bash
   npx cap add android
   npx cap add ios
   ```

4. **Webアセットをビルド**
   Webアセットをビルドするために、以下を実行します。

   ```bash
   npm run build
   npx cap copy
   ```

## アプリのビルド
   Android StudioやXcodeを使用してアプリをビルドします。

   Android
   - Android Studioを開きます。
   - プロジェクトをAndroid Studioで開き、ビルドを実行します。
   ```bash
   npx cap open android
   ```
   iOS
   - Xcodeを開きます。
   - iOSプラットフォーム用にビルドします。
   ```bash
   npx cap open ios
   ```

## アプリの実行
   Android
   - Android Studioでプロジェクトを開いた後、デバイス（エミュレーターまたは実機）でアプリを実行します。

   iOS
   - Xcodeでプロジェクトを開いた後、シミュレーターまたは実機でアプリを実行します。

## ホーム画面

アプリを起動すると、3つの難易度のボタンが配置されており、どれか1つを押すとその難易度のゲーム画面に遷移します。

## ゲーム画面（ゲーム開始前）
- Exitボタン：ホーム画面に戻ります
- Sartボタン：ゲームを開始します。

## ゲーム画面（ゲーム開始後）

### ボタン操作
- Resetボタン：ゲームを初期化します。

- ↶、↷ボタン：テトリミノを左右に回転します。
  <br>
  ![rotate ‐ Clipchampで作成](https://github.com/user-attachments/assets/87af9738-0edd-45a1-a11e-d66c0d14ee43)

- ←、→ボタン：テトリミノを左右に移動します。
  <br>
  ![move ‐ Clipchampで作成](https://github.com/user-attachments/assets/f09e3e99-1ae2-4674-a7a5-426bc9e516b0)

- ↓ボタン：テトリミノを下まで落下させます。
  <br>
  ![movedown ‐ Clipchampで作成](https://github.com/user-attachments/assets/8b5e7f2a-dc5b-4eeb-b8a9-d5ee22976b60)


### ゲーム終了条件
- ゲームオーバー条件：次のテトリミノを配置できなくなったらゲームオーバーです。
  <br>
  ![gameover ‐ Clipchampで作成](https://github.com/user-attachments/assets/9214baf8-8f66-4220-8e3f-8cb70433d020)

- クリア条件：Score（ブロック行を消去した数）が1000に到達するとゲームクリアです。
# Tetris (Capacitor)

このプロジェクトは、Capacitorを使用して開発されたモバイル用のテトリスゲームです。Capacitorを使用することで、WebアプリをiOSやAndroidでネイティブに実行できます。

## 目次
- [Tetris (Capacitor)](#tetris-capacitor)
  - [目次](#目次)
  - [プロジェクト概要](#プロジェクト概要)
  - [インストール](#インストール)
  - [アプリのビルド](#アプリのビルド)
  - [アプリの実行](#アプリの実行)

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
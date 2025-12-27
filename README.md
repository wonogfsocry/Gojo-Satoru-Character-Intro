# 咒術迴戰：五條悟角色介紹 App (Gojo Satoru Character Intro)

這是一個使用 **SwiftUI** 開發的 iOS 應用程式，旨在介紹《咒術迴戰》中的人氣角色——五條悟。App 透過互動式的介面設計，讓使用者能夠在「最強咒術師」的不同時期（學生時期 vs. 導師時期）之間切換，查看相關的人物介紹與名場面。

此專案為 **海大 iOS App 程式設計** 課程的作業成果。

## 📱 App 畫面展示 (App Demo)

<p align="center">
  <img src="ebook_screen.gif" alt="App Demo" width="300" />
</p>

## 🔗 專案文章與教學

詳細的開發過程、心得與技術解說，請參考我的 Medium 文章：

👉 **[iOS應用程式開發入門-01-打造吸睛的 about 頁面](https://medium.com/%E6%B5%B7%E5%A4%A7-ios-app-%E7%A8%8B%E5%BC%8F%E8%A8%AD%E8%A8%88/ios%E6%87%89%E7%94%A8%E7%A8%8B%E5%BC%8F%E9%96%8B%E7%99%BC%E5%85%A5%E9%96%80-01-%E6%89%93%E9%80%A0%E5%90%B8%E7%9D%9B%E7%9A%84-about-%E9%A0%81%E9%9D%A2-61d11224b61f)**

## ✨ 功能特色 (Features)

* **互動式主頁面**：
    * 展示五條悟的基本資料（身高、生日、稱號）。
    * 使用 `ZStack` 與 `Overlay` 技巧堆疊精美的 UI 元素。
    * **術式切換按鈕**：點擊「術式反轉『赫』」或「術式順轉『蒼』」按鈕，可切換至不同的角色時期頁面。
* **多時期介紹 (NavigationView)**：
    * **學生時期**：介紹高專時代的五條悟，包含摯友夏油傑、家入硝子等角色。
    * **導師時期**：介紹擔任老師後的五條悟，包含學生虎杖悠仁、伏黑惠、釘崎野薔薇。
* **橫向捲動視圖 (Horizontal ScrollView)**：
    * 在人物介紹頁面中，使用 `ScrollView(.horizontal)` 展示相關聯的角色列表。
    * 點擊角色名稱可跳轉至萌娘百科 (Moegirl) 查看詳細資料。
* **影音與動畫整合**：
    * **名場面播放**：點擊劇照即可開啟 YouTube 觀看該時期的經典片段。
    * **自定義形狀**：使用 `Path` 繪製五角星圖案 (`StarShape`) 裝飾畫面。
    * **動畫效果**：包含返回按鈕的箭頭動畫 (`offset` 與 `animation`) 以及頁面切換的轉場效果。
* **自訂字體**：
    * 專案中整合了 `Cubic_11` 與 `NewTegomin-Regular` 特殊字體，提升視覺風格。

## 🛠️ 技術運用 (Tech Stack)

* **SwiftUI**: 宣告式 UI 框架
* **Images & Assets**: 使用 Asset Catalog 管理圖片與顏色
* **Custom Fonts**: 導入與應用外部字體文件 (.ttf)
* **Link & UIApplication**: 處理外部網頁跳轉與 URL 開啟
* **Geometry & Shapes**: 自定義圖形繪製

## 📂 檔案結構簡介

* `ContentView.swift`: 主要的視圖邏輯，包含主頁面與 `ExtractedView` (詳細介紹頁面)。
* `Assets.xcassets`: 存放角色圖片 (gojo, summer, homee, tiger 等) 與 App 圖示。
* `Fonts`: 包含專案使用的 `Cubic_11` 等字型檔。

---

## 👤 作者 (Author)

* **Name**: 楊浤立
* **Student ID**: 01157025
* **Created Date**: 2024/11/28

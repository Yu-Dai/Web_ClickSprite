# ClickSprite 網站部署指南

## 🚀 快速部署到 GitHub Pages

### 步驟 1：建立 GitHub 儲存庫
```bash
# 建立新儲存庫
git init
git add .
git commit -m "Initial commit: ClickSprite website"
git branch -M main
git remote add origin https://github.com/yourusername/clicksprite-website.git
git push -u origin main
```

### 步驟 2：啟用 GitHub Pages
1. 進入儲存庫設定頁面
2. 滾動到 "Pages" 部分
3. 選擇 "Deploy from a branch"
4. 選擇 "main" 分支
5. 選擇 "/ (root)" 資料夾
6. 點擊 "Save"

### 步驟 3：等待部署完成
- 部署通常需要 1-2 分鐘
- 完成後可在 `https://yourusername.github.io/clicksprite-website` 訪問

## 🔧 配置設定

### 1. 更新 Google AdSense
在 `index.html` 中替換以下內容：
```html
<!-- 替換為您的 AdSense 客戶端 ID -->
<script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-XXXXXXXXXXXXXXXX"
        crossorigin="anonymous"></script>

<!-- 替換為您的廣告位 ID -->
<ins class="adsbygoogle"
     style="display:block"
     data-ad-client="ca-pub-XXXXXXXXXXXXXXXX"
     data-ad-slot="1234567890"
     data-ad-format="auto"
     data-full-width-responsive="true"></ins>
```

### 2. 更新下載連結
在 `download-manager.js` 中更新：
```javascript
this.downloadUrl = 'https://github.com/yourusername/clicksprite/releases/latest/download/ClickSprite.exe';
this.fallbackUrl = 'https://github.com/yourusername/clicksprite/releases';
```

### 3. 自訂網域（可選）
1. 在儲存庫設定中設定自訂網域
2. 在 DNS 設定中添加 CNAME 記錄
3. 更新 `script.js` 中的追蹤設定

## 📊 功能特色

### ✅ 已實現功能
- **響應式設計**：適配各種螢幕尺寸
- **金鑰生成系統**：安全的金鑰生成和驗證
- **廣告整合**：Google AdSense 支援
- **下載管理**：自動下載和進度顯示
- **用戶統計**：本地數據追蹤
- **事件追蹤**：完整的用戶行為分析

### 🔒 安全機制
- **金鑰驗證**：格式檢查和重複使用防護
- **時間限制**：24小時金鑰有效期
- **本地儲存**：用戶數據本地加密儲存
- **廣告攔截檢測**：自動檢測並提示用戶

## 📈 收益優化建議

### 1. 廣告位置優化
- **頁面頂部**：高曝光率
- **內容中間**：高點擊率
- **頁面底部**：完整閱讀後點擊

### 2. 廣告類型建議
- **響應式廣告**：適配各種螢幕
- **展示廣告**：提高品牌知名度
- **影片廣告**：更高收益

### 3. 內容優化
- **關鍵字優化**：提高搜尋排名
- **內容更新**：保持新鮮度
- **用戶體驗**：降低跳出率

## 🛠️ 維護指南

### 定期維護任務
1. **檢查廣告狀態**：確保廣告正常顯示
2. **更新程式版本**：保持下載連結有效
3. **清理舊數據**：定期清理過期金鑰
4. **監控統計**：分析用戶行為和收益

### 故障排除
1. **廣告不顯示**：檢查 AdSense 設定
2. **下載失敗**：檢查 GitHub Releases
3. **金鑰無效**：檢查金鑰生成邏輯
4. **統計異常**：檢查本地儲存

## 📱 行動裝置優化

### 響應式設計
- 使用 CSS Grid 和 Flexbox
- 適配各種螢幕尺寸
- 觸控友好的按鈕設計

### 效能優化
- 圖片壓縮和懶載入
- CSS 和 JavaScript 最小化
- 快取策略優化

## 🔍 SEO 優化

### 基本 SEO
- 適當的 meta 標籤
- 語義化 HTML 結構
- 圖片 alt 屬性
- 內部連結結構

### 進階 SEO
- Google Search Console 設定
- 網站地圖提交
- 結構化數據標記
- 頁面載入速度優化

## 📊 分析工具整合

### Google Analytics
```html
<!-- 在 <head> 中添加 -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

### 其他分析工具
- Facebook Pixel
- 百度統計
- 其他第三方分析工具

## 🚨 注意事項

### 法律合規
- 遵守廣告法規
- 保護用戶隱私
- 明確服務條款

### 技術限制
- GitHub Pages 靜態網站限制
- 本地儲存容量限制
- 瀏覽器相容性

### 安全考量
- 定期更新依賴
- 監控異常活動
- 備份重要數據

## 📞 技術支援

如有問題，請檢查：
1. 瀏覽器控制台錯誤訊息
2. 網路連線狀態
3. 廣告攔截器設定
4. 本地儲存權限

## 📄 授權條款

本網站僅供學習和研究使用，商業使用請確保符合相關法律法規。

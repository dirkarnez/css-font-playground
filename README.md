css-font-playground
===================
Fonts
- `woff`
- `woff2`
- `otf`

### Reference
- [[設計] 使用 CSS 載入思源黑體(Noto Sans TC)的快速方式 - 免費顧問, 公司CMS, 網上商店, 支付功能等...](https://www.tan-studio.net/programskill/divcss/%E8%A8%AD%E8%A8%88-%E4%BD%BF%E7%94%A8-css-%E8%BC%89%E5%85%A5%E6%80%9D%E6%BA%90%E9%BB%91%E9%AB%94noto-sans-tc%E7%9A%84%E5%BF%AB%E9%80%9F%E6%96%B9%E5%BC%8F/)
  - ```css
      /*
      * Noto Sans TC (Chinese_traditional) http://www.google.com/fonts/earlyaccess
       */
      @font-face {
        font-family: 'Noto Sans TC';
        font-style: normal;
        font-weight: 100;
        src: url(//fonts.gstatic.com/ea/notosanstc/v1/NotoSansTC-Thin.woff2) format('woff2'),
             url(//fonts.gstatic.com/ea/notosanstc/v1/NotoSansTC-Thin.woff) format('woff'),
             url(//fonts.gstatic.com/ea/notosanstc/v1/NotoSansTC-Thin.otf) format('opentype');
        font-display: fallback;
      }
      @font-face {
        font-family: 'Noto Sans TC';
        font-style: normal;
        font-weight: 300;
        src: url(//fonts.gstatic.com/ea/notosanstc/v1/NotoSansTC-Light.woff2) format('woff2'),
             url(//fonts.gstatic.com/ea/notosanstc/v1/NotoSansTC-Light.woff) format('woff'),
             url(//fonts.gstatic.com/ea/notosanstc/v1/NotoSansTC-Light.otf) format('opentype');
        font-display: fallback;
      }
      @font-face {
         font-family: 'Noto Sans TC';
         font-style: normal;
         font-weight: 400;
         src: url(//fonts.gstatic.com/ea/notosanstc/v1/NotoSansTC-Regular.woff2) format('woff2'),
              url(//fonts.gstatic.com/ea/notosanstc/v1/NotoSansTC-Regular.woff) format('woff'),
              url(//fonts.gstatic.com/ea/notosanstc/v1/NotoSansTC-Regular.otf) format('opentype');
        font-display: fallback;
       }
      @font-face {
         font-family: 'Noto Sans TC';
         font-style: normal;
         font-weight: 500;
         src: url(//fonts.gstatic.com/ea/notosanstc/v1/NotoSansTC-Medium.woff2) format('woff2'),
              url(//fonts.gstatic.com/ea/notosanstc/v1/NotoSansTC-Medium.woff) format('woff'),
              url(//fonts.gstatic.com/ea/notosanstc/v1/NotoSansTC-Medium.otf) format('opentype');
        font-display: fallback;
       }
      @font-face {
        font-family: 'Noto Sans TC';
        font-style: normal;
        font-weight: 700;
        src: url(//fonts.gstatic.com/ea/notosanstc/v1/NotoSansTC-Bold.woff2) format('woff2'),
             url(//fonts.gstatic.com/ea/notosanstc/v1/NotoSansTC-Bold.woff) format('woff'),
             url(//fonts.gstatic.com/ea/notosanstc/v1/NotoSansTC-Bold.otf) format('opentype');
        font-display: fallback;
       }
      @font-face {
         font-family: 'Noto Sans TC';
         font-style: normal;
         font-weight: 900;
         src: url(//fonts.gstatic.com/ea/notosanstc/v1/NotoSansTC-Black.woff2) format('woff2'),
              url(//fonts.gstatic.com/ea/notosanstc/v1/NotoSansTC-Black.woff) format('woff'),
              url(//fonts.gstatic.com/ea/notosanstc/v1/NotoSansTC-Black.otf) format('opentype');
        font-display: fallback;
       }
     ```
      - `font-display` to avoid delayed display
   - ```css
      @import url(//fonts.googleapis.com/earlyaccess/notosanstc.css);
      body{
        /* 先套用 Noto Sans TC 這個 思源黑體 */
        font-family: 'Noto Sans TC', '微軟正黑體', sans-serif;
      }
     ```

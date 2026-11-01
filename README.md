# 07 - OKLCH CSS カラー サンドボックス

**ビルド日**: 2026-11-02
**カテゴリ**: practical
**slug**: oklch-css-color-sandbox

## 概要

OKLCH知覚均等色空間のインタラクティブエクスプローラー。L/C/Hスライダーでリアルタイムプレビューと各種変換値を表示。

## 機能

- L（明度0-1）・C（彩度0-0.4）・H（色相0-360°）スライダー
- OKLCH→sRGB変換（OKLab中間変換経由）
- ガモット外警告（sRGB外の場合）
- CSS `oklch()` 出力（クリックでコピー）
- HEX/RGB/HSL変換値表示
- 補色（H+180°）プレビュー
- 明度スケール（L:0.1→0.9）のカラーバー
- 3種のカラーハーモニー（補色・三色・四色）
- OKLCH vs HSL知覚均等性比較パネル
- 色相リング（Canvas描画）

## 技術仕様

- 単一HTMLファイル、Tailwind CDN使用
- OKLCH→OKLab→線形RGB→sRGB変換を純粋JS実装

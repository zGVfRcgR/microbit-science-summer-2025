# 「鼓動するスライム心臓 ～磁力とプログラムで生命を再現～」

## 構成図（機器配置イメージ）

```
[ 心臓型容器 ]
      ↓ （砂鉄スライム）
 [ 回転モーター ] ← 磁石を載せる（磁場生成）
      ↓
[ micro:bit ] ← モーター制御 + LED点灯制御
      ↑
[ 磁力センサー（HCSR04やQMC5883L）] ← 砂鉄の反応を検知・フィードバック
```

## 使用する主要部

|部品名|用途|
|-----|----|
|micro:bit（v2推奨）|制御・LED表示・センサー接続|
|モーター（小型DC or サーボ）| 磁石を回転させ、磁力を変化 |
|磁石（ネオジムなど）| 砂鉄スライムを動かす磁場生成用 |
| 砂鉄スライム | 心臓の“拍動”表現素材 |
| 心臓型容器（シリコン or PET）| 見た目の表現／作品の安全性確保 | 
| QMC5883L（磁力センサー） | 砂鉄の動きを検知し、動作をフィードバック制御 |
| LED | 拍動のタイミングで視覚効果を演出 |

## 機能の概要

- **自動拍動機構**：micro:bitからモーターを周期制御 → 磁石が回転 → 磁場変化で砂鉄スライムが拍動
- **磁力センサーによる反応制御**：砂鉄スライムの反応強度をセンサーが読み取り、拍動周期を調整（速く／ゆっくり）
- **LED表現**：拍動に合わせて光る → 視覚的に心臓の動きを再現（赤い光で効果UP）

## 審査基準との対応

| 観点 | 本作品での対応内容 | 
| ----| ------------------|
| 着想が新しいか | 砂鉄スライム × 生物の拍動の融合は独自性が高い | 
| 創意工夫が盛り込まれているか | 磁力による物理的制御 + センサーによるプログラム的フィードバックを融合 | 
| 研究努力が積まれているか | スライムの粘度・磁石の距離・磁場強度など、事前実験で動きの変化を観察・分析 | 
| 学習したことを発展させているか | 磁力・センサー・電子工作・生物のモデル化など、授業内容の応用が明確 | 



## 工夫ポイント・発展案
- 拍動の速度が手のひらの接近や光センサーで変化 → 生体反応を模倣
- 複数の拍動モード（安静・運動時など）をボタン操作で切り替え可能
- 生物模型として解説文を貼り、来場者に科学現象として説明

## 詳細

- [基本設計](基本設計.md)
- [心臓とは](心臓の仕組み.md)
- 実験
    - [テンプレート](実験/テンプレート.md)
    - [記録表](実験/記録表.md)

## 参照

- [募集要項](募集要項.md)
- [実施要項](実施要項.md)
- [R6年度結果](R6年度結果.md)
<script src="https://makecode.com/gh-pages-embed.js"></script><script>makeCodeRender("{{ site.makecode.home_url }}", "{{ site.github.owner_name }}/{{ site.github.repository_name }}");</script>

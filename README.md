# Raspberry Pi を用いた DIC システム開発プロジェクト

このリポジトリは [MultiDIC](https://github.com/SolavLab/MultiDIC) をフォークし、Raspberry Pi ベースの DIC システム開発用にカスタマイズしたものです。

---

## 📝 開発ブログ

### 2025年8月21日 - ハードウェア到着 🎉

本日、DICシステム構築に必要な主要ハードウェアが到着しました！

#### 購入機材リスト
1. **Raspberry Pi 4 Model B (8GB RAM)** × 3台
   - 高性能な画像処理に必要な8GBモデルを選定
   - ヒートシンク付きで安定動作を確保
   
2. **Raspberry Pi High Quality Camera** × 3台
   - 12.3メガピクセルのソニー製センサー搭載
   - Cマウント/CSマウント対応で柔軟なレンズ選択が可能
   
3. **専用レンズ**
   - 実験要件に合わせた交換レンズを購入
   
4. **Intel RealSense Depth Camera D435if** (検討中)
   - 深度情報取得用の参考機材として調査
   - 価格: ¥60,500 (Amazon.co.jp)

#### 📸 到着した機材の写真
- Raspberry Pi 4 本体パッケージ
- High Quality Camera モジュール
- 今後の拡張を見据えた Intel RealSense の調査資料

#### 次のステップ
- [ ] Raspberry Pi のOS セットアップ
- [ ] カメラモジュールの動作確認
- [ ] 基本的な画像キャプチャスクリプトの作成
- [ ] MultiDIC との連携方法の検討

---

### 2025年7月 - プロジェクト始動

#### プロトタイプ開発計画
- **見積もり担当**: @chan-k-346 → @tsuzuki20
- **ハードウェア構築**: @chan-k-346, @Yutotakahashi
- **ソフトウェア理解**: @chan-k-346, @Yutotakahashi

#### 関連ドキュメント
- [議事録](./docs/meeting_notes.md) (準備中)
- [開発方針](./docs/development_policy.md) (準備中)

---

## 🔧 技術仕様

### ハードウェア構成
- **コンピュータ**: Raspberry Pi 4 Model B (8GB)
- **カメラ**: Raspberry Pi High Quality Camera
- **レンズ**: Cマウント/CSマウント互換レンズ
- **台数**: 3セット（マルチビューDIC用）

### ソフトウェア構成
- **OS**: Raspberry Pi OS (64-bit推奨)
- **DICエンジン**: MultiDIC (MATLAB)
- **画像取得**: Python (picamera2ライブラリ)
- **インターフェース**: Python-MATLAB連携

---

## 📚 参考資料

### MultiDIC オリジナルドキュメント
- [MultiDIC 公式リポジトリ](https://github.com/SolavLab/MultiDIC)
- [インストラクションマニュアル](./docs/pdf/MultiDIC_v_1_1_0_instruction_manual.pdf)
- [DIC プロジェクトレポート (RAPHAEL GUEGAN)](./Manual/Report_Project_DIC_RAPHAEL_GUEGAN.pdf)

### 関連リンク
- [Raspberry Pi 公式ドキュメント](https://www.raspberrypi.org/documentation/)
- [picamera2 ライブラリ](https://github.com/raspberrypi/picamera2)

---

## 🚀 今後の開発予定

### Phase 1: 基礎構築 (2025年8月〜9月)
- Raspberry Pi セットアップ自動化スクリプト
- カメラキャリブレーション補助ツール
- リアルタイム画像プレビュー機能

### Phase 2: MultiDIC統合 (2025年10月〜11月)
- Python-MATLAB ブリッジの実装
- 自動画像転送システム
- バッチ処理スクリプト

### Phase 3: 最適化と拡張 (2025年12月〜)
- エッジコンピューティング対応
- リアルタイムDIC処理の検討
- Web UIの開発

---

## 📄 ライセンス
このプロジェクトは元の MultiDIC のライセンスに従います。詳細は [LICENSE.txt](./LICENSE.txt) を参照してください。

---

## 👥 開発チーム
- @chan-k-346 - プロジェクトリード、ハードウェア担当
- @Yutotakahashi - ハードウェア・ソフトウェア開発
- @tsuzuki20 - 見積もり・調達担当

---

*最終更新: 2025年8月21日*

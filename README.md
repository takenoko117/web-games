# 🎮 takenoko117 Web Games Portal

ブラウザからインストール不要ですぐに遊べる、**takenoko117** 制作のオリジナル Web ゲーム＆インタラクティブ・シミュレーター集です。  
すべてのタイトルは **GitHub Pages** 上で公開されており、PC・スマホブラウザからワンクリックでプレイできます。各リポジトリの最新コミットを自動取得し、常に最新アップデート順で確認・プレイ可能です。

🌐 **ポータルサイトで一覧を見る**: **[https://takenoko117.github.io/web-games/](https://takenoko117.github.io/web-games/)**

---

## 🕹️ ゲーム一覧（クイックリンク）

| タイトル | ジャンル | 技術スタック | プレイリンク (GitHub Pages) | ソースコード |
| :--- | :--- | :--- | :---: | :---: |
| **👾 ネームバトラー (Name Battler)** | ポケモンライク・自律ハッシュバトル | TypeScript / Vite / Canvas / Web Audio | [**▶ 今すぐ遊ぶ**](https://takenoko117.github.io/Pokemon_like_name_battle/) | [📦 Repo](https://github.com/takenoko117/Pokemon_like_name_battle) |
| **⚔️ ぐにゃぐにゃバトル** | TABS風 3Dボクセル物理バトル（全40面＋サンドボックス） | TypeScript / Three.js / 独自Verlet物理 | [**▶ 今すぐ遊ぶ**](https://takenoko117.github.io/TABS_like_claudeOpus5.5/) | [📦 Repo](https://github.com/takenoko117/TABS_like_claudeOpus5.5) |
| **⚛️ FUSION GENESIS** | 核融合・拡大再生産シミュレーター (v2.0) | HTML5 / Canvas / Vanilla JS | [**▶ 今すぐ遊ぶ**](https://takenoko117.github.io/fusion_game/) | [📦 Repo](https://github.com/takenoko117/fusion_game) |
| **🌌 Multiverse Creator** | 30大物理定数・多元宇宙シミュレーター | React / TypeScript / Three.js | [**▶ 今すぐ遊ぶ**](https://takenoko117.github.io/random_universe_sim/) | [📦 Repo](https://github.com/takenoko117/random_universe_sim) |
| **⚡ NEON SURVIVOR** | ヴァンサバ系レトロネオン・ハック＆スラッシュ | HTML5 Canvas / Web Audio API / PWA | [**▶ 今すぐ遊ぶ**](https://takenoko117.github.io/NEON-SURVIVOR/) | [📦 Repo](https://github.com/takenoko117/NEON-SURVIVOR) |
| **🛡️ WOBBLE VOXEL WARS** | 3D TABSライク物理バトルシミュレーター | TypeScript / Three.js / Web Audio | [**▶ 今すぐ遊ぶ**](https://takenoko117.github.io/TABS_like/) | [📦 Repo](https://github.com/takenoko117/TABS_like) |

---

## 📖 各ゲームの詳細紹介

### 1. 👾 ネームバトラー (Name Battler)

* 🌐 **プレイURL**: [https://takenoko117.github.io/Pokemon_like_name_battle/](https://takenoko117.github.io/Pokemon_like_name_battle/)
* 📦 **リポジトリ**: [takenoko117/Pokemon_like_name_battle](https://github.com/takenoko117/Pokemon_like_name_battle)
* 🏷️ **ジャンル**: ポケモンライク / ネームジェネレーター＆オートバトル

**【概要】**  
入力された文字列（名前）から、ステータス・タイプ・技・グラフィックを自律生成し、ポケモン完全準拠のルールで1vs1のオートバトルを繰り広げるウェブゲームです。同じ名前を入力すれば、常に全く同じモンスターが誕生します。

**【主な特徴】**
- **名前から生まれるモンスター（ハッシュ生成）**: 入力された名前のハッシュ値から、ステータス（HP, A, B, C, D, S）、全18タイプの属性、技、左右対称ドット絵（192×192）を決定論的に生成。
- **正規分布による強さのばらつき（種族値合計 60 〜 1200）**: 平均600前後を基準に、1000超えの「神個体」や100未満の「最弱個体」が稀に出現するガチャ感覚のワクワク感。
- **ポケモン完全準拠のバトルシステム**: 全18タイプ相性、タイプ一致補正（STAB 1.5倍）、技命中率判定、急所（1/24で1.5倍）、乱数（0.85〜1.00）、レベル50固定の公式ダメージ計算式を採用。
- **スマートオートAI & 速度調整**: 習得した技から相手のタイプ弱点や最大期待ダメージを自律判断するAI、1x / 2x / 4x / SKIP の速度変更、Web Audio APIによるシンセ効果音を搭載。

---

### 2. ⚔️ ぐにゃぐにゃバトル — 物理バトルシミュレーター

* 🌐 **プレイURL**: [https://takenoko117.github.io/TABS_like_claudeOpus5.5/](https://takenoko117.github.io/TABS_like_claudeOpus5.5/)
* 📦 **リポジトリ**: [takenoko117/TABS_like_claudeOpus5.5](https://github.com/takenoko117/TABS_like_claudeOpus5.5)
* 🏷️ **ジャンル**: 3D ボクセルラグドール・物理タクティカルバトルシミュレーター

**【概要】**  
『Totally Accurate Battle Simulator (TABS)』風の、独自 Verlet 物理エンジン＆ボクセルラグドールで動く 3D 物理バトルシミュレーターです。関節のばね制御でぐにゃぐにゃと歩き、殴り合い、吹き飛び、部位が砕け散るコミカルかつ戦略的な合戦を楽しめます。

**【主な特徴】**
- **超拡張アーケードモード（全40面）＆サンドボックス**:
  - 第1部（基礎歩兵〜巨獣・帝国軍）、第2部（現代兵器・神々の使徒襲来）、第3部〜第4部（天候演出・状態異常ハザード）まで段階的に攻略するタクティカルモード。
  - 制限なしで両軍に自由配置・実験できるサンドボックスモード＆ワンクリック「プリセット編成」を搭載。
- **個性豊かな全33兵種＋防衛施設**:
  - 歩兵・盾兵・槍兵・弓兵・爆弾兵・魔術師・騎兵・大砲・巨人・鎧戦象・ドラゴンなどのファンタジー兵種。
  - 暴走バギー・超巨大戦車・巨大ロボット・霊峰神「ヤマムロン」、使徒神（サキエル・ラミエル・サハクィエル・ゼルエル）、デオキシス、巨大グランドピアノ＆ブロンド長髪女性ピアニストの「ホンゴン」など多彩なユニットが登場。
- **多彩な地形ギミック**: 渓谷の一本橋と奈落、石柱群の飛び道具遮蔽、側面奇襲ゾーン、増殖ゲート、三軍同時展開ゾーンなど。
- **充実の観戦カメラ**: オービット操作、ユニットクリック追従カメラ、スローモーション（`0.25x`）・倍速（`2x`）再生に対応。

---

### 3. ⚛️ FUSION GENESIS: 核融合 拡大再生産シミュレーター

* 🌐 **プレイURL**: [https://takenoko117.github.io/fusion_game/](https://takenoko117.github.io/fusion_game/)
* 📦 **リポジトリ**: [takenoko117/fusion_game](https://github.com/takenoko117/fusion_game)
* 🏷️ **ジャンル**: 科学インクリメンタル / ファクトリー系拡大再生産シミュレーション

**【概要】**  
素粒子物理からプラズマ核融合までを実際に体験しながら学べる拡大再生産シミュレーションゲームです。クォークと電子の射出から始まり、ハドロン合成、水素同位体（重水素 $\text{D}$・三重水素 $\text{T}$）の精製、トカマク炉心での磁気パルス点火、そしてリチウム増殖ブランケットによるトリチウム自律増殖サイクルの構築を目指します。

**【主な特徴】**
- **素粒子・核物理の忠実な再現**: アップ/ダウンクォークの強相互作用による陽子・中性子合成から D-T 核融合反応（$17.59\text{ MeV}$）、v2.0 Hyper-Torus大型炉心までをリアルタイムに可視化。
- **自律増殖ループ（TBR > 1.05）**: 核融合で発生した高速中性子をリチウムブランケットで捕獲し、消費した以上の三重水素を増殖させる拡大再生産システム。
- **充実の攻略手順書 & 数式解説**: 5大フェーズによる最短攻略ロードマップやKaTeXによる数式レンダリングを内蔵。

---

### 4. 🌌 Multiverse Creator (マルチバース・クリエイター)

* 🌐 **プレイURL**: [https://takenoko117.github.io/random_universe_sim/](https://takenoko117.github.io/random_universe_sim/)
* 📦 **リポジトリ**: [takenoko117/random_universe_sim](https://github.com/takenoko117/random_universe_sim)
* 🏷️ **ジャンル**: 宇宙論・素粒子物理インタラクティブ・サイエンスシミュレーター

**【概要】**  
素粒子物理学および宇宙論の標準模型における**約30種類のハイパーパラメータ（微細構造定数、ヒッグス真空期待値、宇宙項密度など）**をランダムまたは手動で改変し、多元宇宙（マルチバース）仮説のもとで誕生する宇宙の運命や知的生命誕生の可能性をシミュレートします。

**【主な特徴】**
- **マルチバース・ルーレット（宇宙ガチャ）**: 微小ゆらぎ（$\pm 10\%$）から超混沌カオス（$10^{-4}\times \sim 10^{4}\times$）まで、ワンクリックで未知の物理法則を持つ宇宙を生成。
- **デュアルスケール観測（3D & 2D）**: Three.js による銀河（2,800個以上・恒星28万個）・コズミックウェブの3Dマクロビューと、Canvas 2D によるクォーク・原子核・電子軌道のミクロビューを同時表示。
- **8段階の宇宙進化アセスメント**: 時空次元、陽子安定性、ビッグバン元素合成、恒星核融合、生命居住可能性などをリアルタイムで診断。

---

### 5. ⚡ NEON SURVIVOR - Retro Neon Hack & Slash

* 🌐 **プレイURL**: [https://takenoko117.github.io/NEON-SURVIVOR/](https://takenoko117.github.io/NEON-SURVIVOR/)
* 📦 **リポジトリ**: [takenoko117/NEON-SURVIVOR](https://github.com/takenoko117/NEON-SURVIVOR)
* 🏷️ **ジャンル**: ヴァンパイアサバイバー系 2D ローグライト・アクション

**【概要】**  
サイバー・レトロネオンな世界観で無数の敵をなぎ倒す、『Vampire Survivors』ライクな爽快ハック＆スラッシュゲームです。外部ライブラリに頼らない軽量な Vanilla JS + HTML5 Canvas 設計と、Web Audio API によるリアルタイム波形合成サウンドで軽快に動作します。

**【主な特徴】**
- **多彩な武器ビルドとインフレ成長**: レベルアップで武器やパッシブスキルを選択・強化し、画面を埋め尽くす弾幕とエフェクトで敵の大群を殲滅。
- **多彩なゲームモード**: 通常モードに加え、高難度モードやオートラン、ボスラッシュなどやり込み要素を搭載。
- **PWA対応 & バランスエディタ同梱**: スマホ・PCの両方で快適に遊べるレスポンシブ設計。

---

### 6. 🛡️ WOBBLE VOXEL WARS - 3D TABSライク物理バトルシミュレーター

* 🌐 **プレイURL**: [https://takenoko117.github.io/TABS_like/](https://takenoko117.github.io/TABS_like/)
* 📦 **リポジトリ**: [takenoko117/TABS_like](https://github.com/takenoko117/TABS_like)
* 🏷️ **ジャンル**: 3D ボクセル物理合戦シミュレーター

**【概要】**  
赤軍（RED ARMY）と青軍（BLUE ARMY）のユニットをフィールドに自由配置し、物理演算による予測不能な 3D ボクセル合戦を観戦・実験できるバトルシミュレーターです。

**【主な特徴】**
- **直感的な部隊配置とプリセット合戦**: ワンクリックで呼び出せる「サンプル布陣」や自由なユニット配置で、すぐに大規模な合戦を開始可能。
- **リアルタイム統計と演出**: 両軍の生存数・コスト合計の表示、タイムスケール変更、Web Audio による効果音演出を搭載。

---

## 👤 Author

* **GitHub**: [@takenoko117](https://github.com/takenoko117)

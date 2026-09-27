# 効果音の出典とライセンス

Day2 の表彰スライドで使う音源です。
**いずれもパブリックドメイン（著作権消滅・権利放棄）の素材**で、商用・公的機関の利用ともに可能、
クレジット表記の義務もありません（念のため本ファイルに記録として残しています）。

| ファイル | 用途 | 元素材 | ライセンス |
|---|---|---|---|
| `drumroll.mp3` | ドラムロール（ループ再生） | [Drum Roll - Concert Band - United States Air Force Band](https://commons.wikimedia.org/wiki/File:Drum_Roll_-_Concert_Band_-_United_States_Air_Force_Band.mp3)（Esprit de Corps, 1997 収録） | **パブリックドメイン**（米空軍バンド＝米国連邦政府の著作物。[公式の配布ページ](https://www.music.af.mil/Multimedia/Music/Public-Domain-Music/)） |
| `reveal.mp3` | 発表の瞬間のシンバル | [CrashCymbalSample.ogg](https://commons.wikimedia.org/wiki/File:CrashCymbalSample.ogg) | **パブリックドメイン**（作者による権利放棄） |

## 加工の内容
元素材をそのまま使わず、ffmpeg で以下の加工をしています（PDのため加工・再配布とも問題なし）。

- `drumroll.mp3` … 原曲 6.0〜26.0秒（持続するロール部分）を20秒切り出し。モノラル/44.1kHz/128kbps。
  前後に30msのフェードを入れ、**ループ再生してもつなぎ目が目立たない**ようにしてある。ピーク0.73に正規化。
- `reveal.mp3` … 原素材 38.40秒から2.6秒を切り出し（最も鳴っている瞬間から始まるので、頭から一気に鳴る）。
  末尾1.2秒でフェードアウト。ピーク0.95に正規化。

再生成が必要になった場合は、上記2つの元ファイルを Wikimedia Commons から取得し、同じ区間・同じ正規化で作り直せます。

## 検討したが採用しなかったもの
- **効果音ラボ** … 商用無料で質は高いが、利用規約で「アプリの組み込み素材」としての利用と直リンクが**禁止**されているため不採用。
- **Pixabay / DOVA-SYNDROME** … 利用は可能だが、規約が「素材としての再配布」に制限をかけており、
  資料一式を関係者に配布する運用を考えると、権利の切れているPD素材のほうが安全と判断。
- **Gravity Sound（CC BY 4.0）** … 音は良いがクレジット表記が義務。公的機関の資料に表記を足す必要が出るため見送り。

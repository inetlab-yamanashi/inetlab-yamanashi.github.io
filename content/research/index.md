---
title: "研究"
---

私たちは，コンピュータサイエンスの知恵を駆使して，インターネットという巨大な社会基盤をより効率よく，より安全に動かすための研究に取り組んでいます．数理的なアプローチやシミュレーションを通じて，現実社会に潜む複雑な課題を論理的に解き明かし，実際のシステム設計や運用に役立つ形へとつなげていくのが私たちのスタイルです．学問としての探求と社会への貢献を両立させながら，将来のネットワークを支える基盤技術を育てています．

詳細な文献リストは [researchmap](https://researchmap.jp/takeru_inoue) や [Google Scholar](https://scholar.google.co.jp/citations?user=dFfLTSAAAAAJ) をご覧ください．

---

### AI計算基盤：巨大なAIを支える超高速・省電力なネットワーク

![datacenter](/img/datacenter.jpg)

ChatGPTなどの巨大なAIを育てるには，数万枚のGPUという計算チップを連携させる「AIクラスタ網」という特別なインフラが欠かせません．現在の課題は，GPU同士の通信でわずかな渋滞（データ同士の衝突）が起きるだけでAI全体の学習効率が大きく落ちてしまうことです．井上研究室では，大手通信事業者との共同研究などを通じ，光のスイッチでネットワークの形を計算内容に合わせて自由に変える「可変ネットワーク」という画期的な仕組みに挑戦しています．数理モデルに基づく設計とコンピュータシミュレーションを武器に，AI学習を圧倒的に速く，かつ低電力で実現するインフラの構築を目指します．こうした取り組みを通じて，最新のネットワーク技術と，数学的なアイデアを設計や実装に落とし込む考え方を，社会の中で使える形に磨いていきます．

- [助川公基, 井上武, 松田奈々, 間野暢, 曽根由明, "光セレクタを用いた可変 2D トーラス相互結合網に関する数理的検討," 信学総大 B-7-36, 2026.](https://pub.confit.atlas.jp/ja/event/general2026/presentation/B-7-36)
- [Takeru Inoue, Toru Mano, Takeaki Uno, "Efficient Evaluation of Nonblocking Property of Optical Circuit-Switched Clos Networks with Non-Uniform Link Distribution," Computer Networks, 276 112008, 2026.](https://doi.org/10.1016/j.comnet.2026.112008)
- Takeru Inoue, Nariaki Tateiwa, Yoshiaki Sone, Koichi Takasugi, Masahisa Kawashima, "Exploring Optical Interconnect Architectures for Scalable and High-performance AI Clusters," in Proc. of PhotonIcs and Electromagnetics Research Symposium (PIERS), 2025.

---

### 通信インフラの防災：災害時でも「繋がる」安心を設計する

![disaster](/img/disaster.jpg)

地震や豪雨などの災害が起きたとき，救助や連絡の「命綱」となるのがインターネットです．私たちは，大手通信事業者や土木分野の研究者と協力し，地下管路や電柱などの通信設備のダメージをAIで予測したり，数千億通り以上の膨大な故障パターンから「ネットワークが正しく繋がっているか」を厳密に計算する独自の技術を開発しています．目指しているのは，単に壊れないだけでなく，たとえ一部が壊れても即座に代わりのルートを見つけて復旧する「強靱（レジリエンス）」な社会インフラの実現です．こうした研究は，災害に備えた設備投資や復旧計画の検討を，データと論理に基づいて支えるための基盤になります．

- [井上 武, 中村 健吾, 西野 正彬, 松田 奈々, 伊藤 陽, "[招待講演] 通信地下管路の被災予測技術を用いた情報通信ネットワークの地震リスク評価と強靱化," 電子情報通信学会 ネットワークシステム研究会, NS2025-176, 2025.](https://ken.ieice.org/ken/paper/20251219FcPN/)
- [Takeru Inoue, Masaaki Nishino, Akira Ito, Yoshiaki Sone, "Fortifying Communication Networks against Strong Earthquakes Using Real Conduit Damage Records," IEEE/Optica Journal of Lightwave Technology, 43(18) 8586-8602, 2025.](https://doi.org/10.1109/JLT.2025.3591108)
- [Takeru Inoue, Akira Ito, Kengo Nakamura, Tatsuya Matsukawa, "Impact of Facility Factors on Robustness of Communication Networks under Natural Disasters," IEEE Communications Magazine, 63(1) 138-144, 2025.](https://doi.org/10.1109/mcom.001.2300741)

---

### 運用・セキュリティ：複雑なネットワークを，賢く・安全に管理する

![operation](/img/operation.jpg)

インターネットの裏側では，膨大な数の機器が複雑に組み合わさって動いています．たった一行の設定ミスが大規模な通信障害を招くこともあるため，私たちはネットワークの構成を仮想空間に再現する「デジタルツイン」技術や，設定の誤りをコンピュータで自動的に検証する仕組みを研究しています．また，ネットワークの状態変化をリアルタイムに可視化し，トラブルを早期に発見するための監視システムの開発にも取り組んでいます．成果の一部は，山梨大学の情報処理教室において，試験中のみ生成AIなどの特定のサイトへのアクセスを制限する「試験モード」として実際に導入・運用されており，教育現場の公平性を守るためにも役立てられています．この研究を通じて，複雑なシステムを論理的に捉え，安全性や運用の確かさを高めるための「一歩先のセキュリティ・エンジニアリング」を形にしていきます．

- 保坂 一希, 井上 武, 吉川 雅修, "情報処理教室の試験モード実装によるAIドメインへのアクセス制限," 日本教育工学会 春期全国大会, 2-S13N3, 2026.
- [Kazuya Anazawa, Takeru Inoue, Toru Mano, Hiroshi Ou, Hirotaka Ujikawa, Dmitrii Briantcev, Sumaiya Binte Ali, Devika Dass, Hideki Nishizawa, Yoshiaki Sone, Eoin Kenny, Marco Ruffini, Daniel Kilper, Eiji Oki, Koichi Takasugi, "Experimental evaluation of an SDN controller for open optical-circuit-switched networks," Journal of Optical Communications and Networking, 17(6) 498-498, 2025.](https://doi.org/10.1364/jocn.558407)

---

### Graphillion：天文学的なネットワークのパターンを自在に操る

![graphillion](/img/graphillion.jpg)

井上研究室の大きな武器の一つが，10年以上にわたって開発・公開を続けているオープンソース・ソフトウェア「Graphillion（グラフィリオン）」です．通信インフラのような複雑なネットワークを分析する際，故障や経路の組み合わせは天文学的な数に膨れ上がり，通常の計算手法では太刀打ちできません．私たちは，巨大なデータを効率よく圧縮して処理する「決定グラフ」というアルゴリズムを駆使し，複雑なパズルのようなネットワークの問題を瞬時に解き明かす仕組みを提供しています．この成果は https://graphillion.org で公開されており，世界中の誰もがダウンロードしてすぐに利用できるようになっています．研究と実装を往復しながら，ネットワークを正確に分析するためのアルゴリズム基盤を育て，現実の課題に適用できる形で提供していきます．

- [YouTube](https://youtube.com/playlist?list=PLg12KU_3EZvY1VGVoMk5lpw9BMvD-7Hbn)
- [Takeru Inoue, Norihito Yasuda, Hidetomo Nabeshima, Masaaki Nishino, Shuhei Denzumi, Shin-ichi Minoato, "International Competition on Graph Counting Algorithms 2023," IEICE Transactions on Fundamentals of Electronics, Communications and Computer Sciences, E107.A(9) 1441-1451, 2024.](https://doi.org/10.1587/transfun.2023dmp0006)
- [Takeru Inoue, Hiroaki Iwashita, Jun Kawahara, Shin-ichi Minato, "Graphillion: software library for very large sets of labeled graphs," International Journal on Software Tools for Technology Transfer, 18(1) 57-66, 2016.](https://doi.org/10.1007/s10009-014-0352-z)
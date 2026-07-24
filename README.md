<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>インタビュー：5年越しの出版に込められた想い | 優 You</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;1,300&family=Noto+Serif+JP:wght@200;300;400;600&display=swap" rel="stylesheet">
    
    <style>
        :root {
            --bg-color: #fcfbf9;
            --text-main: #242424;
            --text-sub: #5a5550;
            --accent-color: #8c7b6e;
            --band-bg: #e6e0d5;
            --light-gray: #e8e6e1;
            --font-serif: 'Noto Serif JP', serif;
            --font-en: 'Cormorant Garamond', serif;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: var(--font-serif);
            color: var(--text-main);
            background-color: var(--bg-color);
            line-height: 2;
            letter-spacing: 0.05em;
            -webkit-font-smoothing: antialiased;
        }

        /* ヘッダー */
        header {
            background-color: rgba(252, 251, 249, 0.95);
            backdrop-filter: blur(8px);
            padding: 2rem 5%;
            position: sticky;
            top: 0;
            z-index: 1000;
            border-bottom: 1px solid rgba(232, 230, 225, 0.5);
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        header h1 {
            font-size: 1rem;
            letter-spacing: 0.2em;
            font-weight: 300;
        }

        header h1 a {
            color: var(--text-main);
            text-decoration: none;
            transition: opacity 0.3s;
        }

        header h1 a:hover {
            opacity: 0.6;
        }

        nav a {
            color: var(--text-main);
            text-decoration: none;
            font-size: 0.8rem;
            font-family: var(--font-en);
            letter-spacing: 0.15em;
            transition: opacity 0.3s;
        }

        nav a:hover {
            opacity: 0.6;
        }

        /* メインコンテナ */
        .interview-container {
            max-width: 820px;
            margin: 0 auto;
            padding: 80px 30px 60px;
        }

        /* タイトルエリア */
        .interview-header {
            margin-bottom: 80px;
            text-align: center;
            border-bottom: 1px solid var(--light-gray);
            padding-bottom: 60px;
        }

        .interview-eyebrow {
            font-size: 0.85rem;
            color: var(--accent-color);
            letter-spacing: 0.25em;
            text-transform: uppercase;
            font-family: var(--font-en);
            margin-bottom: 20px;
            font-weight: 400;
        }

        .interview-header h1 {
            font-size: 2.2rem;
            font-weight: 300;
            margin-bottom: 25px;
            line-height: 1.6;
            letter-spacing: 0.08em;
        }

        .interview-lead {
            font-size: 1rem;
            color: var(--text-sub);
            line-height: 2;
            max-width: 700px;
            margin: 0 auto 40px;
            font-weight: 300;
        }

        .interview-meta {
            display: flex;
            justify-content: center;
            gap: 30px;
            flex-wrap: wrap;
            font-size: 0.85rem;
            color: var(--text-sub);
            font-family: var(--font-en);
            letter-spacing: 0.1em;
        }

        .meta-item {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 5px;
        }

        .meta-label {
            color: var(--accent-color);
            font-weight: 400;
        }

        /* インタビュアー紹介 */
        .interviewer-info {
            background-color: var(--band-bg);
            padding: 40px 30px;
            margin: 60px 0;
            border-left: 3px solid var(--accent-color);
            border-radius: 16px;
        }

        .interviewer-info p {
            margin-bottom: 10px;
        }

        .interviewer-info p:last-child {
            margin-bottom: 0;
        }

        /* セクション */
        .interview-section {
            margin: 80px 0;
            padding: 50px 0;
            border-bottom: 1px solid var(--light-gray);
        }

        .interview-section:last-of-type {
            border-bottom: none;
        }

        .section-title {
            font-size: 1.5rem;
            font-weight: 400;
            margin-bottom: 10px;
            letter-spacing: 0.1em;
            color: var(--text-main);
        }

        .section-number {
            color: var(--accent-color);
            font-size: 0.9rem;
            font-family: var(--font-en);
            letter-spacing: 0.15em;
            display: block;
            margin-bottom: 5px;
        }

        /* Q&A */
        .qa-block {
            margin: 40px 0;
        }

        .question {
            background-color: #f8f6f1;
            padding: 25px 30px;
            margin-bottom: 25px;
            border-left: 4px solid var(--accent-color);
            border-radius: 12px;
            font-size: 0.98rem;
            line-height: 2;
        }

        .question::before {
            content: '【質問】';
            color: var(--accent-color);
            font-weight: 600;
            display: block;
            margin-bottom: 12px;
            font-family: var(--font-serif);
            font-size: 0.95rem;
        }

        .answer {
            padding: 0 20px;
            font-size: 0.97rem;
            line-height: 2.1;
            text-align: justify;
        }

        .answer p {
            margin-bottom: 20px;
        }

        .answer p:last-child {
            margin-bottom: 0;
        }

        .answer::before {
            content: '【回答】';
            color: var(--accent-color);
            font-weight: 600;
            display: block;
            margin-bottom: 15px;
            font-family: var(--font-serif);
            font-size: 0.95rem;
        }

        /* 引用 */
        .pullquote {
            border-left: 4px solid var(--accent-color);
            padding: 30px;
            margin: 50px 0;
            background-color: rgba(140, 123, 110, 0.04);
            font-size: 1.05rem;
            font-weight: 400;
            line-height: 2.1;
            text-align: center;
            color: var(--text-sub);
        }

        /* 写真セクション */
        .photo-section {
            margin: 60px 0;
            text-align: center;
        }

        .photo-container {
            max-width: 100%;
            margin: 30px 0;
            overflow: hidden;
            border-radius: 12px;
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.08);
        }

        .photo-container img {
            width: 100%;
            height: auto;
            display: block;
            filter: sepia(0.12) contrast(0.98);
        }

        .photo-caption {
            font-size: 0.85rem;
            color: var(--text-sub);
            margin-top: 15px;
            font-style: italic;
            letter-spacing: 0.05em;
        }

        /* 観察メモ */
        .observation {
            background-color: #f5f3ee;
            padding: 20px 25px;
            margin: 30px 0;
            border-left: 3px solid var(--light-gray);
            font-size: 0.9rem;
            color: var(--text-sub);
            font-style: italic;
            line-height: 1.9;
        }

        /* フッター */
        footer {
            background-color: var(--band-bg);
            padding: 60px 30px;
            text-align: center;
            border-top: 1px solid var(--light-gray);
            margin-top: 100px;
            border-radius: 16px 16px 0 0;
        }

        .footer-meta {
            font-size: 0.85rem;
            color: var(--text-sub);
            margin-bottom: 20px;
            font-family: var(--font-en);
            letter-spacing: 0.1em;
        }

        .back-link {
            display: inline-block;
            color: var(--accent-color);
            text-decoration: none;
            font-size: 0.9rem;
            margin-top: 20px;
            transition: opacity 0.3s;
        }

        .back-link:hover {
            opacity: 0.6;
        }

        @media (max-width: 600px) {
            .interview-container {
                padding: 60px 20px 40px;
            }

            .interview-header h1 {
                font-size: 1.7rem;
            }

            .interview-lead {
                font-size: 0.95rem;
            }

            .question,
            .answer {
                font-size: 0.95rem;
            }

            .interview-meta {
                gap: 15px;
            }
        }
    </style>
</head>
<body>

    <header>
        <h1><a href="/">優 | You</a></h1>
        <nav>
            <a href="/#publication">出版情報へ</a>
        </nav>
    </header>

    <div class="interview-container">

        <!-- ヘッダー -->
        <div class="interview-header">
            <span class="interview-eyebrow">Special Interview</span>
            <h1>5年越しの出版に込められた想い<br>〜『私には帰る場所がない』制作秘話〜</h1>
            <p class="interview-lead">
                デザインエッグ社から2026年秋に出版される『私には帰る"場所"がない』。その5年にわたる執筆期間、文体の変化、そして現代社会への問いを、著者・優さんに聞いた。
            </p>
            <div class="interview-meta">
                <div class="meta-item">
                    <span class="meta-label">取材日</span>
                    <span>2026年7月〇日</span>
                </div>
                <div class="meta-item">
                    <span class="meta-label">インタビュアー</span>
                    <span>〇〇〇〇</span>
                </div>
                <div class="meta-item">
                    <span class="meta-label">聞き手・構成</span>
                    <span>編集部</span>
                </div>
            </div>
        </div>

        <!-- インタビュアー紹介 -->
        <div class="interviewer-info">
            <p><strong>このインタビューについて</strong></p>
            <p>本稿は、デビュー作『私には帰る"場所"がない』の出版を控える著者・優さんへの独占インタビューです。5年間の執筆プロセス、言語化と生存の関係、そして現代社会への問いが綴られています。</p>
        </div>

        <!-- セクション1 -->
        <div class="interview-section">
            <span class="section-number">第一章</span>
            <h2 class="section-title">導入：5年という「空白」の真相</h2>

            <div class="qa-block">
                <div class="question">
                    ついに、5年越しのご出版ということで、本当におめでとうございます。読者の方々にとっても『待ちに待った』という瞬間だと思います。決して短くないこの期間、あえて原稿を寝かせていたのか、あるいは葛藤があったのか……。この5年という時間を置いたからこそ見えたものは何でしょうか？
                </div>

                <div class="answer">
                    <p>ありがとうございます。本当に長い期間でしたね。当初、私はこの執筆を一気に完成させるつもりでいました。でも、執筆を進めるうちに、自分が何を本当に伝えたいのか、それが曖昧だと感じるようになった。</p>
                    <p>初期段階では、感情が全面に出た、いわば "尖った" 文体でした。しかし5年という時間は、その熱量を冷ましながらも、より本質的なものへ昇華させてくれた。何度も推敲し、何度も自分と対話することで、ようやく『これだ』という手応えを感じることができたんです。</p>
                </div>
            </div>

            <div class="observation">
                ※ ここで優さんは視線を落とし、5年前を懐かしむように笑った。
            </div>
        </div>

        <!-- 写真1：執筆の現場 -->
        <div class="photo-section">
            <div class="photo-container">
                <img src="https://via.placeholder.com/820x380?text=Workspace" alt="執筆ノートとペン">
            </div>
            <p class="photo-caption">5年間、優さんが執筆に使い続けたノートとペン。ページの端々に推敲の跡が残る。</p>
        </div>

        <!-- セクション2 -->
        <div class="interview-section">
            <span class="section-number">第二章</span>
            <h2 class="section-title">核心：「書く」という行為の本質</h2>

            <div class="qa-block">
                <div class="question">
                    本書を読んでいると、言葉の一つひとつに、単なる文章を超えた執念のようなものを感じます。そもそも優さんは、なぜ書くのでしょうか？世の中には、思っていることがあっても胸にしまっておく人もいれば、喋って発散する人もいます。その中で、あえて『言語化する』という道を選んだ理由は？
                </div>

                <div class="answer">
                    <p>それは、私にとって生存そのものなんです。言葉がなければ、私は存在を実感することができない。</p>
                    <p>幼少期から、私の意見や感情は家庭内で否定され続けました。その過程で、「自分の思いを言葉にすることは危険である」という恐怖が根付いた。しかし同時に、言葉を失うことは『自分を失うこと』と同義だった。だから、私は言葉を手放すことができなかった。</p>
                    <p>だから、書くことは私にとって単なる表現ではなく、自己確認の儀式であり、生存の証明なんです。そして、その痛みを通してしか、私は自分の輪郭を感じることができないんです。</p>
                </div>
            </div>

            <div class="pullquote">
                「書くことは、私にとって単なる表現ではなく、自己確認の儀式であり、生存の証明である」
            </div>

            <!-- 写真2：思考の軌跡 -->
            <div class="photo-section">
                <div class="photo-container">
                    <img src="https://via.placeholder.com/820x380?text=Manuscripts" alt="原稿の推敲跡">
                </div>
                <p class="photo-caption">何度も推敲された原稿ページ。書き込みと修正が、5年間の思考の歩みを記録している。</p>
            </div>
        </div>

        <!-- セクション3 -->
        <div class="interview-section">
            <span class="section-number">第三章</span>
            <h2 class="section-title">『帰る場所がない』というタイトルの真意</h2>

            <div class="qa-block">
                <div class="question">
                    本のタイトル『私には帰る"場所"がない』について、質問させてください。これまで友人知人に少なからず反響をいただいたと思いますが、この『帰る場所』という言葉には、物理的な家や故郷という意味合いだけでなく、精神的な拠り所や、ありのままの自分でいられる空間という深層的な意味が込められているのではないでしょうか？
                </div>

                <div class="answer">
                    <p>文字通り、私には帰る場所がありません。それは実家がないといった物理的な意味です。これは、一見幸福で豊かに見える位相においても、多くの人が抱えている喪失の一形態なのだと考えています。</p>
                    <p>生きるなかで何がしかの喪失体験からは避けられ得ず、そして往々にして人はその喪のプロセスを辿り、生涯をかけて昇華していくものです。しかし、それを安易に『乗り越えた』『成長した』と切り取ることは、その人が経験した痛みの本質を見失わせてしまいます。</p>
                    <p>そして、読者もそれは恐らく望んでいません。なぜなら、それは人の不幸を愉しむシャーデンフロイデの意味合いではなく、生きる上で避けられない苦しさへの共感と、その苦しさを言葉にする勇気への敬意だからです。</p>
                    <p>やはりこの不景気なご時世でお金を払ってわざわざ私の書籍を手に取って購入しようと決めてくださる以上は、確かな読了感を得ていただきたいと思っています。</p>
                </div>
            </div>
        </div>

        <!-- 写真3：執筆空間 -->
        <div class="photo-section">
            <div class="photo-container">
                <img src="https://via.placeholder.com/820x380?text=Writing+Space" alt="執筆環境">
            </div>
            <p class="photo-caption">優さんが日々執筆する空間。机上には参考文献と執筆ノートが並ぶ。5年間、ここで言葉と向き合い続けた。</p>
        </div>

        <!-- セクション4 -->
        <div class="interview-section">
            <span class="section-number">第四章</span>
            <h2 class="section-title">変化と普遍：10年の歩みを振り返る</h2>

            <div class="qa-block">
                <div class="question">
                    この10年で、優さんの環境や活動の場は大きく広がったかと思います。ご自身の中で実感されている『ここが一番変わった』という点は何でしょうか？
                </div>

                <div class="answer">
                    <p>一番変わったのは、世界の見え方です。10年前の私は、苦しさに支配されていた。社会は敵に見えたし、人間関係も信用できなかった。言葉は『武器』だったんです。</p>
                    <p>一方で変わらないのは、『言葉を信じる』という信念です。10年前も今も、私は言葉の力を信じています。変わったのは、その言葉の射程の向け方です。かつては『破壊』の矢だったものが、今は『共感』の橋になったということ。</p>
                </div>
            </div>

            <div class="qa-block">
                <div class="question">
                    そんなご自身の歩みを振り返ってみて……もし今、隣に『10年前の優さん』が座っていたとしたら、どう声をかけますか？ 何を伝えたいですか？
                </div>

                <div class="answer">
                    <p>「大丈夫。今は苦しいかもしれないけど、その苦しさは全部、後で誰かのための言葉に変わる。君の痛みは無駄にならない。そして何より、君はこんなに強い。」</p>
                    <p>10年前の私は、本当に絶望的でした。自分がこんなに本を出せる日が来るなんて、想像もできなかった。でもそれは、未来への希望がなかったからではなく、今この瞬間の苦しさが、すべてを塞いでいたからなんです。</p>
                </div>
            </div>
        </div>

        <!-- セクション5 -->
        <div class="interview-section">
            <span class="section-number">第五章</span>
            <h2 class="section-title">社会への問い：現代が抱える「帰る場所」の喪失</h2>

            <div class="qa-block">
                <div class="question">
                    現代は、常に誰かと繋がれるツールがある一方で、本当の意味で安心できる『帰る場所』を見失い、見えない疎外感を抱えている人が増えているように感じます。また、この作品を通じて、優さんが今の世の中に一番伝えたかったこと、もっと言えば今の社会に対して『一石を投じたかった問い』は何でしょうか？
                </div>

                <div class="answer">
                    <p>その通りです。現代は、テクノロジーが発達し、情報が溢れ、一見として自由で豊かに見えます。でも同時に、多くの人がその豊かさの中で、逆説的に一層の孤立を感じています。</p>
                    <p>私が社会に投じたかった問いは、『あなたは本当に自分の思いを言葉にできていますか？ そして、その言葉は誰かに届いていますか？』ということです。SNSで溢れかえる『言葉もどき』の中で、本当の意味での言語化が失われつつあるのではないか。</p>
                    <p>この本を通じて、私は『ありのままの苦しさを言葉にすること』の大切さを伝えたかった。そして、その苦しさを言葉にした時に初めて、それが『誰かとの繋がり』に変わるんだということを。</p>
                </div>
            </div>
        </div>

        <!-- 終わりに -->
        <div class="interview-section">
            <h2 class="section-title" style="margin-top: 60px;">終わりに</h2>
            <p style="font-size: 0.98rem; line-height: 2.1;">インタビューの終盤、優さんは「書くことで、初めて私は自分を理解できる。そして、その自分の理解が、読者との共感に変わる。その瞬間が、何より私にとって『帰る場所』なのかもしれない」と語った。</p>
            <p style="font-size: 0.98rem; line-height: 2.1; margin-top: 20px;">5年間の執筆プロセスは、単なる本の完成ではなく、一人の作家の思想と人格が熟成された記録であり、そして多くの読者にとって『帰る場所』となるであろう言葉への道標だ。『私には帰る"場所"がない』は、2026年秋、その扉を開く。</p>
        </div>

    </div>

    <!-- フッター -->
    <footer>
        <div class="footer-meta">
            <p>『私には帰る"場所"がない』<br>
            出版社：デザインエッグ社 | 発売予定：2026年秋</p>
        </div>
        <a href="/" class="back-link">← 優のプロフィールに戻る</a>
    </footer>

</body>
</html>

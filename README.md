<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>テトリスシミュレータの使い道紹介？</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700&family=Noto+Sans+JP:wght@400;500;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', 'Noto Sans JP', sans-serif;
            line-height: 1.7;
            margin: 0 auto;
            max-width: 800px;
            padding: 20px;
            background-color: #111827;
            color: #d1d5db;
        }
        h1 { font-size: 2.25em; font-weight: bold; margin-top: 1.5em; margin-bottom: 0.75em; border-bottom: 2px solid #374151; padding-bottom: 0.25em; }
        h2 { font-size: 1.875em; font-weight: bold; margin-top: 1.5em; margin-bottom: 0.75em; border-bottom: 1px solid #374151; padding-bottom: 0.25em; }
        h3 { font-size: 1.5em; font-weight: bold; margin-top: 1.25em; margin-bottom: 0.5em; }
        p { margin-bottom: 1em; }
        b, strong { font-weight: bold; color: #fef08a; }
        img { max-width: 100%; height: auto; border-radius: 0.5rem; margin: 1em 0; box-shadow: 0 4px 6px rgba(0,0,0,0.1); }
        iframe { width: 100%; min-height: 450px; border: 1px solid #4b5563; border-radius: 0.5rem; margin: 1em 0; }
        ul, ol { padding-left: 1.5em; margin-bottom: 1em; }
        a { color: #fde047; text-decoration: underline; }
        .toc { background-color: #1f2937; border: 1px solid #4b5563; border-radius: 0.75rem; padding: 1.5rem; margin-bottom: 2rem; }
        .toc h2 { font-size: 1.25em; font-weight: bold; margin-top: 0; margin-bottom: 1rem; border-bottom: 1px solid #4b5563; padding-bottom: 0.5rem; color: #e5e7eb; }
        .toc ul { list-style-type: none; padding-left: 0; }
        .toc ul ul { padding-left: 1.5rem; margin-top: 0.5rem; }
        .toc a { text-decoration: none; color: #d1d5db; }
        .toc a:hover { text-decoration: underline; color: #ffffff; }
    </style>
</head>
<body>
    <div class="toc"><h2>目次</h2><ul><ul><li><a href="#toc-0-テトリスシミュレータ">テトリスシミュレータの使い道紹介？</a></li><ul><ul><li><a href="#toc-1-特定のパフェパターン">特定のパフェパターンの練習</a></li><li><a href="#toc-2-特定のミノ順での練習">特定のミノ順での練習</a></li></ul><li><a href="#toc-3-謎テト">謎テト</a></li><ul><li><a href="#toc-4-謎テトを実際に操作し">謎テトを実際に操作して考えられる</a></li></ul><li><a href="#toc-5-対戦の研究">対戦の研究</a></li><ul><li><a href="#toc-6-画像認識（汎用）">画像認識（汎用）</a></li><li><a href="#toc-7-画像認識（ぷよテト2">画像認識（ぷよテト2）</a></li></ul><li><a href="#toc-8-記事に用いる">記事に用いる</a></li><ul><li><a href="#toc-9-テンプレを載せている">テンプレを載せているサイトなどで、実際に遊べるようにできる</a></li></ul></ul></ul></div>
    <h1 id="toc-0-テトリスシミュレータ"><span style="font-size: inherit; -webkit-tap-highlight-color: transparent; -webkit-text-size-adjust: 100%;">テトリスシミュレータの使い道紹介？</span></h1><span style="transition-timing-function: ease; background-color: rgba(55, 65, 81, 0.5);">自作テトリスシミュレータの使い道を考えてみた<br><br>↓自作シミュレータ</span><br style="transition-timing-function: ease;"><p style="transition-timing-function: ease;"><a href="https://selmtoe.github.io/Tetris_Simulator/">https://selmtoe.github.io/Tetris_Simulator/</a></p><p></p><h3 id="toc-1-特定のパフェパターン"><span style="background-color: rgba(55, 65, 81, 0.5);">特定のパフェパターンの練習</span></h3>例：はちみつ理想形のパフェ練習<br>組むまでの過程を飛ばして練習できる、セットアップの低い状況下なら有用かも？<br><br><h3 id="toc-2-特定のミノ順での練習"><span style="background-color: rgba(55, 65, 81, 0.5);">特定のミノ順での練習<br></span></h3>
                    <span style="background-color: rgba(55, 65, 81, 0.5);">例：DPC（O残し）の練習<br></span>同じくこれまでの過程を飛ばして練習可能<br><br><h2 id="toc-3-謎テト"><span style="background-color: rgba(55, 65, 81, 0.5);">謎テト</span></h2><h3 id="toc-4-謎テトを実際に操作し"><span style="background-color: rgba(55, 65, 81, 0.5);">謎テトを実際に操作して考えられる</span></h3><p>新しいテキストボックス</p>今後の展望として、クリア条件とかを設定できたら便利かも？<br><h2 id="toc-5-対戦の研究"><span style="background-color: rgba(55, 65, 81, 0.5);">対戦の研究</span></h2><span style="background-color: rgba(55, 65, 81, 0.5);">画像から盤面を認識して、直接取り込める。<br></span>AIではなく機械的なものだが、精度は結構高い<br><h3 id="toc-6-画像認識（汎用）">画像認識（汎用）<br></h3>盤面の左下と右上を指定することで、盤面を読み込める<br><br><h3 id="toc-7-画像認識（ぷよテト2">画像認識（ぷよテト2）</h3>ぷよテト2の2人対戦の画像は特別にネクスト、ホールド、操作ミノを含めて認識可能<br>Youtubeの動画などを、そのままスクショしてload PPTを押せば認識可能（ただし、最大画面であること）<br>この状況からAIを動かしたりできれば、最善手を調べたり、<br><br><h2 id="toc-8-記事に用いる"><span style="background-color: rgba(55, 65, 81, 0.5);">記事に用いる</span></h2><h3 id="toc-9-テンプレを載せている"><span style="background-color: rgba(55, 65, 81, 0.5);">テンプレを載せているサイトなどで、実際に遊べるようにできる</span></h3>体験が増えて面白いかも？<br><br><p>新しいテキストボックス</p>
                <p></p>
</body>
</html>

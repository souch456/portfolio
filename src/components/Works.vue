<template>
    <h2>Works</h2>
    <ul>
        <h3>自然言語処理による教育データ間の類似度計算</h3>
        <p>修士研究で実装．教材データや学生の感想など幅広い教育データのテキストから特徴量を抽出し，コサイン類似度を計算．
            類似度をもとにデータの紐付けをおこなった．特徴量としてTF-IDF，BM25，Sentence BERT，T5などを用いた．
            <br>使用言語：Python，SQL，Cypher</p>
    </ul>
    <ul>
        <h3>Webサイトのスクレイピング</h3>
        <p>インターン課題で実装．食べログサイト「ぐるなび」にて，特定のキーワードで検索した際の
            結果(店名，住所，電話番号など)をBeautifulSoupによりスクレイピングし，その結果を出力．
            <br>使用言語：Python
            <br>環境：Docker
            <br><a href="https://github.com/souch456/Final_Answer">githubリンク</a>
        </p>
    </ul>
    <ul>
        <h3>Amazon Aurora Serverlessのスケーリングに関する調査</h3>
        <p>インターンで取り組んだ．Aurora Serverlessにおける負荷分散の仕組みとして，インスタンスの容量(性能)を負荷に応じて
            自動的に調整するスケーリングと呼ばれる機能がある．それが具体的にどの程度の負荷をトリガーにして行われるのかを様々な負荷テスト
            を通して検証，考察した．
            <br>使用言語：Python
            <br>環境：AWS
        </p>
    </ul>
</template>
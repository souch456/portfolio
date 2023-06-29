<script setup>
import {usePDF, VuePDF} from '@tato30/vue-pdf'
import { ref } from 'vue';
const { pdf, pages, info } = usePDF("research.pdf")

const page = ref(1)

const NextPage = () => {
  page.value += 1;
};
const PrevPage = () => {
  page.value -= 1;
}
</script>

<template>
    <h2>研究紹介</h2>
    <h3>概要</h3>
    <p>近年，教育現場ではさまざまな学習支援システムを通して，学生の学びの過程や教材スライドなどが大規模な教育データとして蓄積されている．これらの教育データ間のつながりを基にした研究として，講義動画や教材スライドといった複数形式の教材推薦やシラバス間の情報を紐付けた履修支援ダッシュボード開発などがあり，関連度による教育データ連携は幅広く行われている．しかしながら，連携の基準が様々であり明確な基準がないことから，それぞれの連携の持つ意味が異なるため，データ連携が限定的であるという問題がある．そこで自身の研究では，多くの教育データが要素として持つ内容に着目して，それぞれのデータを同一の特徴空間で表現しその類似度により連携を行うことで，システム間のデータのつながりに基づく横断的な学習分析を支援することを目的としている．</p>
    <h3>研究スライド</h3>
    <div class="pdf-viewer">
    <VuePDF :pdf="pdf" :page="page" fit-parent />
    </div>
    <button @click="PrevPage">Prev Page</button>
    <button @click="NextPage">Next Page</button>
</template>

<style>
.pdf-viewer {
    width: 100%;
    text-align: center;

}
</style>

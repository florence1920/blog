<template>
    <div class="postWrap">
        <ul class=rPostList>
            <li>
                <p class="title">카카오 AI추천 : 토픽 모델링과 MAB를 이용한 카카오 개인화 추천</p>
                <p class="date">2021.06.05</p>
                <p class="cont"> 글 작성에는 추천팀 sasha.k와 marv.20가 함께해 주셨습니다. 머신러닝에 대한 기초 지식이 있고, 추천 알고리즘에 관심이 있는 분들에게 카카오 추천팀이 개인화 추천 기술을 활용하는 방법에 대해 공유합니다. 우리의 일상 속에는 수많은 추천이 함께합니다. 카카오 추천팀은 카카오가 제공하는 서비스들에서 여러분들이 더 좋은 추천을 경험하실 수 있도록 매일 노력하고 있는데요, 오늘은 수없이 많은 정보 가운데 여러분 한 분 […]</p>
                <div class="imgBG">
                    <img src="@/assets/images/rpImg.png">
                </div>
            </li>

            <li>
                <p class="title">카카오 AI추천 : 토픽 모델링과 MAB를 이용한 카카오 개인화 추천</p>
                <p class="date">2021.06.05</p>
                <p class="cont"> 글 작성에는 추천팀 sasha.k와 marv.20가 함께해 주셨습니다. 머신러닝에 대한 기초 지식이 있고, 추천 알고리즘에 관심이 있는 분들에게 카카오 추천팀이 개인화 추천 기술을 활용하는 방법에 대해 공유합니다. 우리의 일상 속에는 수많은 추천이 함께합니다. 카카오 추천팀은 카카오가 제공하는 서비스들에서 여러분들이 더 좋은 추천을 경험하실 수 있도록 매일 노력하고 있는데요, 오늘은 수없이 많은 정보 가운데 여러분 한 분 […]</p>
                <div class="imgBG">
                    <img src="@/assets/images/rpImg.png">
                </div>
            </li>
        </ul>
        <div class="cateBox"></div>
    </div>
</template>

<script>
export default{
}

</script>

<style scoped>
    .postWrap {position:relative;}
    .postWrap .cateBox {width:275px; height:500px; background: rebeccapurple; position:absolute; top:0; right:0;}
    .postWrap .cateBoxF {position:fixed;}
    .rPostList {padding: 0 294px 0 0;}
    .rPostList li {width:866px; margin: 0 0 16px; padding: 35px 32px 31px; background:#fff;}
    .rPostList li .title {font-weight: 600; font-size: 20px; color: #111; letter-spacing: -1.5px; }
    .rPostList li .date {margin: 10px 0 0;font-size: 14px; color: #aaa;}
    .rPostList li .cont { display: -webkit-box; letter-spacing: -2px; overflow: hidden; margin-top: 15px; font-size: 16px; line-height: 26px; max-height: 78px; -webkit-line-clamp: 3; -webkit-box-orient: vertical; text-overflow: ellipsis;}
    .rPostList li .imgBG {background:#000; margin:30px 0 0;}
    .rPostList li .imgBG img {display:block; width: 100%; opacity: 0.9;}
</style>
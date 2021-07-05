<template>
  <div id="nav">
    <Nav/>
  </div>
  <div id="container" v-on:scroll="scrollFunction">
      <Top/>
      <div class="router-view-wrap">
        <router-view/>
      </div>
  </div>
</template>

<script>
import Nav from "@/components/Nav";
import Top from "@/components/Top";
export default {
  components: {
    Nav,
    Top
  },
  created(){
    window.addEventListener('scroll',this.handleScroll);
  },
  destroyed(){
    window.removeEventListener('scroll',this.handleScroll);
  },
  methods:{
    handleScroll(event){
      let st = document.scrollingElement.scrollTop;
      if(st >= 1300){
        $('.cateBox').css({"position":"fixed","top":"15px","right":"calc((100% - 1160px) / 2)"});
      }else if(st < 1300) {
        $('.cateBox').css({"position":"absolute","top":"0","right":"0"});
      }
    }
  }
}
</script>

<style>
  @import url("assets/css/reset.css");
  #container {min-height: 3000px; background: #F1F2F4;}
  #container .section_featured {padding: 84px calc((100% - 1160px)/2) 130px;}
  #container .section_featured .tit {height: 51px; line-height: 51px; font-size:34px; font-weight: 500; margin: 0 0 13px;}
</style>

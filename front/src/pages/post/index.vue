<template>
    <div class="section_featured">        
        <div class="post">
            <div class="inner">
                <p class="tit">Featured Posts</p>
                <SwiperFeatured/>
            </div>
            <div class="inner">
                <p class="tit">Related Posts</p>
                <RPosts/>
            </div>
        </div>
    </div>
</template>

<script>
import Top from "@/components/Top"
import SwiperFeatured from '@/components/SwiperFeatured.vue'
import RPosts from '@/components/RPosts.vue'
export default {
    components: {
        Top,
        SwiperFeatured,
        RPosts
    }
}
    
</script>

<style scoped>
    .section_featured .inner {margin: 0 0 83px;}
    
</style>
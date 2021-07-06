<template>
    <div id="footer">
        <ul class="contact">
            <li>
                <p class="tit">Contact with LeeSeungHeon</p>
                <div class="depth">
                    <div title="copy" class="mailWrap" :class="{active:hover}" @mouseover="hover = true" @mouseleave="hover = false">
                        <p id="info">jetaime12121@gmail.com</p>
                        <button v-on:click="copyText"><img src="@/assets/images/copy.png"/></button>
                    </div>
                </div>
            </li>
            <li>
                <p class="tit">About Project</p>
                <ul class="depth">
                    <li><a href="">Filo</a></li>
                    <li><a href="">Filo Game</a></li>
                    <li><a href="">TravelMaker</a></li>
                </ul>
            </li>
            <li>
                <p class="tit">About Channel</p>
                <ul class="depth">
                    <li><a href="">Blog GitHub</a></li>
                    <li><a href="">Filo GitHub</a></li>
                </ul>
            </li>
        </ul>
        <p class="copyR">Copyright © LSH. All rights reserved.</p>
    </div>
</template>


<script>
    export default {
        data(){
            return {
                hover:false
            }
        },
        methods:{
            copyText: function copyText(){
                //임시로 textarea 생성
                let tempElem = document.createElement('textarea');
                tempElem.value = 'jetaime12121@gmail.com';
                document.body.appendChild(tempElem);
                //요소 선택
                tempElem.select();
                document.execCommand("copy");
                document.body.removeChild(tempElem);

                alert('copied');
            },
            turnOn: function turnOn(){
                let email = document.querySelector('.info');
                email.style
            }
            
        }
    }
</script>


<style scoped>
    #footer .contact {overflow: hidden;}
    #footer .contact > li {float: left; width: 400px; height: 260px; padding: 28px 40px;}
    #footer .contact > li:nth-child(1) {width: calc(100% - 800px); background: #031461; padding: 28px 32px;}
    #footer .contact > li:nth-child(2) {background: #020D41;}
    #footer .contact > li:nth-child(3) {background: #01092B;}
    #footer .contact > li .tit {color:#fff; font-size:26px; font-weight: 500;}
    #footer .contact > li .depth {margin: 30px 0 0;}
    #footer .contact > li .depth .mailWrap {overflow: hidden;}
    #footer .contact > li .depth .mailWrap #info{float: left;}
    #footer .contact > li .depth .mailWrap img {float: left; width: 25px; margin: 0 0 0 20px;}
    #footer .contact > li .depth .mailWrap button {background:none; cursor: pointer;}
    #footer .contact > li .depth #info {line-height: 35px; color:rgba(255,255,255,.5); font-size: 16px; font-weight: 600;}
    #footer .contact > li .depth .active #info {color:#fff;}
    #footer .contact > li .depth > li > a {line-height: 35px; color:rgba(255,255,255,.5); font-size: 16px; font-weight: 600;}
    #footer .contact > li .depth > li > a:hover {color:#fff;}
    #footer .copyR {height: 70px; background: #000; line-height: 70px; color:rgba(255,255,255,.5); font-size:13px; font-weight: 600; padding: 0 32px;}
</style>
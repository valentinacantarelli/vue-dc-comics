<template>
    <header>
        <div class="container">
            <img src="../assets/img/dc-logo.png" alt="Logo Dc">
            <ul>
                <li v-for="(link, index) in menu" :key="index">
                    <a :href="link.url" :class="{ active : link.current }">{{link.text}}</a>
                </li>
            </ul>
        </div>
    </header>
    
</template>

<script>
export default {
    name:"Header",
    data(){
        return {
			menu: [
                {
                    text: "CHARACTERS",
                    url: "#",
                    current: false,
                },
                {
                    text: "COMICS",
                    url: "#",
                    current: true,
                },
                 {
                    text: "MOVIES",
                    url: "#",
                    current: false,
                },
                 {
                    text: "TV",
                    url: "#",
                    current: false,
                },
                 {
                    text: "GAMES",
                    url: "#",
                    current: false,
                },
                {
                    text: "COLLECTIBLES",
                    url: "#",
                    current: false,
                },
                 {
                    text: "VIDEOS",
                    url: "#",
                    current: false,
                },
                 {
                    text: "FANS",
                    url: "#",
                    current: false,
                },
                 {
                    text: "NEWS",
                    url: "#",
                    current: false,
                },
                {
                    text: "SHOP",
                    url: "#",
                    current: false,
                },
            ],
		}
    }
}
</script>

<style lang="scss" scope>
@import "../assets/style/variables";
@mixin larghezza{
    width:65%;
    margin:auto;
}
header{
    width:100%;
    height:95px;
    
    
}
.container{
    display: flex;
    justify-content: space-between;
    @include larghezza;
    
    img{
        margin-top:20px;
        height: 60px;
    }
    ul{
        display:flex;        
        
        li{
            list-style: none;
             padding:40px 13px;          
            font-size: 13px;

            a{
                text-decoration: none;
                color:black;
                font-weight: bold;
                border-bottom: 3px solid transparent; 
                
                &:hover{
                    border-bottom:3px solid $defaultColor;
                    padding:35px 0;
                    color:$defaultColor;
                }
            }
        }
    }
}
</style>
<template>
    <div class="container">
        <img src="../assets/img/dc-logo.png" alt="Logo Dc">
        <ul>
            <li v-for="(link, index) in menu" :key="index">
                <a :href="link.url" :class="{ active : link.current }">{{link.text}}</a>
            </li>
        </ul>
    </div>
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
@import "src/assets/style/variables";
.container{
    width:1000px;
    margin:auto;
    display: flex;
    justify-content: space-between;

    img{
        margin-top:20px;
        height: 60px;
    }
    ul{
        display:flex;
        vertical-align: middle;
        padding:40px 0;

        li{
            list-style: none;
             padding:0 13px;          
            font-size: 13px;

            a{
                text-decoration: none;
                color:black;
                font-weight: bold;
                padding:35px 0; 
                
                &.active{
                    border-bottom:3px solid #0282f9;
                    color:#0282f9;
                }
            }
        }
    }
}
</style>
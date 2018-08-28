<template lang="pug">
.Content
    .HeaderNav
        h2 GREEN.
    #nav.nav
        ul
            li.home HOME
            li.about ABOUT
            li.gallery GALLERY
            li.contact CONTACT
    .hamburger(v-on:click="Menu()")
        a.icon 
        a.icon1
        a.icon2
</template>
<script>
export default {
    methods:{
        Menu: function(){
            var x = document.getElementById("nav")
            if(x.className === "nav"){
                x.className += "responsive"
            }else{
                x.className = "nav"
            }
        }
    }
}

</script>
<style lang="sass" scoped>

$green: #B2D430 

.Content
    padding: 3rem 
    display: flex
    .HeaderNav
        h2
            color: $green                   
    .nav
        margin-left: auto
        ul
            list-style-type: none
            display: flex
            li 
                margin-left: 20px
                border-bottom: 2px solid #B2D430
                padding: 8px 0
                letter-spacing: 0.2rem
    .hamburger
            display: flex
            display: none
            flex-direction: column
            a.icon, a.icon1, a.icon2
                float: right
                display: block
                color: $green 
                width: 20px
                height: 3px
                background-color: black
                margin: 3px 0  
@media (max-width: 590px)    
    .Content
        .HeaderNav
        .nav
            ul
                display: none
        .hamburger
            display: flex
            
@media (max-width: 590px)  
    .Content
        .hamburger
            position: absolute
            top: 3rem
            right: 2rem
            a.icon, a.icon1, a.icon2
                background-color: #EEE
        .navresponsive
            ul
                list-style-type: none
                font-size: 14px
                font-weight: 400
                position: absolute
                top: 0
                right: 0
                width: 40%
                height: 100%
                padding: 5rem
                background: black 
                li
                    margin-top: 0.9rem
                    color: white


</style>

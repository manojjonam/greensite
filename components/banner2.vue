<template lang="pug">
.Banner
    .title 
        h2 FRESH & NON-GMO PRODUCTS
    .sub-title
        p Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.
</template>
<script>
export default {
    
}
</script>
<style lang="sass" scoped>
.Banner
    height: 25rem
    padding: 5%
    background: url("https://uicookies.com/demo/theme/green/img/slider_2.jpg")
    background-attachment: fixed
    background-size: cover
    @media (max-width:700px)
        height: 45%
    .title
        h2
            margin-top: 2rem
            color: #EEE
            font-family: "Just Another Hand",cursive
            font-size: 4rem
            text-align: center
            text-transform: uppercase
            
    .sub-title
        p
            text-align: center
            margin-bottom: 2rem
            opacity: 0.5
            font-size: 1.5rem       

</style>

<template>
<div class="mouse_cont">
 <p>Scroll Down/ Click above button to scroll</p>

    <span class="mouse">
       
        <span class="mouse-wheel"></span>
    </span>
</div>

</template>
<style scoped>
/* SMAL DEVICES */
@media only screen and (max-width: 768px) and (min-width: 280px) {
.mouse_cont p{
    color: var(--light-text);
}
.mouse_cont{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}
.mouse{
    width:25px;
    height: 50px;
    border:2px solid #f8f8f8;
    border-radius: 20px;
    display: flex;
}
.mouse-wheel{
    display: block;
    width: 10px;
    height:10px;
    background:#f3f3f3;
    border-radius:50%;
    margin:auto;
    animation: move-wheel 1s linear infinite;
}
@keyframes move-wheel{
    0%{
        opacity:0;
        transform: translateY(-1rem);
    }
    100%{
        opacity:1;
        transform: translateY(1rem);
    }
}}
/* SMAL DEVICES */
@media only screen and  (min-width: 769px) {
.mouse_cont{
    /* opacity: 0; */
    display: none;
}
}
</style>
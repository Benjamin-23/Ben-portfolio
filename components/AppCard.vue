<template>
<div class="mb-4 transition ease-in-out delay-100 hover:scale-105 hover:animate-pulse">  
    <div class="card ">
        <div class="smallCard  flex items-center">
            <slot></slot>
        </div>
    </div>
</div>
</template>
<style scoped>
.topCard{
    background: #4F228D;
    border-radius: 15px;
}
.smallCard {
    background: linear-gradient(110.49deg, #130428 19.95%, #251043 67.64%, #38126D 107.08%, #261045 156.61%, #190634 183.21%);
    box-shadow: 8px 7px 26px rgba(0, 0, 0, 0.12);
    border-radius: 15px;
}
.card{ 
background: #2c1250;
box-shadow: 4px 7px 26px rgba(0, 0, 0, 0.12);
border-radius: 15px;
z-index: 10;
}
</style>
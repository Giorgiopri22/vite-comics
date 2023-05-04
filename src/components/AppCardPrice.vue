<script>


export default {
    props: {
        image: {
            type: String,
            required: true
        },
        text: {
            type: String,
            required: true
        }
    }
}

</script>

<template>
    
    <div class="list-item-buy">
        <img :src="image" alt="">
        {{ text }}
    </div>

</template>

<style lang="scss" scoped> 

.list-item-buy {
    display: flex;
    align-items: center;
    gap: 15px;
    text-transform: uppercase;

    img {
        height: 50px;
    }
}
 
</style>
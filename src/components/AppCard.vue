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

    <div class="card">
        <figure>
            <img :src="image" alt="">
        </figure>
        <div class="text-card">
            {{ text }}
        </div>
    </div>

</template>

<style lang="scss" scoped> 

.card{

    img{
        width: 180px;
        aspect-ratio: 1;
        object-fit: cover;
        object-position: center;
        margin-bottom: 18px;
    }

    .text-card{
        text-transform: uppercase;
    }
}
 
</style>
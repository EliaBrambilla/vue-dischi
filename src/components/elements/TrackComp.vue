<template>
    <div class="card bg-element">
        <div class="img-title">
            <img :src="album.poster" alt="">
            <h3>{{album.title}}</h3>
        </div>
        <div class="details">
            <h5>{{album.author}}</h5>
            <h5>{{album.year}}</h5>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'TrackComp',
        props: {
            album: Object
        }
    }
</script>

<style lang="scss" scoped>
    .card{
        width: calc( 100% / 5 - (3%));
        height: 300px;
        margin-bottom: 20px;
        padding: 10px;
        color: white;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        img{
            width: 100%;
        }
        .details{
            opacity: 0.5;
            margin-bottom: 5px;
        }
    }
</style>
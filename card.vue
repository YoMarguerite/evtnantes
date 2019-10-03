<template>
    <a :href="event.fields.lieu_siteweb">
        <img :id="event.recordid" class="card-img-top" :src="event.fields.media_1" :alt="event.fields.description">
        <b-popover :target="event.recordid" triggers="hover" placement="top">
            {{ event.fields.description }}
        </b-popover>
    </a>
    <div class="card-body">
        <h5 class="card-title">{{ event.fields.nom }}</h5>
    </div>
</template>
<script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>
<script>
var demo = new Vue({
    props:{
        event:{}
    }
})
</script>

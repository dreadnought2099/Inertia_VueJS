<script>
export default {
    props: {
        films: Array,
    },
    data() {
        return {
            name: "RMAGALLANEZ",
        };
    },
};
</script>

<template>
    <h1 class="text-3xl">Welcome to Oasis!</h1>
    <div class="card"></div>

    <div class="card-body">
        <p class="text-lg">Hello my name is {{ name }}.</p>
        <input type="text" v-model="name" />
    </div>

    <ul>
        <li v-for="film in films" :key="film"></li>
        {{
            film
        }}
    </ul>
</template>

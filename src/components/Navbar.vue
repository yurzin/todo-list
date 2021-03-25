<template>
    <nav class="blue darken-3">
        <div class="nav-wrapper">
            <router-link to="/" class="brand-logo">Todo List</router-link>
            <ul class="right hide-on-med-and-down">
                <router-link
                        to="/"
                        exact
                        active-class="active"
                        custom v-slot="{navigate}"
                >
                    <li @click="navigate">Create</li>
                </router-link>
                <router-link
                        to="/list"
                        active-class="active"
                        custom v-slot="{navigate}"
                >
                    <li @click="navigate">List</li>
                </router-link>
            </ul>
        </div>
    </nav>
</template>

<script>
    export default {}
</script>

<style lang="scss" scoped>
    nav {
        padding: 0 2rem;
    }

    li {
        cursor: pointer;
        margin: 0 2rem;
    }
</style>
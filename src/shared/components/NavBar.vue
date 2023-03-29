<script setup lang="ts">

    /* const props = defineProps({
        title: {
            type: string,
            required: true
        }
    }); */
    // const props = defineProps<{ title?: string }>();

    interface Props {
        title: string
    }

    const props = defineProps<Props>();

</script>

<template>
    <nav>
        <img src="@/assets/logo.svg" alt="Vue logo" height="25" width="25">
        <span>{{ props.title || 'No title' }}</span>

        <RouterLink to="/" >Inicio</RouterLink>
        <RouterLink to="/about" >Acerca de</RouterLink>
    </nav>
</template>

<style scoped>

    nav {
        align-items: flex-start;
        display: flex;
        font-size: 12px;
        margin-top: 10px;
        text-align: center;
        width: 100%;
    };

    img {
        margin-right: 5px;
    }

    span {
        margin-right: 10px;
    }

    a {
        margin-right: 5px;
    }

</style>
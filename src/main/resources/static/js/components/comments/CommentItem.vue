<template>
    <v-list-item>
        <user-link
            :user="comment.author"
        ></user-link>
        <v-list-item-content>
            <v-list-item-title v-html="comment.text"></v-list-item-title>
        </v-list-item-content>
    </v-list-item>
</template>

<script>
    import UserLink from "../profile/UserLink.vue";
    export default {
        name: "CommentItem",
        components: {UserLink},
        props: ["comment"]
    }
</script>

<style scoped>

</style>
<template>
    <ul class="list_style">
        <TreeViewItem
            v-for="(childItem, index) in items"
            :key="index"
            :item="childItem"
        >
        </TreeViewItem>
    </ul>
</template>

<script>
import TreeViewItem from "@/components/TreeViewItem";

export default {
    name: "TreeView",
    components: {
        TreeViewItem
    },
    props: {
        items: Array
    },
    data: function () {
        return {

        }
    }
}
</script>

<style scoped>
    .list_style li {
        list-style-type: none;
    }
</style>
<template>
    <li class="list_style">
        <img src="@/assets/folder.svg" alt="">
        <img src="@/assets/person.svg" alt="">
        <a class=""
           data-toggle="collapse"
           :href="'#' + randomDataToggleId"
           role="button"
           aria-expanded="false"
           :aria-controls="randomDataToggleId"
           v-on:click="itemClickHandler">
            {{ item.text }}
        </a>
        <div v-if="item.items.length > 0" class="collapse" :id="randomDataToggleId">
            <ul>
                <TreeViewItem
                    v-for="(childItem, index) in item.items"
                    :key="index"
                    :item="childItem"
                >
                </TreeViewItem>
            </ul>
        </div>
    </li>
</template>

<script>

export default {
    name: "TreeViewItem",
    props: {
        item: {
            type: Object,
            default: function () {
                return {
                    value: "something",
                    text: "some text",
                    items: []
                }
            }
        }
    },
    data: function () {
        return {
            randomDataToggleId: null
        }
    },
    mounted() {
        this.randomDataToggleId = 'collapse' + Math.floor(Math.random() * Math.floor(1000));
    },
    methods: {
        itemClickHandler() {
            this.$emit('on-items-click', this.item);
        }
    }
}
</script>

<style scoped>
    .list_style li {
        list-style-type: none;
    }
</style>
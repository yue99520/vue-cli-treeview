<template>
    <div id="app">
        <TreeView
            :items="items"
        >
        </TreeView>
        <button v-on:click="onButtonClick">改變資料</button>
    </div>
</template>

<script>


import TreeView from "@/components/TreeView";
export default {
    name: 'App',
    components: {
        TreeView
    },
    data: function () {
        return {
            items: [
                {
                    value: "something",
                    text: "some text",
                    items: []
                },
                {
                    value: "something",
                    text: "some text",
                    items: [
                        {
                            value: "something",
                            text: "some text",
                            items: [
                                {
                                    value: "something",
                                    text: "some text",
                                    items: [

                                    ]
                                },
                                {
                                    value: "something",
                                    text: "some text",
                                    items: [

                                    ]
                                },
                                {
                                    value: "something",
                                    text: "some text",
                                    items: [

                                    ]
                                }
                            ]
                        },
                        {
                            value: "something",
                            text: "some text",
                            items: [

                            ]
                        },
                        {
                            value: "something",
                            text: "some text",
                            items: [

                            ]
                        },
                        {
                            value: "something",
                            text: "some text",
                            items: [

                            ]
                        }
                    ]
                },
                {
                    value: "something",
                    text: "some text",
                    items: [
                        {
                            value: "something",
                            text: "some text",
                            items: [
                                {
                                    value: "something",
                                    text: "some text",
                                    items: [

                                    ]
                                },
                                {
                                    value: "something",
                                    text: "some text",
                                    items: [

                                    ]
                                },
                                {
                                    value: "something",
                                    text: "some text",
                                    items: [

                                    ]
                                }
                            ]
                        },
                        {
                            value: "something",
                            text: "some text",
                            items: [

                            ]
                        },
                        {
                            value: "something",
                            text: "some text",
                            items: [

                            ]
                        },
                        {
                            value: "something",
                            text: "some text",
                            items: [

                            ]
                        }
                    ]
                },
                {
                    value: "something",
                    text: "some text",
                    items: [
                        {
                            value: "something",
                            text: "some text",
                            items: [
                                {
                                    value: "something",
                                    text: "some text",
                                    items: [

                                    ]
                                },
                                {
                                    value: "something",
                                    text: "some text",
                                    items: [

                                    ]
                                },
                                {
                                    value: "something",
                                    text: "some text",
                                    items: [

                                    ]
                                }
                            ]
                        },
                        {
                            value: "something",
                            text: "some text",
                            items: [

                            ]
                        },
                        {
                            value: "something",
                            text: "some text",
                            items: [

                            ]
                        },
                        {
                            value: "something",
                            text: "some text",
                            items: [

                            ]
                        }
                    ]
                },
                {
                    value: "something",
                    text: "some text",
                    items: [
                        {
                            value: "something",
                            text: "some text",
                            items: [
                                {
                                    value: "something",
                                    text: "some text",
                                    items: [

                                    ]
                                },
                                {
                                    value: "something",
                                    text: "some text",
                                    items: [

                                    ]
                                },
                                {
                                    value: "something",
                                    text: "some text",
                                    items: [

                                    ]
                                }
                            ]
                        },
                        {
                            value: "something",
                            text: "some text",
                            items: [

                            ]
                        },
                        {
                            value: "something",
                            text: "some text",
                            items: [

                            ]
                        },
                        {
                            value: "something",
                            text: "some text",
                            items: [

                            ]
                        }
                    ]
                },
                {
                    value: "something",
                    text: "some text",
                    items: [
                        {
                            value: "something",
                            text: "some text",
                            items: [
                                {
                                    value: "something",
                                    text: "some text",
                                    items: [

                                    ]
                                },
                                {
                                    value: "something",
                                    text: "some text",
                                    items: [

                                    ]
                                },
                                {
                                    value: "something",
                                    text: "some text",
                                    items: [

                                    ]
                                }
                            ]
                        },
                        {
                            value: "something",
                            text: "some text",
                            items: [

                            ]
                        },
                        {
                            value: "something",
                            text: "some text",
                            items: [

                            ]
                        },
                        {
                            value: "something",
                            text: "some text",
                            items: [

                            ]
                        }
                    ]
                },
            ],
            temp: true,
        }
    },
    methods: {
        onButtonClick() {
            let pend = [
                {
                    value: "something",
                    text: "some text",
                    items: [
                        {
                            value: "something",
                            text: "some text",
                            items: [

                            ]
                        },
                        {
                            value: "something",
                            text: "some text",
                            items: [

                            ]
                        },
                        {
                            value: "something",
                            text: "some text",
                            items: [

                            ]
                        }
                    ]
                },
                {
                    value: "something",
                    text: "some text",
                    items: [

                    ]
                },
                {
                    value: "something",
                    text: "some text",
                    items: [

                    ]
                },
                {
                    value: "something",
                    text: "some text",
                    items: [

                    ]
                }
            ];
            if (this.temp) {
                this.items[0].items = pend;
            } else {
                this.items[0].items = [];
            }
            this.temp = !this.temp;
        }
    }
}
</script>

<style>

</style>

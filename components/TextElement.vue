<template>
  <div :class="classAttributes" :style="cssAttributes">
    <div v-html="content"></div>
  </div>
</template>

<script>
    export default {
        props: {
            classAttributes: {
                type: Array,
                default: function () {
                    return []
                }
            },
            cssAttributes: {
                type: Object,
                default() {},
            },
            content: {
                type: String,
                default: ''
            }
        },
        data() {
            return {
            }
        }
    }
</script>

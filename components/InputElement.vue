<template>
  <div :class="classAttributes" :style="cssAttributes">
    <input class="form-control" v-model="value" :aria-placeholder="placeHolder" />
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
            placeHolder: {
                type: String,
                default: ''
            },
            value: {
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

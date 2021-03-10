<template>
  <div>
    <template v-if="headingSize === 'h1'" :class="classAttributes" :style="cssAttributes">
      <h1 v-html="content"></h1>
    </template>
    <template v-if="headingSize === 'h2'" :class="classAttributes" :style="cssAttributes">
      <h2 v-html="content"></h2>
    </template>
    <template v-if="headingSize === 'h3'" :class="classAttributes" :style="cssAttributes">
      <h3 v-html="content"></h3>
    </template>
    <template v-if="headingSize === 'h4'" :class="classAttributes" :style="cssAttributes">
      <h4 v-html="content"></h4>
    </template>
    <template v-if="headingSize === 'h5'" :class="classAttributes" :style="cssAttributes">
      <h5 v-html="content"></h5>
    </template>
    <template v-if="headingSize === 'h6'" :class="classAttributes" :style="cssAttributes">
      <h6 v-html="content"></h6>
    </template>
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
            },
            headingSize: {
                type: String,
                default: 'h1'
            }
        },
        data() {
            return {
            }
        }
    }
</script>

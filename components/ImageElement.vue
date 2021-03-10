<template>
  <div :class="classAttributes"  :style="cssAttributes">
    <a :href="href" :target="target" >
      <img :src="src" :alt="alt" />
    </a>
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
            src: {
                type: String,
                default: ''
            },
            alt: {
                type: String,
                default: ''
            },
            href: {
                type: String,
                default: ''
            },
            target: {
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

<style>
  img {
    width: 100%;
  }
</style>

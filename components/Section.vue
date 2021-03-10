<template>
  <div :class="classAttributes" :style="cssAttributes">
    <template v-for="child in children">
      <Section v-if="child.type === 'section'" :classAttributes="child.classAttributes" :style="child.cssAttributes" :children="child.children" />
      <template v-else-if="child.type === 'text'">
        <TextElement :classAttributes="child.classAttributes" :style="child.cssAttributes" :content="child.content" />
      </template>
      <template v-else-if="child.type === 'heading'">
        <HeadingElement :classAttributes="child.classAttributes" :style="child.cssAttributes" :content="child.content" :headingSize="child.headingSize" />
      </template>
      <template v-else-if="child.type === 'button'">
        <ButtonElement :classAttributes="child.classAttributes" :style="child.cssAttributes" :content="child.content" />
      </template>
      <template v-else-if="child.type === 'image'">
        <ImageElement :classAttributes="child.classAttributes" :style="child.cssAttributes" :src="child.src" :alt="child.alt" :href="child.href" :target="child.target" />
      </template>
      <template v-else-if="child.type === 'input'">
        <InputElement :classAttributes="child.classAttributes" :style="child.cssAttributes" :placeHolder="child.placeHolder" />
      </template>
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
            children: {
                type: Array,
                default: function () {
                    return []
                }
            }
        },
        data() {
            return {
            }
        }
    }
</script>

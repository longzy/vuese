<template>
  <div></div>
</template>

<script lang="ts">
@Component
export default class Child extends Vue {
  // Description of prop
  @Prop(Number)
  a: number

  @Prop([Number, String])
  b: number | string

  @Prop({
    type: Number,
    // The default value is 1
    default: 1,
    required: true
  })
  c: number
}
</script>

<script>
export default {
  name: "MainBlock",
  props: {
    title: String,
  },
};
</script>

<template>
    <section class="main-block">
      <div class="main-block__container">
        <div class="main-block__header">
            <div class="main-block__title">
                {{ title }}
            </div>
            <slot name="header-button"></slot> 
        </div>
        <div class="main-block__elements">
          <slot name="elements"></slot>
          <slot name="empty-state"></slot>
        </div>
        <slot name="footer-button"></slot>
      </div>
    </section>
  </template>

  
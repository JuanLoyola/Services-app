<template>
  <div class="content">
    <h1 class="content__title">Lorem, ipsum dolor.
    </h1>
    <FAQQuestion
      question="Lorem ipsum dolor sit amet?"
      answer="Lorem ipsum dolor sit amet consectetur adipisicing elit. Error, vero."
    />

    <FAQQuestion
      question="Lorem ipsum dolor sit amet?"
      answer="Lorem ipsum dolor sit amet consectetur adipisicing elit. Error, vero."
    />

    <FAQQuestion
      question="Lorem ipsum dolor sit amet?"
      answer="Lorem ipsum dolor sit amet consectetur adipisicing elit. Error, vero."
    />

    <FAQQuestion
      question="Lorem ipsum dolor sit amet?"
      answer="Lorem ipsum dolor sit amet consectetur adipisicing elit. Error, vero."
    />

    <FAQQuestion
      question="Lorem ipsum dolor sit amet?"
      answer="Lorem ipsum dolor sit amet consectetur adipisicing elit. Error, vero."
    />
  </div>
</template>

<script>
import FAQQuestion from '@/components/FAQQuestion'

export default {
  name: 'TheFaq',

  components: {
    FAQQuestion
  },

  data () {
    return {
      show: false
    }
  }
}
</script>

<style lang="scss" scoped>
.content {
  height: 400px;
  background-color: #ffffff;
  display: flex;
  flex-flow: column nowrap;
  align-items: center;

  &__title {
    font-size: 1.3rem;
    margin-top: 18px;
    margin-bottom: 40px;
  }
}
</style>

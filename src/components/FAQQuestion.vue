<template>
<div>
  <div class="section">
    <div
      class="question"
      @click="toggleAnswer(showAnswer)"
    >
      <h1 class="question__title">{{ question }}</h1>
      <BaseIcon
        v-if="showAnswer"
        class="question__icon"
        name="minus"
        color="black"
      />
      <i
      v-if="showAnswer"
      class="question__icon fas fa-minus"
      ></i>

      <i
      v-else
      class="question__icon fas fa-plus"
      ></i>
    </div>
    <p
      v-if="showAnswer"
      class="answer"
    >
      {{ answer }}
    </p>
  </div>
</div>
</template>

<script>
export default {
  name: 'FAQQuestion',

  props: {
    question: {
      type: String
    },

    answer: {
      type: String
    }
  },

  data () {
    return {
      showAnswer: false
    }
  },

  methods: {
    toggleAnswer (showAnswer) {
      this.showAnswer = !showAnswer
    }
  }
}
</script>

<style lang="scss" scoped>
.section {
  width: 1300px;
  height: auto;
  display: flex;
  flex-flow: column nowrap;
  box-shadow: inset 0px -1px 0px #000000;
}

.question {
  width: 100%;
  height: 56px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  cursor: pointer;

  &__title {
    font-size: 1.3rem;
  }

  &__icon {
    margin-right: 16px;
  }
}

.answer {
  font-size: 1rem;
  color: #A59A98;
  width: 1284px;
  max-height: 96px;
  margin-bottom: 24px;
  display: flex;
}

@media (min-width: 320px) and (max-width: 1024px) {
  .section {
    width: 100%;
    height: auto;
    display: flex;
    flex-flow: column nowrap;
    box-shadow: inset 0px -1px 0px #000000;
  }
  .question {
    max-width: 100%;
    height: 56px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    cursor: pointer;

    &__title {
      font-size: 1rem;
      margin-right: 20px;
    }

    &__icon {
      margin-right: 16px;
    }
  }

  .answer {
    font-size: 0.8rem;
    text-align: start;
    color: #A59A98;
    max-width: 290px;
    max-height: 96px;
    margin-bottom: 24px;
    display: flex;
  }
}
</style>

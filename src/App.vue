<script setup>
import {ref} from "vue";
import Card from "primevue/card"
import FlipCard from "./components/FlipCard.vue"

let cardVar = ref(
    [
      { show: false },
      { show: false },
      { show: false },
      { show: false },
      { show: false },
      { show: false },
      { show: false },
      { show: false }
    ]
);

</script>

<template>
  <div class="grid">
    <FlipCard :show="cardVar[0]" @click="cardVar[0] = !cardVar[0]">
      <template #front>
        <Card class="fill">
          <template #content>
            <h2> Card Front </h2>
          </template>
        </Card>
      </template>

      <template #back>
        <Card class="fill">
          <template #title>Card Back</template>
          <template #content>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur non dictum orci. Aenean et aliquet orci. Nunc tristique orci tortor.
          </template>
        </Card>
      </template>
    </FlipCard>
    <FlipCard :show="cardVar[1]" @click="cardVar[1] = !cardVar[1]">
      <template #front>
        <Card class="fill">
          <template #content>
            <h2> Card Front </h2>
          </template>
        </Card>
      </template>

      <template #back>
        <Card class="fill">
          <template #title>Card Back</template>
          <template #content>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur non dictum orci. Aenean et aliquet orci. Nunc tristique orci tortor.
          </template>
        </Card>
      </template>
    </FlipCard>
    <FlipCard :show="cardVar[2]" @click="cardVar[2] = !cardVar[2]">
      <template #front>
        <Card class="fill">
          <template #content>
            <h2> Card Front </h2>
          </template>
        </Card>
      </template>

      <template #back>
        <Card class="fill">
          <template #title>Card Back</template>
          <template #content>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur non dictum orci. Aenean et aliquet orci. Nunc tristique orci tortor.
          </template>
        </Card>
      </template>
    </FlipCard>
    <FlipCard :show="cardVar[3]" @click="cardVar[3] = !cardVar[3]">
      <template #front>
        <Card class="fill">
          <template #content>
            <h2> Card Front </h2>
          </template>
        </Card>
      </template>

      <template #back>
        <Card class="fill">
          <template #title>Card Back</template>
          <template #content>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur non dictum orci. Aenean et aliquet orci. Nunc tristique orci tortor.
          </template>
        </Card>
      </template>
    </FlipCard>
  </div>

  <div class="grid">
    <FlipCard :show="cardVar[4]" @click="cardVar[4] = !cardVar[4]">
      <template #front>
        <Card class="fill">
          <template #content>
            <h2> Card Front </h2>
          </template>
        </Card>
      </template>

      <template #back>
        <Card class="fill">
          <template #title>Card Back</template>
          <template #content>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur non dictum orci. Aenean et aliquet orci. Nunc tristique orci tortor.
          </template>
        </Card>
      </template>
    </FlipCard>
    <FlipCard :show="cardVar[5]" @click="cardVar[5] = !cardVar[5]">
      <template #front>
        <Card class="fill">
          <template #content>
            <h2> Card Front </h2>
          </template>
        </Card>
      </template>

      <template #back>
        <Card class="fill">
          <template #title>Card Back</template>
          <template #content>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur non dictum orci. Aenean et aliquet orci. Nunc tristique orci tortor.
          </template>
        </Card>
      </template>
    </FlipCard>
    <FlipCard :show="cardVar[6]" @click="cardVar[6] = !cardVar[6]">
      <template #front>
        <Card class="fill">
          <template #content>
            <h2> Card Front </h2>
          </template>
        </Card>
      </template>

      <template #back>
        <Card class="fill">
          <template #title>Card Back</template>
          <template #content>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur non dictum orci. Aenean et aliquet orci. Nunc tristique orci tortor.
          </template>
        </Card>
      </template>
    </FlipCard>
    <FlipCard :show="cardVar[7]" @click="cardVar[7] = !cardVar[7]">
      <template #front>
        <Card class="fill">
          <template #content>
            <h2> Card Front </h2>
          </template>
        </Card>
      </template>

      <template #back>
        <Card class="fill">
          <template #title>Card Back</template>
          <template #content>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur non dictum orci. Aenean et aliquet orci. Nunc tristique orci tortor.
          </template>
        </Card>
      </template>
    </FlipCard>
  </div>
</template>

<style scoped>

.grid {
  display : inline-flex;
}

.fill {
  position: absolute;
  width: 100%;
  height: 100%;
}
</style>

<template>
  <v-container>
    <div>
      {{ $t('message') }}
      <br />

      <select v-model="$i18n.locale">
        <option v-for="(lang, i) in langs" :key="`Lang${i}`" :value="lang">{{ lang }}</option>
      </select>

    </div>
  </v-container>
</template>

<script>
export default {
  name: 'HelloWorld',

  data: () => ({
    langs: ['en', 'ko', 'ru']
  })
}
</script>

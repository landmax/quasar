<template>
  <div class="q-pa-md">
    <q-input filled v-model="input" mask="date" :rules="['date']">
      <q-icon slot="append" name="event" class="cursor-pointer">
        <q-popup-proxy :breakpoint="600">
          <q-date v-model="input" filled />
        </q-popup-proxy>
      </q-icon>
    </q-input>
  </div>
</template>

<script>
export default {
  data () {
    return {
      input: '',
      date: '2018/11/03'
    }
  }
}
</script>

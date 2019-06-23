<template>
  <v-card style="width: 100%;">
    <v-toolbar
      color="indigo"
      dark
      dense
    >
      <v-toolbar-title>Add new debt</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-icon>send</v-icon>
    </v-toolbar>
    <v-form>
      <v-autocomplete
        v-model="selected"
        :items="['John Kowalski', 'Adam Johnes', 'Ian Goodmore', 'Fahrad Agron']"
        chips
        label="Who?"
        full-width
        hide-details
        hide-no-data
        hide-selected
        multiple
        single-line
      ></v-autocomplete>
      <v-divider></v-divider>
      <v-text-field
        label="What?"
        placeholder="What?"
        single-line
        full-width
        hide-details
      ></v-text-field>
      <v-divider></v-divider>
      <v-text-field
        label="Amount"
        placeholder="How much?"
        single-line
        full-width
        hide-details
      ></v-text-field>
    </v-form>
  </v-card>
</template>

<script>
export default {
    name: 'AddDebtForm',
    data () {
      return {
        selected: ['John Kowalski'],
        items: ['John Kowalski', 'Adam Johnes', 'Ian Goodmore', 'Fahrad Agron'],
        title: 'Hi,\nI just wanted to check in and see if you had any plans the upcoming weekend. We are thinking of heading up to Napa'
      }
    }
}
</script>

<style>

</style>
<template>
  <div>
    <v-row justify="space-between">
      <v-col cols="12" md="4">
        <v-form ref="form">
          <v-col cols="12" md="10">
              <h3>Your name</h3>
            <v-text-field :counter="max" filled></v-text-field>
          </v-col>

          <v-col cols="12" md="10">
            <h3>Write a message to us</h3>
            <v-textarea
            style="margin-top: 10px;"
              filled
              name="input-7-4"
            ></v-textarea>
          </v-col>
        </v-form>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  name: "Contact",
  data() {
    return {
      model: "Ryan"
    };
  }
};
</script>

<style>
</style>
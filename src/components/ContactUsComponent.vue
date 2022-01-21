<template>
  <v-container  class="pt-15 mt-12">
    <v-row justify="center">
      <v-col lg="12" class="text-center">
        <v-subheader class="text-h4 justify-center">Contact Us</v-subheader>
        <p>Lorem Ipsum is simply dummy text of the printing and typesetting</p>
      </v-col>
      <v-col lg="6">
        <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3746984.465708819!2d88.10026026270491!3d23.490583053663357!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x30adaaed80e18ba7%3A0xf2d28e0c4e1fc6b!2sBangladesh!5e0!3m2!1sen!2sbd!4v1642763959134!5m2!1sen!2sbd" width="100%" height="100%" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
      </v-col>
      <v-col lg="6">
        <v-form ref="form">
          <v-text-field
              v-model="contractInfo.name"
              label="Name"
              required
          ></v-text-field>

          <v-text-field
              v-model="contractInfo.email"
              label="E-mail"
              required
          ></v-text-field>

        <v-textarea label="Message" v-model="contractInfo.message">

        </v-textarea>

          <v-btn
              color="success"
              class="mr-4"
          >
            Send
          </v-btn>




        </v-form>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: "ContactUsComponent",
  data(){
    return{
      contractInfo:{}
    }
  }
}
</script>

<style scoped>

</style>
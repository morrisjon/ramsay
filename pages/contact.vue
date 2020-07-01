<template>
  <div class="primary darken-1 py-16">
    <h1
      class="text-h3 grey--text text--lighten-4 text-center font-weight-bold custom-heading"
    >
      Contact Us Now!
    </h1>
    <h4
      class="text-h6 grey--text text--lighten-3 text-center px-16 custom-heading mt-5 mb-12"
    >
      We would love to help you grow your business.
    </h4>
    <v-container>
      <v-form class="bg contact-form mx-auto py-3 px-5 rounded">
        <v-row>
          <v-col cols="12" md="6">
            <v-text-field
              label="First Name"
              placeholder="Enter your first name..."
              outlined
              required
            ></v-text-field>
          </v-col>

          <v-col cols="12" md="6">
            <v-text-field
              label="Last Name"
              placeholder="Enter your last name..."
              outlined
              required
            ></v-text-field>
          </v-col>

          <v-col cols="12" md="6">
            <v-text-field
              label="E-mail"
              outlined
              placeholder="Enter your e-mail..."
              required
              type="email"
            ></v-text-field>
          </v-col>

          <v-col cols="12" md="6">
            <v-text-field
              label="Phone"
              placeholder="Enter your phone number..."
              outlined
              type="tel"
            ></v-text-field>
          </v-col>
          <v-col cols="12">
            <v-text-field
              label="Company"
              placeholder="Enter your company name..."
              outlined
              required
            ></v-text-field>
          </v-col>
          <v-col cols="12">
            <v-textarea
              label="Message"
              placeholder="Enter your message here..."
              outlined
              required
            ></v-textarea>
          </v-col>
          <v-col cols="12">
            <v-btn color="primary" rounded>Submit</v-btn>
          </v-col>
        </v-row>
      </v-form>
    </v-container>
  </div>
</template>
<style scoped>
  .contact-form {
    width: 680px;
  }
  .custom-heading {
    width: 640px;
    margin-right: auto;
    margin-left: auto;
  }
</style>

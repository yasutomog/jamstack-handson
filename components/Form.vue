<template>
  <div>
    <!--<form name="contact" method="POST" data-netlify="true">-->
      <!--<input type="hidden" name="form-name" value="contact">-->
      <!--<p>-->
        <!--<label>Your Name: <input type="text" name="name" placeholder="name"></label>-->
      <!--</p>-->
      <!--<p>-->
        <!--<label>Message: <textarea name="message" placeholder="msg"></textarea></label>-->
      <!--</p>-->
      <!--<div data-netlify-recaptcha="true"></div>-->
      <!--<p>-->
        <!--<button type="submit">Send</button>-->
      <!--</p>-->
    <!--</form>-->
    <v-form name="contact" method="POST" data-netlify="true" lazy-validation>
      <v-text-field
              v-show="false"
              name="form-name"
              value="contact"
      />
      <v-text-field
              :counter="10"
              label="Name"
              name="name"
              required
      ></v-text-field>

      <v-text-field
              label="E-mail"
              name="message"
              required
      ></v-text-field>
      <v-btn block color="secondary" dark type="submit">Send</v-btn>
    </v-form>
  </div>
</template>

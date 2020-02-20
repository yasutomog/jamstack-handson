<template>
  <div>
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
      <div>
        <script type="text/javascript" async="" src="https://www.gstatic.com/recaptcha/releases/JZfekeK8w6ZlhLfH_ZyseSLX/recaptcha__ja.js"></script><script src="https://www.google.com/recaptcha/api.js"></script>
        <div class="g-recaptcha" data-sitekey="6LdAvUIUAAAAAHjrjmjtNTcXyKm0WKwefLp-dQv9">
          <div style="width: 304px; height: 78px;">
            <div>
              <iframe
                      src="https://www.google.com/recaptcha/api2/anchor?ar=1&amp;k=6LdAvUIUAAAAAHjrjmjtNTcXyKm0WKwefLp-dQv9&amp;co=aHR0cHM6Ly9xdWlya3ktYmhhYmhhLTg0YjliMC5uZXRsaWZ5LmNvbTo0NDM.&amp;hl=ja&amp;v=JZfekeK8w6ZlhLfH_ZyseSLX&amp;size=normal&amp;cb=uhz2vlm4rb38"
                      width="304"
                      height="78"
                      role="presentation"
                      name="a-c2vafq3z1eaq"
                      frameborder="0"
                      scrolling="no"
                      sandbox="allow-forms allow-popups allow-same-origin allow-scripts allow-top-navigation allow-modals allow-popups-to-escape-sandbox">
              </iframe>
            </div>
            <textarea id="g-recaptcha-response" name="g-recaptcha-response" class="g-recaptcha-response" style="width: 250px; height: 40px; border: 1px solid rgb(193, 193, 193); margin: 10px 25px; padding: 0px; resize: none; display: none;"></textarea>
          </div>
        </div>
        <noscript>
          <div>
            <div style="width: 302px; height: 422px; position: relative;">
              <div style="width: 302px; height: 422px; position: absolute;">
                <iframe src="https://www.google.com/recaptcha/api/fallback?k=6LdAvUIUAAAAAHjrjmjtNTcXyKm0WKwefLp-dQv9" frameborder="0" scrolling="no"
                        style="width: 302px; height:422px; border-style: none;">
                </iframe>
              </div>
            </div>
            <div style="width: 300px; height: 60px; border-style: none; bottom: 12px; left: 25px; margin: 0px; padding: 0px; right: 25px; background: #f9f9f9; border: 1px solid #c1c1c1; border-radius: 3px;">
              <textarea id="g-recaptcha-response" name="g-recaptcha-response" class="g-recaptcha-response"
              style="width: 250px; height: 40px; border: 1px solid #c1c1c1; margin: 10px 25px; padding: 0px; resize: none;" >
              </textarea>
            </div>
          </div>
        </noscript>
      </div>
      <v-btn block color="secondary" dark type="submit">Send</v-btn>
    </v-form>
  </div>
</template>

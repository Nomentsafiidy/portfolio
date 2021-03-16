<template>
  <div id="m_contact">
    <div class="m_title">Contact</div>
    <div class="m_contact_container">
      <div class="m_contact_info">
        <div class="m_contact_title">
          Contact Info
        </div>
        <p>
          Une idée? Un projet ? N'hésite pas à me contacter
        </p>
        <div class="m_contact_item">
          <div class="m_avatar_icon">
            <img
              src="./../../assets/svg/email.svg"
              width="40"
              height="40"
              alt="linkedin"
            />
          </div>
          <div class="m_content">
            <div class="m_content_title">Email</div>
            <div class="m_content_descrition">mnomentsafidyca@gmail.com</div>
          </div>
        </div>
        <div class="m_contact_item">
          <div class="m_avatar_icon">
            <img
              src="./../../assets/svg/call.svg"
              width="40"
              height="40"
              alt="linkedin"
            />
          </div>
          <div class="m_content">
            <div class="m_content_title">Phone</div>
            <div class="m_content_descrition">+261 34 94 156 67</div>
          </div>
        </div>
        <div class="m_contact_item">
          <div class="m_avatar_icon">
            <img
              src="./../../assets/svg/skype.svg"
              width="40"
              height="40"
              alt="linkedin"
            />
          </div>
          <div class="m_content">
            <div class="m_content_title">Skype</div>
            <div class="m_content_descrition">
              Nomentsafidy.ANDRIAMIARANTSOA
            </div>
          </div>
        </div>
      </div>
      <div class="m_contact_form">
        <div class="m_contact_title">
          Envoyer un message
        </div>
        <form class="m_form_content" action="#">
          <input class="m_input" type="text" placeholder="Nom *" />
          <input class="m_input" type="text" placeholder="Email *" />
          <input class="m_input" type="text" placeholder="Objet" />
          <textarea
            class="m_textarea"
            rows="4"
            placeholder="Message"
          ></textarea>
          <input class="m_btn_warning" type="Submit" value="Send Message" />
        </form>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Contact",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style src="./contact.scss" lang="scss"></style>

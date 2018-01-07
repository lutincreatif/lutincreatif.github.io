---
layout: page
title: Contacts
permalink: /contact/
---

<form action="https://formspree.io/lutincreatif@gmail.com"
      method="POST">

    <!--
    <input type="text" name="name"><br />
    <input type="email" name="_replyto"><br />
    <input type="objet" name="_replyto"><br />
    <textarea>  </textarea>

    <input type="submit" value="Envoyer">
    -->
      <input type="hidden" name="_language" value="fr" />
      <input type="hidden" name="_next" value="{{ '/thanks/' | relative_url }}" />

       <label for="name">Nom : <span class="required">*</span></label><br />
       <input type="text" id="name" name="name" value="" placeholder="John Doe" required="required" autofocus="autofocus" /><br /><br />

       <label for="email">Email : <span class="required">*</span></label><br />
       <input type="email" id="email" name="email" value="" placeholder="johndoe@example.com" required="required" /><br /><br />

       <label for="message">Message: <span class="required">*</span></label><br />
       <textarea id="message" name="message" placeholder="Votre message" required="required" data-minlength="20" rows="4" cols="80"></textarea><br /><br />

       <span id="loading"></span>
       <input type="submit" value="Envoyer" id="submit-button" />
</form>

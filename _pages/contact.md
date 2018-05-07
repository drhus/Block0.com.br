---
title: Contact us
permalink: /contact/
ext-js: /js/gform-submission-handler.js
---

If you want to get in touch with genesisBlock, you can either email <a href="mailto:genesis.block@fecap.edu.br">Prof. Jésus Gomes</a> or fill out the form below. 

  <form id="gform" method="POST" class="pure-form pure-form-stacked" data-email="example@email.net"
  action="https://script.google.com/macros/s/AKfycbwy9hyU8QGx9Fxzm8t0x2qthrSrX-cifqwaPVxwSpeTYLsZ9Pw7/exec">
  <div class="row">
    <div class="col-xs-6">
      <input type="email" name="_replyto" class="form-control input-lg" placeholder="Email" title="Email">
    </div>
    <div class="col-xs-6">
      <input type="text" name="name" class="form-control input-lg" placeholder="Name" title="Name">
    </div>
  </div>
  <input type="hidden" name="_subject" value="New submission from genesisBlock website">
  <textarea type="text" name="content" class="form-control input-lg" placeholder="Message" title="Message" required="required" rows="3"></textarea>

  <button type="submit" class="btn btn-lg btn-primary">Submit</button>
</form>


  <form id="gform" method="POST" class="pure-form pure-form-aligned"  action="https://script.google.com/macros/s/AKfycbwy9hyU8QGx9Fxzm8t0x2qthrSrX-cifqwaPVxwSpeTYLsZ9Pw7/exec">

    <fieldset class="pure-group">
      <input class="pure-input-1-2" id="name" name="name" placeholder="Full Name*" />
      <input class="pure-input-1-2" id="email" name="email" type="email" value="" required placeholder="Email Address*"/>
      <span id="email-invalid" style="display:none"> Must be a valid email address</span>
      <textarea class="pure-input-1-2" id="message" name="message" placeholder="Message / Inquiry*"></textarea>
    </fieldset>

    <button type="submit" class="pure-button pure-input-1-2">Submit</button>

  </form>


  <div style="display:none;" id="thankyou_message">
    <h2><em>Done!</em></h2>
  </div>

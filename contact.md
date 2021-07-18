---
layout: default
title: Contact
description: Get in touch with the TruCol protocol.
---

<form name="contact" method="POST" netlify>
  <div class="form-group col-sm-6">
    <label for="name"><h5 class="no-anchor">Your Name</h5></label>
    <input type="text" class="form-control form-control-lg" name="name" id="name" aria-describedby="nameHelp">
    <small id="nameHelp" class="form-text text-muted">We would like to get to know you better.</small>
  </div>
  <div class="form-group col-sm-6">
    <label for="email"><h5 class="no-anchor">Email address</h5></label>
    <input type="email" class="form-control form-control-lg" name="email" id="email" aria-describedby="emailHelp">
    <small id="emailHelp" class="form-text text-muted">We'll never share your email with anyone else.</small>
  </div>
  <div class="form-group col-sm-12">
    <label for="message"><h5 class="no-anchor">Message</h5></label>
    <textarea class="form-control form-control-lg" name="message" id="message" rows="3" style="height:200px;"></textarea>
  </div>
  <button type="submit" class="btn btn-primary">Submit</button>
</form>

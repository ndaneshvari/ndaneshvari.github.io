---
layout: archive
title: "Contact me!"
permalink: /contact/
author_profile: true

---

{% include base_path %}

***
Feel free to reach out for anything. Happy to chat professionally or as friends. 

local USERNAME = '<SMTP USERNAME>'
local PASSWORD = '<SMTP PASSWORD>'
local SERVER = '<SMTP SERVER>'
local RECAPTCHAKEY = '<RECAPTCHA PRIVATE KEY>'
local recaptcha = require 'recaptcha'
local markdown = require 'markdown'
if recaptcha.validate(RECAPTCHAKEY, request) then
        html = markdown(request.form.body)
        email.send {
                server = SERVER, username = USERNAME, password = PASSWORD,
                from = 'hello@webscript.io', to = 'hello@webscript.io',
                subject = '[contact form] '..request.form.subject,
                text = request.form.body,
                replyto = request.form.replyto,
                html = markdown(request.form.body)
        }
        return 'Mail sent.'
else
        return 'Failed CAPTCHA.'
end



<form accept-charset="UTF-8" action="https://getform.io/{YOUR_UNIQUE_FORM_ENDPOINT}" method="POST" enctype="multipart/form-data" target="_blank">
            <div class="form-group">
            <label for="exampleInputName">Name</label>
            <input type="text" name="name" class="form-control" id="exampleInputName" placeholder="Enter your name" required="required">
          </div>
          <div class="form-group">
            <label for="exampleInputEmail1" required="required">Email address</label>
            <input type="email" name="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" placeholder="Enter email">
          </div>
        <div class="form-group">
            <label for="exampleMessage">Message</label>
            <input type="text" name="message" class="form-control" id="exampleInputName" placeholder="What's on your mind?" required="required">
          </div>
          <hr>
          <div class="form-group mt-3">
            <label class="mr-2">Attach a file (optional):</label>
            <input type="file" name="file">
          </div>
          <hr>
          <button type="submit" class="btn btn-primary">Submit</button>
        </form>

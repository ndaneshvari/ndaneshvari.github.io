---
layout: archive
title: "Contact me!"
permalink: /contact/
author_profile: true

---

{% include base_path %}

***
Feel free to reach out for anything. Happy to chat professionally or as friends. 

@import url(http://fonts.googleapis.com/css?family=Montserrat:400,700);

body { background:rgb(30,30,40); }
form { max-width:420px; margin:50px auto; }

.feedback-input {
  color:white;
  font-family: Helvetica, Arial, sans-serif;
  font-weight:500;
  font-size: 18px;
  border-radius: 5px;
  line-height: 22px;
  background-color: transparent;
  border:2px solid #CC6666;
  transition: all 0.3s;
  padding: 13px;
  margin-bottom: 15px;
  width:100%;
  box-sizing: border-box;
  outline:0;
}

.feedback-input:focus { border:2px solid #CC4949; }

textarea {
  height: 150px;
  line-height: 150%;
  resize:vertical;
}

[type="submit"] {
  font-family: 'Montserrat', Arial, Helvetica, sans-serif;
  width: 100%;
  background:#CC6666;
  border-radius:5px;
  border:0;
  cursor:pointer;
  color:white;
  font-size:24px;
  padding-top:10px;
  padding-bottom:10px;
  transition: all 0.3s;
  margin-top:-4px;
  font-weight:700;
}
[type="submit"]:hover { background:#CC4949; }



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

---
layout: archive
title: "Contact me!"
permalink: /contact/
author_profile: true

---

{% include base_path %}

***
Feel free to reach out for anything. Happy to chat professionally or as friends. 

import 'jquery';
import 'bootstrap';
import ContactForm from 'auth0-contact-form';

const metricsLib = window.metricsLib;
const $ = jQuery;
const options = {
  onFormSuccess(metricsData) {
    metricsLib.track('contact-form-success', metricsData);
  }
};

const contactForm = new ContactForm(options);

$('.btn').click(contactForm.show);

@import '../node_modules/auth0-contact-form/build/contact-form.css'

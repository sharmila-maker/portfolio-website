Sharmila A - Portfolio Website
==============================

FILES
  index.html   the whole website (HTML + CSS + JavaScript)
  photo.jpg    YOUR PHOTO (add it next to index.html, exact name: photo.jpg)
               Already included (square, face centred). To change it, replace the file with another square photo.
               If the file is missing, a gold "SA" monogram is shown.

OPEN: double-click index.html.

GLITTER: gold sparkles float on the page and follow the mouse. They switch off
automatically for people who enabled "reduce motion" on their device.

MESSAGES AND E-MAIL
  Without setup, "Send message" opens the visitor's mail app addressed to you,
  and "WhatsApp me" opens WhatsApp chat with +91 86105 57485 (works already).

  Make the form send real e-mails to your Gmail, with an automatic reply to
  the visitor (free, EmailJS, 200 mails a month):
   1. Sign up at emailjs.com.
   2. Email Services > Add New Service > Gmail > connect a.sharmilaa818@gmail.com.
      Copy the Service ID.
   3. Email Templates > Create New Template  (this mail comes to YOU)
        To Email: a.sharmilaa818@gmail.com
        Reply-To: {{reply_to}}
        Subject:  Portfolio message from {{from_name}}
        Content:  {{message}}  -  {{from_name}} ({{from_email}})
      Copy the Template ID.
   4. Create a second template (the automatic REPLY to the visitor)
        To Email: {{from_email}}
        Subject:  Thanks for contacting Sharmila
        Content:  Hi {{from_name}}, thank you for your message. I will reply soon.
      Copy its Template ID.
   5. Account > General: copy your Public Key.
   6. In index.html find MAIL_CONFIG and paste the four values:
        publicKey, serviceId, templateId, autoReplyTemplateId
   7. Save, open the page, send a test message.

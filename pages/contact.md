---
layout: default
title: Contact
permalink: /contact/
---

<div style="text-align: center; margin: 2rem 0;">
  <h2>Contact Me</h2>
  
  <div class="row mt-4">
    <div class="col-md-6">
      <div class="card h-100">
        <div class="card-body">
          <h5 class="card-title">Contact Information</h5>
          <div class="mt-3">
            <p><strong>Phone:</strong> <a href="tel:+15402302501">+1 (540) 230-2501</a></p>
            <p><strong>Email:</strong> <a href="mailto:stormwatersolutions24060@gmail.com">stormwatersolutions24060@gmail.com</a></p>
          </div>
        </div>
      </div>
    </div>
    
    <div class="col-md-6">
      <div class="card h-100">
        <div class="card-body">
          <h5 class="card-title">Send a Message</h5>
          <form id="contactForm" class="mt-3">
            <div class="mb-3">
              <label for="name" class="form-label">Name *</label>
              <input type="text" class="form-control" id="name" name="name" required>
            </div>
            
            <div class="mb-3">
              <label for="phone" class="form-label">Phone Number</label>
              <input type="tel" class="form-control" id="phone" name="phone">
            </div>
            
            <div class="mb-3">
              <label for="email" class="form-label">Email *</label>
              <input type="email" class="form-control" id="email" name="email" required>
            </div>
            
            <div class="mb-3">
              <label for="message" class="form-label">Message *</label>
              <textarea class="form-control" id="message" name="message" rows="4" required></textarea>
            </div>
            
            <button type="submit" class="btn btn-primary">Send Message</button>
          </form>
          
          <script>
            document.getElementById('contactForm').addEventListener('submit', function(e) {
              e.preventDefault();
              
              const name = document.getElementById('name').value;
              const phone = document.getElementById('phone').value;
              const email = document.getElementById('email').value;
              const message = document.getElementById('message').value;
              
              const subject = 'Contact Form Submission from ' + name;
              const body = 'Name: ' + name + '\n' +
                          'Phone: ' + phone + '\n' +
                          'Email: ' + email + '\n\n' +
                          'Message:\n' + message;
              
              const mailtoLink = 'mailto:stormwatersolutions24060@gmail.com?subject=' + encodeURIComponent(subject) + '&body=' + encodeURIComponent(body);
              
              window.location.href = mailtoLink;
            });
          </script>
        </div>
      </div>
    </div>
  </div>
</div> 
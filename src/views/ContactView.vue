<template>
  <section id="contact">
    <div class="container">
      <div class="row justify-content-end">
        <div class="col flex-grow-1"></div>
        <div class="col-12 col-sm-8 col-md-6 col-lg-4">
          <div class="contact-card">
            <div class="contact-container-title">
              <h4 class="contact-title">Get in touch</h4>
              <div class="contact-content">
                <form id="contact-form">
                  <label class="form-label" for="SenderName">Name</label>
                  <input type="text" class="form-control" id="SenderName" />
                  <label class="form-label" for="SenderMail">E-mail</label>
                  <input type="email" class="form-control" id="SenderMail" />
                  <label class="form-label" for="Message">Message</label>
                  <textarea class="form-control" rows="10"></textarea>
                  <button class="btn btn-primary w-100 mt-3" disabled>
                    <font-awesome-icon :icon="['fas', 'paper-plane']" /> Coming soon!
                  </button>
                </form>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style>
#contact {
  background-color: rgba(var(--bs-dark-rgb), 1);
  background-repeat: no-repeat;
  background-image: url(src/assets/images/vanishing-stripes.svg);
  background-size: cover;
}
.contact-card {
  width: 100%;
  min-height: 20rem;
  -webkit-backdrop-filter: blur(4px);
  backdrop-filter: blur(4px);
  padding: 1.5rem 2.5rem;
  box-sizing: border-box;
  background-image: linear-gradient(
    145deg,
    rgba(49, 50, 54, 0.3) 0%,
    rgba(124, 152, 179, 0.3) 100%
  );
  border-radius: 10px;
}
</style>

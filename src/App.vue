<script setup></script>

<template>
  <main>
    <h1>My Brothers’ Farm is no longer in business</h1>

    <div class="sections">
      <section>
        <p>For meat products, contact <strong>Grateful Bison</strong></p>

        <div class="contact-container">
          <div class="contact-list start">
            <a
              href="https://www.instagram.com/gratefulbison/"
              class="img-link row"
            >
              <img
                class="icon"
                src="./assets/instagram-logo.png"
                alt="Instagram logo"
              />
              @gratefulbison
            </a>

            <a href="mailto:gratefulbison@proton.me" class="img-link row">
              <img
                class="icon"
                src="./assets/email-icon.png"
                alt="Email icon"
              />
              gratefulbison@proton.me
            </a>
          </div>
        </div>
      </section>

      <div class="vertical-divider" />

      <section>
        <p>For tree products, contact <strong>Farmhands Co-op</strong></p>
        <div class="contact-list">
          <a href="https://farmhandscoop.com" class="img-link">
            <img
              class="logo"
              src="./assets/farmhands-logo.png"
              alt="Farmhands Co-op logo"
            />
            FarmhandsCoop.com
          </a>
        </div>
      </section>
    </div>
  </main>
</template>

<style scoped>
h1 {
  text-align: center;
  margin: 0 0 1rem;
  font-size: clamp(1.25rem, 4vw, 2rem);
}

.img-link {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
  align-items: center;
  text-decoration: none;
}

.img-link.row {
  flex-direction: row;
}

.img-link:hover {
  text-decoration: underline;
}

.sections {
  display: flex;
  flex-direction: column;
  align-items: stretch;
  gap: 1.5rem;
  margin-top: 1.5rem;
}

.vertical-divider {
  width: 100%;
  height: 1px;
  background-color: #ddd;
}

.contact-list {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 1rem;
  margin-top: 1rem;
}

.contact-list.start {
  align-items: flex-start;
}

.contact-container {
  display: flex;
  justify-content: center;
}

.icon {
  width: clamp(56px, 12vw, 64px);
  height: auto;
  aspect-ratio: 1 / 1;
}

.logo {
  width: min(80vw, 352px);
  height: auto;
}

@media (min-width: 740px) {
  .sections {
    flex-direction: row;
    gap: 2rem;
  }

  .vertical-divider {
    width: 1px;
    height: auto;
    background-color: transparent;
    border-left: 1px solid #ddd;
  }
}
</style>

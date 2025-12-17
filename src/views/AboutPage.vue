<script setup>
// AboutPage component
</script>

<template>
  <div class="about-page">
    <!-- Page Header -->
    <section class="page-header">
      <div class="container">
        <h1 class="page-title">About Us</h1>
        <p class="page-subtitle">
          <!-- Add your about page tagline -->
          Learn more about who we are and what drives us.
        </p>
      </div>
    </section>

    <!-- Story Section -->
    <section class="section">
      <div class="container">
        <div class="content-grid">
          <div class="content-text">
            <h2>Our Story</h2>
            <p>
              <!-- Add your organization's story here -->
              Health & Awareness, Inc is a faith-based 501 (c)(3) organization that educates individuals in the community by raising awareness about preventive behaviors, early detection, and a healthy lifestyle to stop the progression of Chronic Kidney Disease. 
            </p>
            <p>
              Add more paragraphs as needed to tell your complete story.
            </p>
          </div>
          <div class="content-image">
            <!-- Add an image here -->
            <div class="image-placeholder">
              <span>Image</span>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Values Section -->
    <section class="section values-section">
      <div class="container">
        <div class="section-header">
          <h2 class="section-title">Our Values</h2>
          <p class="section-subtitle">
            The principles that guide everything we do.
          </p>
        </div>
        <div class="values-grid">
          <div class="value-item">
            <h3>Value 1</h3>
            <p>Description of this core value and what it means to your organization.</p>
          </div>
          <div class="value-item">
            <h3>Value 2</h3>
            <p>Description of this core value and what it means to your organization.</p>
          </div>
          <div class="value-item">
            <h3>Value 3</h3>
            <p>Description of this core value and what it means to your organization.</p>
          </div>
          <div class="value-item">
            <h3>Value 4</h3>
            <p>Description of this core value and what it means to your organization.</p>
          </div>
        </div>
      </div>
    </section>

    <!-- Team Section -->
    <section class="section">
      <div class="container">
        <div class="section-header">
          <h2 class="section-title">Our Team</h2>
          <p class="section-subtitle">
            Meet the dedicated people behind our mission.
          </p>
        </div>
        <div class="team-grid">
          <div class="team-member">
            <div class="member-photo">
              <div class="photo-placeholder"></div>
            </div>
            <h3 class="member-name">Team Member Name</h3>
            <p class="member-role">Role / Title</p>
          </div>
          <div class="team-member">
            <div class="member-photo">
              <div class="photo-placeholder"></div>
            </div>
            <h3 class="member-name">Team Member Name</h3>
            <p class="member-role">Role / Title</p>
          </div>
          <div class="team-member">
            <div class="member-photo">
              <div class="photo-placeholder"></div>
            </div>
            <h3 class="member-name">Team Member Name</h3>
            <p class="member-role">Role / Title</p>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<style scoped>
.page-header {
  background: linear-gradient(135deg, var(--color-primary) 0%, var(--color-primary-dark) 100%);
  color: var(--color-white);
  padding: var(--spacing-16) 0;
  text-align: center;
}

.page-title {
  color: var(--color-white);
  margin-bottom: var(--spacing-4);
}

.page-subtitle {
  font-size: var(--font-size-lg);
  opacity: 0.9;
  max-width: 600px;
  margin: 0 auto;
}

/* Content Grid */
.content-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: var(--spacing-10);
  align-items: center;
}

.content-text h2 {
  margin-bottom: var(--spacing-6);
}

.content-text p {
  color: var(--color-gray-600);
  line-height: var(--line-height-relaxed);
}

.image-placeholder {
  background-color: var(--color-gray-200);
  border-radius: var(--radius-xl);
  aspect-ratio: 4/3;
  display: flex;
  align-items: center;
  justify-content: center;
  color: var(--color-gray-500);
  font-size: var(--font-size-lg);
}

/* Values Section */
.values-section {
  background-color: var(--color-gray-50);
}

.values-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: var(--spacing-6);
}

.value-item {
  background-color: var(--color-white);
  padding: var(--spacing-8);
  border-radius: var(--radius-xl);
  box-shadow: var(--shadow-sm);
}

.value-item h3 {
  color: var(--color-primary);
  margin-bottom: var(--spacing-3);
}

.value-item p {
  color: var(--color-gray-600);
  margin-bottom: 0;
}

/* Team Section */
.team-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: var(--spacing-8);
}

.team-member {
  text-align: center;
}

.photo-placeholder {
  width: 150px;
  height: 150px;
  background-color: var(--color-gray-200);
  border-radius: var(--radius-full);
  margin: 0 auto var(--spacing-4);
}

.member-name {
  font-size: var(--font-size-lg);
  margin-bottom: var(--spacing-1);
}

.member-role {
  color: var(--color-gray-500);
  margin-bottom: 0;
}

/* Responsive */
@media (min-width: 768px) {
  .content-grid {
    grid-template-columns: 1fr 1fr;
  }

  .values-grid {
    grid-template-columns: repeat(2, 1fr);
  }

  .team-grid {
    grid-template-columns: repeat(3, 1fr);
  }
}
</style>

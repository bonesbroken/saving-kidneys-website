<script setup>
// HomePage component
</script>

<template>
  <div class="home-page">
    <!-- Hero Section -->
    <section class="hero">
      <div class="container hero-container">
        <div class="hero-content">
          <h1 class="hero-title">
            <!-- Add your main headline here -->
            Making a Difference Together
          </h1>
          <p class="hero-subtitle">
            <!-- Add your tagline or brief description here -->
            Join us in our mission to create positive change in our community.
          </p>
          <div class="hero-actions">
            <RouterLink to="/donate" class="btn btn-primary btn-lg">
              Donate Now
            </RouterLink>
            <RouterLink to="/about" class="btn btn-outline btn-lg">
              Learn More
            </RouterLink>
          </div>
        </div>
      </div>
    </section>

    <!-- Impact Stats Section -->
    <section class="section stats-section">
      <div class="container">
        <div class="stats-grid">
          <div class="stat-item">
            <span class="stat-number">0</span>
            <span class="stat-label">Lives Impacted</span>
          </div>
          <div class="stat-item">
            <span class="stat-number">0</span>
            <span class="stat-label">Years of Service</span>
          </div>
          <div class="stat-item">
            <span class="stat-number">0</span>
            <span class="stat-label">Volunteers</span>
          </div>
          <div class="stat-item">
            <span class="stat-number">$0</span>
            <span class="stat-label">Funds Raised</span>
          </div>
        </div>
      </div>
    </section>

    <!-- Mission Preview Section -->
    <section class="section mission-preview">
      <div class="container">
        <div class="section-header">
          <h2 class="section-title">Our Mission</h2>
          <p class="section-subtitle">
            <!-- Add your mission statement preview here -->
            Brief description of what your charity does and why it matters.
          </p>
        </div>
        <div class="mission-content">
          <RouterLink to="/mission" class="btn btn-secondary">
            Learn About Our Mission
          </RouterLink>
        </div>
      </div>
    </section>

    <!-- Programs/Services Section -->
    <section class="section programs-section">
      <div class="container">
        <div class="section-header">
          <h2 class="section-title">What We Do</h2>
          <p class="section-subtitle">
            <!-- Add description of your programs -->
            Our programs and services that help make a difference.
          </p>
        </div>
        <div class="programs-grid">
          <div class="card">
            <div class="card-body">
              <h3 class="card-title">Program 1</h3>
              <p class="card-text">
                Description of program or service goes here.
              </p>
            </div>
          </div>
          <div class="card">
            <div class="card-body">
              <h3 class="card-title">Program 2</h3>
              <p class="card-text">
                Description of program or service goes here.
              </p>
            </div>
          </div>
          <div class="card">
            <div class="card-body">
              <h3 class="card-title">Program 3</h3>
              <p class="card-text">
                Description of program or service goes here.
              </p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Call to Action Section -->
    <section class="section cta-section">
      <div class="container">
        <div class="cta-content">
          <h2 class="cta-title">Ready to Make a Difference?</h2>
          <p class="cta-text">
            Your support helps us continue our vital work in the community.
          </p>
          <div class="cta-actions">
            <RouterLink to="/donate" class="btn btn-primary btn-lg">
              Donate Today
            </RouterLink>
            <RouterLink to="/contact" class="btn btn-outline btn-lg">
              Get Involved
            </RouterLink>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<style scoped>
/* Hero Section */
.hero {
  background: linear-gradient(135deg, var(--color-primary) 0%, var(--color-primary-dark) 100%);
  color: var(--color-white);
  padding: var(--spacing-20) 0;
  text-align: center;
}

.hero-content {
  max-width: 800px;
  margin: 0 auto;
}

.hero-title {
  font-size: var(--font-size-5xl);
  color: var(--color-white);
  margin-bottom: var(--spacing-6);
}

.hero-subtitle {
  font-size: var(--font-size-xl);
  opacity: 0.9;
  margin-bottom: var(--spacing-8);
}

.hero-actions {
  display: flex;
  gap: var(--spacing-4);
  justify-content: center;
  flex-wrap: wrap;
}

.hero .btn-outline {
  border-color: var(--color-white);
  color: var(--color-white);
}

.hero .btn-outline:hover {
  background-color: var(--color-white);
  color: var(--color-primary);
}

/* Stats Section */
.stats-section {
  background-color: var(--color-gray-50);
}

.stats-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: var(--spacing-8);
  text-align: center;
}

.stat-item {
  padding: var(--spacing-6);
}

.stat-number {
  display: block;
  font-size: var(--font-size-4xl);
  font-weight: var(--font-weight-bold);
  color: var(--color-primary);
  margin-bottom: var(--spacing-2);
}

.stat-label {
  font-size: var(--font-size-base);
  color: var(--color-gray-600);
}

/* Mission Preview */
.mission-content {
  text-align: center;
}

/* Programs Section */
.programs-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: var(--spacing-6);
}

/* CTA Section */
.cta-section {
  background: linear-gradient(135deg, var(--color-secondary) 0%, var(--color-secondary-dark) 100%);
  color: var(--color-white);
  text-align: center;
}

.cta-content {
  max-width: 600px;
  margin: 0 auto;
}

.cta-title {
  color: var(--color-white);
  margin-bottom: var(--spacing-4);
}

.cta-text {
  font-size: var(--font-size-lg);
  opacity: 0.9;
  margin-bottom: var(--spacing-8);
}

.cta-actions {
  display: flex;
  gap: var(--spacing-4);
  justify-content: center;
  flex-wrap: wrap;
}

.cta-section .btn-primary {
  background-color: var(--color-white);
  color: var(--color-secondary-dark);
}

.cta-section .btn-primary:hover {
  background-color: var(--color-gray-100);
}

.cta-section .btn-outline {
  border-color: var(--color-white);
  color: var(--color-white);
}

.cta-section .btn-outline:hover {
  background-color: var(--color-white);
  color: var(--color-secondary-dark);
}

/* Responsive */
@media (min-width: 768px) {
  .hero {
    padding: var(--spacing-24) 0;
  }

  .stats-grid {
    grid-template-columns: repeat(4, 1fr);
  }

  .programs-grid {
    grid-template-columns: repeat(3, 1fr);
  }
}

@media (max-width: 768px) {
  .hero-title {
    font-size: var(--font-size-3xl);
  }
}
</style>

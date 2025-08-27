<template>
  <div id="app">
    <!-- Header Section -->
    <header class="hero">
      <div class="container">
        <div class="hero-content">
          <h1 class="hero-title">Zihan Sun</h1>
          <p class="hero-subtitle">Machine Learning & Blockchain Enthusiast</p>
          <p class="hero-description">
            Passionate about artificial intelligence, machine learning, and blockchain technology.
            Contributing to open-source projects and exploring innovative solutions.
          </p>
          <div class="hero-links">
            <a href="https://github.com/yueqianhaobo" target="_blank" class="btn btn-primary">
              <svg width="20" height="20" viewBox="0 0 24 24" fill="currentColor">
                <path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/>
              </svg>
              GitHub Profile
            </a>
          </div>
        </div>
      </div>
    </header>

    <!-- About Section -->
    <section class="section about">
      <div class="container">
        <h2 class="section-title">About Me</h2>
        <div class="about-content">
          <div class="card">
            <h3>Background</h3>
            <p>
              I am a dedicated researcher and developer with a strong focus on machine learning and blockchain technologies. 
              My work involves contributing to educational resources and developing practical implementations of cutting-edge algorithms.
            </p>
          </div>
          <div class="card">
            <h3>Interests</h3>
            <ul class="interests-list">
              <li>Machine Learning & Deep Learning</li>
              <li>Blockchain Technology</li>
              <li>Open Source Development</li>
              <li>Educational Content Creation</li>
              <li>Algorithm Implementation</li>
            </ul>
          </div>
        </div>
      </div>
    </section>

    <!-- Projects Section -->
    <section class="section projects">
      <div class="container">
        <h2 class="section-title">Featured Projects</h2>
        <div class="projects-grid grid grid-3">
          <div class="card project-card" v-for="project in projects" :key="project.id">
            <h3 class="project-title">{{ project.title }}</h3>
            <p class="project-description">{{ project.description }}</p>
            <div class="project-tags">
              <span class="tag" v-for="tag in project.tags" :key="tag">{{ tag }}</span>
            </div>
            <a :href="project.link" target="_blank" class="btn btn-outline">View Project</a>
          </div>
        </div>
      </div>
    </section>

    <!-- Contact Section -->
    <section class="section contact">
      <div class="container">
        <h2 class="section-title">Get In Touch</h2>
        <div class="contact-content">
          <div class="card contact-card">
            <p>Feel free to reach out for collaborations, discussions about machine learning, blockchain, or any interesting projects!</p>
            <div class="contact-links">
              <a href="https://github.com/yueqianhaobo" target="_blank" class="contact-link">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="currentColor">
                  <path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/>
                </svg>
                GitHub
              </a>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Footer -->
    <footer class="footer">
      <div class="container">
        <p>&copy; 2024 Zihan Sun. Built with Vue 3.</p>
      </div>
    </footer>
  </div>
</template>

<script>
import { ref } from 'vue'

export default {
  name: 'App',
  setup() {
    const projects = ref([
      {
        id: 1,
        title: 'Lee ML Notes',
        description: 'Comprehensive notes and implementations for machine learning concepts, making complex algorithms accessible to learners.',
        tags: ['Machine Learning', 'Education', 'Python'],
        link: 'https://github.com/datawhalechina/leeml-notes'
      },
      {
        id: 2,
        title: 'Blockchain Learning Program',
        description: 'Educational resources and practical implementations for understanding blockchain technology and its applications.',
        tags: ['Blockchain', 'Education', 'Cryptocurrency'],
        link: 'https://github.com/datawhalechina/team-learning-program/tree/master/Blockchain'
      },
      {
        id: 3,
        title: 'ML Toy Code',
        description: 'Collection of machine learning algorithms implemented from scratch for educational purposes and better understanding.',
        tags: ['Machine Learning', 'Algorithms', 'Implementation'],
        link: 'https://github.com/datawhalechina/machine-learning-toy-code'
      }
    ])

    return {
      projects
    }
  }
}
</script>

<style scoped>
.hero {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  padding: 100px 0;
  text-align: center;
}

.hero-title {
  font-size: 3.5rem;
  font-weight: 700;
  margin-bottom: 1rem;
}

.hero-subtitle {
  font-size: 1.5rem;
  margin-bottom: 1.5rem;
  opacity: 0.9;
}

.hero-description {
  font-size: 1.1rem;
  max-width: 600px;
  margin: 0 auto 2rem;
  opacity: 0.8;
  line-height: 1.6;
}

.hero-links {
  margin-top: 2rem;
}

.btn-primary {
  background-color: rgba(255, 255, 255, 0.2);
  border: 2px solid rgba(255, 255, 255, 0.3);
  color: white;
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  padding: 15px 30px;
  font-size: 1.1rem;
  backdrop-filter: blur(10px);
}

.btn-primary:hover {
  background-color: rgba(255, 255, 255, 0.3);
  border-color: rgba(255, 255, 255, 0.5);
}

.about {
  background-color: white;
}

.about-content {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
}

.interests-list {
  list-style: none;
  padding: 0;
}

.interests-list li {
  padding: 0.5rem 0;
  border-bottom: 1px solid #eee;
}

.interests-list li:last-child {
  border-bottom: none;
}

.interests-list li:before {
  content: '▸';
  color: #3498db;
  margin-right: 0.5rem;
}

.projects {
  background-color: #f8f9fa;
}

.projects-grid {
  margin-top: 3rem;
}

.project-card {
  display: flex;
  flex-direction: column;
  height: 100%;
}

.project-title {
  color: #2c3e50;
  margin-bottom: 1rem;
  font-size: 1.3rem;
}

.project-description {
  flex-grow: 1;
  margin-bottom: 1.5rem;
  color: #666;
  line-height: 1.6;
}

.project-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem;
  margin-bottom: 1.5rem;
}

.tag {
  background-color: #e3f2fd;
  color: #1976d2;
  padding: 0.25rem 0.75rem;
  border-radius: 20px;
  font-size: 0.85rem;
  font-weight: 500;
}

.btn-outline {
  background-color: transparent;
  border: 2px solid #3498db;
  color: #3498db;
  margin-top: auto;
}

.btn-outline:hover {
  background-color: #3498db;
  color: white;
}

.contact {
  background-color: white;
}

.contact-content {
  max-width: 600px;
  margin: 0 auto;
  text-align: center;
}

.contact-card {
  text-align: center;
}

.contact-links {
  margin-top: 2rem;
}

.contact-link {
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  color: #3498db;
  text-decoration: none;
  font-weight: 500;
  transition: color 0.3s ease;
}

.contact-link:hover {
  color: #2980b9;
}

.footer {
  background-color: #2c3e50;
  color: white;
  text-align: center;
  padding: 2rem 0;
}

@media (max-width: 768px) {
  .hero-title {
    font-size: 2.5rem;
  }
  
  .hero-subtitle {
    font-size: 1.2rem;
  }
  
  .about-content {
    grid-template-columns: 1fr;
  }
}
</style>
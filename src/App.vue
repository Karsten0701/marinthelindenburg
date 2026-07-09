<script setup>
import logoUrl from '../logo.png'
import portraitUrl from '../portrait.jpeg'

const navItems = [
  { label: 'Profile', href: '#profile' },
  { label: 'Experience', href: '#experience' },
  { label: 'Skills', href: '#skills' },
  { label: 'Contact', href: '#contact' },
]

const highlights = [
  'Attraction & Theme Park Management student',
  'Guest service, hospitality, retail and marketing experience',
  'Leadership, public speaking and performance background',
]

const experiences = [
  {
    role: 'Promotion & Marketing Employee',
    company: 'Brandwise',
    period: 'February 2026 - Present',
    points: [
      'Represent brands during promotional events and campaigns while creating positive customer interactions.',
      'Engage with guests and consumers by providing product information and encouraging participation.',
      'Adapt communication style to connect with different audiences.',
      'Work independently while maintaining professionalism and enthusiasm.',
      'Develop skills in marketing, brand representation, and guest engagement.',
    ],
  },
  {
    role: 'Restaurant Service Employee',
    company: 'Hospitality',
    period: 'March 2025 - August 2025',
    points: [
      'Provided friendly and attentive service in a fast-paced hospitality environment.',
      'Created welcoming experiences for guests through positive communication and attention to detail.',
      'Collaborated with team members to ensure smooth daily operations.',
      'Learned the importance of hospitality standards and guest satisfaction.',
    ],
  },
  {
    role: 'Owner & Market Vendor',
    company: 'Handmade Crochet Business',
    period: 'July 2024 - December 2024',
    points: [
      'Created and sold handmade crochet products at local markets.',
      'Managed customer relationships, sales transactions, and product presentation.',
      'Developed entrepreneurial skills, creativity, and confidence in interacting with customers.',
      'Took responsibility for planning, organization, and independent work.',
    ],
  },
  {
    role: 'Cashier',
    company: 'Albert Heijn',
    period: 'April 2022 - June 2024',
    points: [
      'Delivered efficient and friendly service to customers in a busy retail environment.',
      'Assisted guests with questions and ensured a positive shopping experience.',
      'Handled transactions accurately and responsibly.',
      'Developed strong customer service, teamwork, and problem-solving skills.',
    ],
  },
]

const achievements = [
  {
    title: 'Student Council President',
    points: [
      'Represented students and acted as a communication link between students and school leadership.',
      'Led meetings and contributed to improving the student experience.',
      'Developed leadership, teamwork, and decision-making skills.',
    ],
  },
  {
    title: 'Municipal Youth Panel Member',
    meta: '2021 - 2024',
    points: [
      'Participated in discussions with local representatives about topics affecting young people.',
      'Shared ideas and perspectives to support community improvements.',
      'Collaborated with other young people and professionals.',
    ],
  },
  {
    title: 'Municipal Debate Tournament',
    points: [
      'Winner of the Municipal Debate Tournament.',
      'Runner-up in a separate edition.',
      'Strengthened public speaking, confidence, critical thinking, and persuasive communication skills.',
    ],
  },
  {
    title: 'Lead Performer - High School Musical',
    meta: '2024',
    points: [
      "Performed the leading role in the school's musical production.",
      'Collaborated with performers, directors, and production teams.',
      'Developed stage presence, creativity, discipline, and confidence in front of audiences.',
    ],
  },
]

const skills = [
  'Guest Experience & Customer Service',
  'Hospitality Operations',
  'Teamwork & Collaboration',
  'Cross-Cultural Communication',
  'Public Speaking',
  'Leadership',
  'Entertainment & Performance',
  'Marketing & Brand Representation',
  'Problem Solving',
  'Adaptability',
  'Positive Attitude & Professionalism',
]

const interests = [
  'Theme Parks & Attractions',
  'Themed Entertainment',
  'Dancing',
  'Reading',
  'Traveling',
  'Spending time with friends and family',
]

const themeParkPassion = [
  'Lifelong passion for theme parks and immersive entertainment.',
  'Visited Disney Parks in California, Florida, and Paris.',
  'Visited Universal Parks in the United States.',
  'Experienced many amusement and theme parks throughout Europe and North America.',
  'Particularly inspired by Europa-Park and its focus on storytelling, attractions, and guest experiences.',
  'Interested in how theme parks create emotional connections and memorable moments for guests.',
]
</script>

<template>
  <div class="site-shell">
    <header class="topbar" aria-label="Main navigation">
      <a class="brand" href="#top" aria-label="Marinthe Lindenburg home">
        <span class="brand-mark">
          <img :src="logoUrl" alt="" />
        </span>
        <span>Marinthe Lindenburg</span>
      </a>
      <nav class="nav-links">
        <a v-for="item in navItems" :key="item.href" :href="item.href">{{ item.label }}</a>
      </nav>
    </header>

    <main id="top">
      <section class="hero section-grid">
        <div class="hero-copy">
          <p class="eyebrow">The Netherlands | Dutch native | English fluent | German basic understanding</p>
          <h1>Guest Experience & Themed Entertainment</h1>
          <p class="hero-text">
            A hospitality-minded theme park management student focused on warm service, storytelling and memorable guest moments.
          </p>
          <div class="hero-actions" aria-label="Portfolio links">
            <a class="button primary" href="#experience">View Experience</a>
            <a class="button secondary" href="#contact">Contact</a>
          </div>
        </div>

        <aside class="portrait-panel" aria-label="Professional portrait">
          <div class="portrait-frame">
            <img :src="portraitUrl" alt="Portrait of Marinthe Lindenburg" />
          </div>
          <div class="quick-card">
            <p class="quick-label">Focus</p>
            <p>Disney Academic Exchange Program, themed entertainment and positive guest interaction.</p>
          </div>
        </aside>
      </section>

      <section id="profile" class="content-section">
        <div class="section-heading">
          <p class="eyebrow">Professional Profile</p>
          <h2>Warm service with a themed entertainment mindset.</h2>
        </div>
        <div class="profile-layout">
          <p class="lead">
            Passionate first-year Attraction & Theme Park Management student with hands-on experience in guest
            service, hospitality, retail, marketing and entertainment. Skilled at creating positive interactions
            through strong communication, teamwork and enthusiasm. Experienced in leadership roles, public speaking,
            and performance environments. Driven by a lifelong passion for themed entertainment and motivated to
            contribute to memorable guest experiences as part of the Disney Academic Exchange Program.
          </p>
          <div class="highlight-list">
            <div v-for="item in highlights" :key="item" class="highlight-item">
              <span></span>
              <p>{{ item }}</p>
            </div>
          </div>
        </div>
      </section>

      <section class="split-section">
        <div class="education-block">
          <p class="eyebrow">Education</p>
          <h2>Breda University of Applied Sciences</h2>
          <p>Bachelor's Degree - Attraction & Theme Park Management</p>
          <p class="muted">Expected Graduation: 2029</p>
        </div>
        <div class="education-block compact">
          <p class="eyebrow">Previous Education</p>
          <h3>HAVO and VWO Diplomas</h3>
          <p>The Netherlands</p>
        </div>
      </section>

      <section id="experience" class="content-section experience-section">
        <div class="section-heading narrow">
          <p class="eyebrow">Professional Experience</p>
          <h2>Service, communication and responsibility in real guest-facing settings.</h2>
        </div>
        <div class="timeline">
          <article v-for="experience in experiences" :key="experience.role" class="timeline-item">
            <div class="timeline-meta">
              <p>{{ experience.period }}</p>
            </div>
            <div class="timeline-content">
              <h3>{{ experience.role }}</h3>
              <p class="company">{{ experience.company }}</p>
              <ul>
                <li v-for="point in experience.points" :key="point">{{ point }}</li>
              </ul>
            </div>
          </article>
        </div>
      </section>

      <section class="content-section">
        <div class="section-heading">
          <p class="eyebrow">Leadership & Achievements</p>
          <h2>Confidence built through leadership, debate and performance.</h2>
        </div>
        <div class="achievement-grid">
          <article v-for="achievement in achievements" :key="achievement.title" class="achievement-card">
            <h3>{{ achievement.title }}</h3>
            <p v-if="achievement.meta" class="achievement-meta">{{ achievement.meta }}</p>
            <ul>
              <li v-for="point in achievement.points" :key="point">{{ point }}</li>
            </ul>
          </article>
        </div>
      </section>

      <section id="skills" class="content-section skills-section">
        <div class="section-heading">
          <p class="eyebrow">Skills</p>
          <h2>Practical strengths for guest-focused environments.</h2>
        </div>
        <div class="skill-cloud" aria-label="Skills list">
          <span v-for="skill in skills" :key="skill">{{ skill }}</span>
        </div>
      </section>

      <section class="passion-section">
        <div>
          <p class="eyebrow">Theme Park Experience & Passion</p>
          <h2>Inspired by the way parks turn details into emotional memories.</h2>
        </div>
        <ul class="passion-list">
          <li v-for="point in themeParkPassion" :key="point">{{ point }}</li>
        </ul>
      </section>

      <section class="content-section">
        <div class="section-heading">
          <p class="eyebrow">Interests</p>
          <h2>Curiosity that stays close to people, places and stories.</h2>
        </div>
        <div class="interest-row">
          <span v-for="interest in interests" :key="interest">{{ interest }}</span>
        </div>
      </section>

      <section id="contact" class="contact-section">
        <div>
          <p class="eyebrow">Contact</p>
          <h2>Open to opportunities connected to guest experience and themed entertainment.</h2>
        </div>
        <div class="contact-links">
          <a href="mailto:marinthelindenburg@gmail.com">marinthelindenburg@gmail.com</a>
          <a href="https://linkedin.com/in/marinthelindenburg" target="_blank" rel="noreferrer">LinkedIn profile</a>
        </div>
      </section>
    </main>

    <footer class="site-footer">
      <div class="footer-inner">
        <a class="footer-brand" href="#top" aria-label="Back to top">
          <img :src="logoUrl" alt="" />
          <span>Marinthe Lindenburg</span>
        </a>
        <p>Guest experience, themed entertainment and hospitality with care.</p>
        <div class="footer-links">
          <a href="mailto:marinthelindenburg@gmail.com">Email</a>
          <a href="https://linkedin.com/in/marinthelindenburg" target="_blank" rel="noreferrer">LinkedIn</a>
        </div>
      </div>
    </footer>
  </div>
</template>

<style>
:root {
  color: #141414;
  background: #ffffff;
  font-family:
    Inter, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
  font-synthesis: none;
  text-rendering: optimizeLegibility;
  --ink: #141414;
  --muted: #646464;
  --line: #eadfe4;
  --pink: #ef9cb7;
  --pink-soft: #fff0f5;
  --turquoise: #19bdb8;
  --turquoise-deep: #087c78;
  --turquoise-soft: #e7fbfa;
  --paper: #ffffff;
  --soft: #fbfafb;
}

* {
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
}

body {
  margin: 0;
  min-width: 320px;
  background:
    linear-gradient(90deg, rgba(239, 156, 183, 0.08) 1px, transparent 1px),
    linear-gradient(180deg, rgba(25, 189, 184, 0.07) 1px, transparent 1px),
    var(--paper);
  background-size: 72px 72px;
}

a {
  color: inherit;
  text-decoration: none;
}

img {
  display: block;
  max-width: 100%;
}

.site-shell {
  min-height: 100vh;
  overflow: hidden;
}

.topbar {
  position: sticky;
  top: 0;
  z-index: 10;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 18px;
  padding: 14px clamp(18px, 5vw, 72px);
  border-bottom: 1px solid rgba(20, 20, 20, 0.08);
  background: rgba(255, 255, 255, 0.9);
  backdrop-filter: blur(18px);
}

.brand,
.nav-links,
.hero-actions,
.contact-links,
.footer-links {
  display: flex;
  align-items: center;
}

.brand {
  min-width: max-content;
  gap: 12px;
  font-weight: 800;
}

.brand-mark {
  display: grid;
  width: 44px;
  height: 44px;
  place-items: center;
  border: 1px solid rgba(20, 20, 20, 0.12);
  background: #fff;
  box-shadow: 8px 8px 0 var(--pink-soft);
}

.brand-mark img {
  width: 34px;
  height: 34px;
  object-fit: contain;
}

.nav-links {
  flex-wrap: wrap;
  justify-content: flex-end;
  gap: 8px;
  color: var(--muted);
  font-size: 0.94rem;
  font-weight: 700;
}

.nav-links a {
  position: relative;
  padding: 9px 10px;
}

.nav-links a::after {
  position: absolute;
  right: 10px;
  bottom: 4px;
  left: 10px;
  height: 2px;
  background: linear-gradient(90deg, var(--pink), var(--turquoise));
  content: "";
  opacity: 0;
  transform: scaleX(0.35);
  transform-origin: left;
  transition: opacity 160ms ease, transform 160ms ease;
}

.nav-links a:hover,
.nav-links a:focus-visible {
  color: var(--ink);
}

.nav-links a:hover::after,
.nav-links a:focus-visible::after {
  opacity: 1;
  transform: scaleX(1);
}

main {
  overflow: hidden;
}

.hero,
.content-section,
.split-section,
.passion-section,
.contact-section,
.footer-inner {
  width: min(1120px, calc(100% - 40px));
  margin: 0 auto;
}

.hero {
  position: relative;
  min-height: calc(100vh - 73px);
  padding: clamp(48px, 7vw, 92px) 0 clamp(42px, 6vw, 72px);
  align-items: center;
}

.hero::before {
  position: absolute;
  top: 42px;
  right: min(34vw, 360px);
  width: 148px;
  height: 148px;
  border-top: 16px solid var(--pink);
  border-left: 16px solid var(--turquoise);
  content: "";
  opacity: 0.38;
  pointer-events: none;
}

.section-grid {
  display: grid;
  grid-template-columns: minmax(0, 0.98fr) minmax(290px, 0.58fr);
  gap: clamp(28px, 6vw, 72px);
}

.hero-copy {
  position: relative;
  max-width: 690px;
}

.eyebrow {
  margin: 0 0 16px;
  color: var(--turquoise-deep);
  font-size: 0.78rem;
  font-weight: 900;
  letter-spacing: 0;
  text-transform: uppercase;
}

h1,
h2,
h3,
p {
  margin-top: 0;
}

h1 {
  max-width: 640px;
  margin-bottom: 22px;
  color: var(--ink);
  font-size: clamp(3rem, 6vw, 5.75rem);
  line-height: 0.98;
  letter-spacing: 0;
}

h2 {
  margin-bottom: 18px;
  color: var(--ink);
  font-size: clamp(2rem, 4vw, 3.45rem);
  line-height: 1.04;
  letter-spacing: 0;
}

h3 {
  margin-bottom: 10px;
  font-size: 1.18rem;
  line-height: 1.25;
}

.hero-text,
.lead {
  max-width: 640px;
  color: #3e3e3e;
  font-size: clamp(1.04rem, 1.7vw, 1.2rem);
  line-height: 1.7;
}

.hero-actions {
  flex-wrap: wrap;
  gap: 12px;
  margin-top: 30px;
}

.button {
  display: inline-flex;
  min-height: 48px;
  align-items: center;
  justify-content: center;
  padding: 0 20px;
  border: 1px solid var(--ink);
  font-weight: 800;
  transition: transform 160ms ease, box-shadow 160ms ease;
}

.button:hover {
  transform: translate(-2px, -2px);
}

.button.primary {
  background: var(--ink);
  box-shadow: 7px 7px 0 var(--turquoise);
  color: #fff;
}

.button.secondary {
  background: var(--paper);
  box-shadow: 7px 7px 0 var(--pink);
}

.portrait-panel {
  position: relative;
  align-self: stretch;
  display: grid;
  align-content: center;
  gap: 18px;
}

.portrait-panel::before {
  position: absolute;
  inset: 32px -18px auto auto;
  width: 86%;
  height: 78%;
  border: 1px solid rgba(25, 189, 184, 0.32);
  content: "";
  pointer-events: none;
}

.portrait-frame {
  position: relative;
  min-height: 500px;
  overflow: hidden;
  border: 1px solid var(--ink);
  background: var(--pink-soft);
  box-shadow: 18px 18px 0 var(--turquoise-soft);
}

.portrait-frame::after {
  position: absolute;
  right: 0;
  bottom: 0;
  width: 42%;
  height: 12px;
  background: linear-gradient(90deg, var(--pink), var(--turquoise));
  content: "";
}

.portrait-frame img {
  width: 100%;
  height: 100%;
  min-height: 500px;
  object-fit: cover;
  object-position: center 18%;
}

.quick-card,
.education-block,
.achievement-card {
  border: 1px solid var(--line);
  background: rgba(255, 255, 255, 0.92);
}

.quick-card {
  position: relative;
  z-index: 1;
  padding: 22px;
  border-color: rgba(20, 20, 20, 0.12);
  box-shadow: 0 18px 45px rgba(20, 20, 20, 0.08);
}

.quick-label {
  margin-bottom: 8px;
  color: var(--turquoise-deep);
  font-size: 0.78rem;
  font-weight: 900;
  text-transform: uppercase;
}

.quick-card p:last-child,
.education-block p:last-child,
.achievement-card p:last-child,
.passion-section p:last-child,
.site-footer p {
  margin-bottom: 0;
}

.content-section {
  padding: clamp(62px, 8vw, 108px) 0;
}

.section-heading {
  max-width: 790px;
  margin-bottom: 34px;
}

.section-heading.narrow {
  max-width: 720px;
}

.profile-layout {
  display: grid;
  grid-template-columns: minmax(0, 1fr) minmax(260px, 0.58fr);
  gap: clamp(28px, 5vw, 64px);
  align-items: start;
}

.highlight-list {
  display: grid;
  gap: 14px;
}

.highlight-item {
  display: grid;
  grid-template-columns: 14px 1fr;
  gap: 14px;
  align-items: start;
  padding: 14px;
  border-left: 4px solid var(--turquoise);
  background: var(--turquoise-soft);
}

.highlight-item:nth-child(2) {
  border-left-color: var(--pink);
  background: var(--pink-soft);
}

.highlight-item:nth-child(3) {
  border-left-color: var(--ink);
  background: #fff;
}

.highlight-item span {
  width: 12px;
  height: 12px;
  margin-top: 7px;
  background: var(--turquoise);
}

.highlight-item:nth-child(2) span {
  background: var(--pink);
}

.highlight-item:nth-child(3) span {
  background: var(--ink);
}

.highlight-item p {
  margin: 0;
  color: #333;
  line-height: 1.6;
}

.split-section {
  display: grid;
  grid-template-columns: minmax(0, 1fr) minmax(260px, 0.45fr);
  gap: 22px;
  padding: 34px 0;
}

.education-block {
  position: relative;
  padding: clamp(26px, 4vw, 42px);
  overflow: hidden;
}

.education-block::after {
  position: absolute;
  right: 24px;
  bottom: 24px;
  width: 72px;
  height: 72px;
  border-right: 10px solid rgba(25, 189, 184, 0.28);
  border-bottom: 10px solid rgba(239, 156, 183, 0.32);
  content: "";
}

.education-block:first-child {
  background: var(--pink-soft);
}

.education-block.compact {
  background: var(--turquoise-soft);
}

.muted,
.company,
.timeline-meta p {
  color: var(--muted);
}

.experience-section {
  position: relative;
}

.timeline {
  display: grid;
  gap: 0;
  border-top: 1px solid var(--line);
}

.timeline-item {
  position: relative;
  display: grid;
  grid-template-columns: 230px minmax(0, 1fr);
  gap: 34px;
  padding: 34px 0 34px 28px;
  border-bottom: 1px solid var(--line);
}

.timeline-item::before {
  position: absolute;
  top: 40px;
  left: 0;
  width: 11px;
  height: 34px;
  background: var(--turquoise);
  content: "";
}

.timeline-item:nth-child(even)::before {
  background: var(--pink);
}

.timeline-meta p {
  margin: 0;
  font-weight: 800;
}

.timeline-content ul {
  margin: 18px 0 0;
  padding-left: 20px;
  color: #3e3e3e;
  line-height: 1.7;
}

.timeline-content li::marker {
  color: var(--turquoise-deep);
}

.achievement-grid {
  display: grid;
  grid-template-columns: repeat(4, minmax(0, 1fr));
  gap: 16px;
}

.achievement-card {
  min-height: 210px;
  padding: 24px;
  box-shadow: 0 16px 34px rgba(20, 20, 20, 0.05);
}

.achievement-card:nth-child(2),
.achievement-card:nth-child(3) {
  background: var(--soft);
}

.achievement-card:nth-child(1) {
  border-top: 5px solid var(--pink);
}

.achievement-card:nth-child(2) {
  border-top: 5px solid var(--turquoise);
}

.achievement-card:nth-child(3) {
  border-top: 5px solid var(--ink);
}

.achievement-card:nth-child(4) {
  border-top: 5px solid var(--pink);
}

.achievement-card p {
  color: #4d4d4d;
  line-height: 1.6;
}

.achievement-meta {
  margin-bottom: 12px;
  color: var(--turquoise-deep);
  font-weight: 900;
}

.achievement-card ul,
.passion-list {
  margin: 0;
  padding-left: 19px;
  color: #4d4d4d;
  line-height: 1.62;
}

.achievement-card li + li,
.passion-list li + li {
  margin-top: 7px;
}

.achievement-card li::marker {
  color: var(--turquoise-deep);
}

.skills-section {
  position: relative;
  border-top: 1px solid var(--line);
  border-bottom: 1px solid var(--line);
  background: linear-gradient(135deg, rgba(255, 240, 245, 0.72), rgba(231, 251, 250, 0.62));
}

.skill-cloud,
.interest-row {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
}

.skill-cloud span,
.interest-row span {
  border: 1px solid rgba(20, 20, 20, 0.14);
  padding: 10px 14px;
  background: #fff;
  color: #292929;
  font-weight: 800;
}

.skill-cloud span:nth-child(3n + 1),
.interest-row span:nth-child(odd) {
  background: var(--pink-soft);
}

.skill-cloud span:nth-child(3n + 2),
.interest-row span:nth-child(even) {
  background: var(--turquoise-soft);
}

.passion-section {
  position: relative;
  display: grid;
  grid-template-columns: minmax(0, 0.8fr) minmax(0, 1fr);
  gap: clamp(28px, 6vw, 72px);
  padding: clamp(58px, 8vw, 96px) clamp(24px, 5vw, 56px);
  overflow: hidden;
  background:
    linear-gradient(135deg, rgba(239, 156, 183, 0.15), transparent 28%),
    linear-gradient(315deg, rgba(25, 189, 184, 0.22), transparent 35%),
    #111;
  color: #fff;
}

.passion-section::after {
  position: absolute;
  right: 28px;
  bottom: 28px;
  width: 180px;
  height: 80px;
  border-right: 1px solid rgba(255, 255, 255, 0.26);
  border-bottom: 1px solid rgba(255, 255, 255, 0.26);
  content: "";
}

.passion-section .eyebrow {
  color: var(--turquoise);
}

.passion-section h2 {
  color: #fff;
}

.passion-section p {
  color: rgba(255, 255, 255, 0.84);
  font-size: 1.05rem;
  line-height: 1.8;
}

.passion-list {
  color: rgba(255, 255, 255, 0.86);
  font-size: 1.05rem;
  line-height: 1.75;
}

.passion-list li::marker {
  color: var(--turquoise);
}

.contact-section {
  display: grid;
  grid-template-columns: minmax(0, 1fr) minmax(260px, auto);
  gap: 32px;
  align-items: end;
  padding: clamp(56px, 8vw, 90px) 0;
  border-top: 1px solid var(--line);
}

.contact-links {
  flex-direction: column;
  align-items: flex-start;
  gap: 10px;
  max-width: 100%;
  font-weight: 900;
}

.contact-links a {
  max-width: 100%;
  overflow-wrap: anywhere;
  border-bottom: 2px solid var(--turquoise);
}

.contact-links a:hover,
.footer-links a:hover {
  color: var(--turquoise-deep);
}

.site-footer {
  margin-top: 12px;
  padding: 30px 0;
  border-top: 1px solid var(--line);
  background: #fff;
}

.footer-inner {
  display: grid;
  grid-template-columns: minmax(210px, 0.8fr) minmax(0, 1fr) auto;
  gap: 24px;
  align-items: center;
}

.footer-brand {
  display: flex;
  align-items: center;
  gap: 12px;
  font-weight: 900;
}

.footer-brand img {
  width: 38px;
  height: 38px;
  object-fit: contain;
}

.site-footer p {
  color: var(--muted);
  line-height: 1.5;
}

.footer-links {
  flex-wrap: wrap;
  justify-content: flex-end;
  gap: 14px;
  font-weight: 900;
}

.footer-links a {
  border-bottom: 2px solid var(--pink);
}

@media (max-width: 980px) {
  .topbar {
    align-items: flex-start;
    flex-direction: column;
  }

  .nav-links {
    width: 100%;
    justify-content: flex-start;
  }

  .section-grid,
  .profile-layout,
  .split-section,
  .passion-section,
  .contact-section,
  .footer-inner {
    grid-template-columns: 1fr;
  }

  .hero {
    min-height: auto;
  }

  .hero::before {
    top: 26px;
    right: 16px;
    width: 92px;
    height: 92px;
    border-width: 10px;
  }

  .portrait-panel {
    max-width: 520px;
  }

  .portrait-frame,
  .portrait-frame img {
    min-height: 420px;
  }

  .achievement-grid {
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }

  .contact-section,
  .footer-inner {
    align-items: start;
  }

  .footer-links {
    justify-content: flex-start;
  }
}

@media (max-width: 640px) {
  .topbar {
    padding: 14px 16px;
  }

  .brand {
    white-space: normal;
  }

  .brand-mark {
    width: 40px;
    height: 40px;
    box-shadow: 5px 5px 0 var(--pink-soft);
  }

  .brand-mark img {
    width: 30px;
    height: 30px;
  }

  .nav-links {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 6px;
    font-size: 0.88rem;
  }

  .nav-links a {
    min-height: 38px;
    padding: 9px 8px;
    border: 1px solid rgba(20, 20, 20, 0.08);
    background: rgba(255, 255, 255, 0.74);
    text-align: center;
  }

  .hero,
  .content-section,
  .split-section,
  .passion-section,
  .contact-section,
  .footer-inner {
    width: min(100% - 32px, 1120px);
  }

  .hero {
    padding-top: 42px;
  }

  h1 {
    font-size: 2.8rem;
    line-height: 1;
  }

  h2 {
    font-size: 2.05rem;
  }

  .hero-text,
  .lead,
  .passion-section p {
    font-size: 1rem;
  }

  .portrait-panel::before {
    display: none;
  }

  .portrait-frame,
  .portrait-frame img {
    min-height: 380px;
  }

  .timeline-item {
    grid-template-columns: 1fr;
    gap: 12px;
    padding-left: 22px;
  }

  .achievement-grid {
    grid-template-columns: 1fr;
  }

  .button {
    width: 100%;
  }

  .skill-cloud span,
  .interest-row span {
    max-width: 100%;
    overflow-wrap: anywhere;
  }
}

@media (max-width: 420px) {
  h1 {
    font-size: 2.35rem;
  }

  h2 {
    font-size: 1.82rem;
  }

  .portrait-frame,
  .portrait-frame img {
    min-height: 330px;
  }
}
</style>

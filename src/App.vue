<script setup>
import { computed, ref } from 'vue'

const currentLang = ref('tr')

const setLang = (lang) => {
  currentLang.value = lang
}

const formAction = 'https://formsubmit.co/hazalgelenbey@gmail.com'
const siteUrl = 'https://portfolyo-7319bxtqr-hazalgelenbeys-projects.vercel.app/'

const translations = {
  tr: {
    brand: 'Hazal Gelenbey',
    status: 'Frontend developer portfolio • yeni fırsatlara açığım',
    profile: {
      name: 'Hazal Gelenbey',
      title: 'Frontend Developer',
      tagline: 'Building real products, not just interfaces.',
      summary:
        'Vue.js ve Flutter ile kullanıcı odaklı, ölçeklenebilir ve gerçek kullanıcılar tarafından aktif olarak kullanılan ürünler geliştiriyorum.',
      summary2:
        'App Store’da yayında olan mobil uygulama geliştirme deneyimimle, sadece kod değil değer üreten çözümler üretiyorum.',
      location: 'Türkiye',
      company: 'Worknitive',
      availability: 'Full-time • Remote • Hybrid',
      email: 'hazalgelenbey@gmail.com',
      linkedin: 'https://www.linkedin.com/in/hazalgelenbey/',
      github: 'https://github.com/hazalgelenbey',
      cvFile: '/HAZALGELENBEY2026.pdf'
    },
    actions: {
      contact: 'İletişime Geç',
      cv: 'CV İndir',
      linkedin: 'LinkedIn',
      github: 'GitHub'
    },
    metrics: [
      { label: 'Ana alan', value: 'Frontend' },
      { label: 'Ek katkı', value: 'Mobile + Backend' },
      { label: 'Ürün deneyimi', value: 'Live Apps' }
    ],
    aboutTitle: 'Hakkımda',
    aboutLead: 'Kullanıcı deneyimi ve ürün etkisi odaklı yaklaşımım',
    aboutParagraphs: [
      'Frontend ve mobil geliştirme alanında, kullanıcı deneyimini merkeze alarak çalışan bir geliştiriciyim. Vue.js ve Flutter ile modern, performanslı ve sürdürülebilir ürünler geliştiriyorum.',
      'Şu anda Worknitive bünyesinde, gerçek kullanıcılar tarafından kullanılan bir ürünün hem web hem mobil tarafında aktif rol alıyorum. App Store’da yayında olan mobil uygulamanın geliştirme sürecinde yer alarak, üretim ortamında çalışmanın getirdiği performans, ölçeklenebilirlik ve kullanıcı deneyimi gibi kritik konularda deneyim kazandım.',
      'Amacım sadece görevleri tamamlamak değil, ürünün gerçek hayattaki etkisini artıran çözümler geliştirmek.'
    ],
    highlightsTitle: 'Beni öne çıkaran noktalar',
    highlightsLead: 'Sadece teknik değil, ürün tarafında da güçlü katkı',
    highlights: [
      {
        title: 'Çok yönlü geliştirme',
        text: 'Frontend, mobil ve backend süreçlerini birlikte ele alarak uçtan uca ürün geliştirme bakış açısıyla çalışıyorum.'
      },
      {
        title: 'Gerçek ürün deneyimi',
        text: 'App Store’da yayında olan ve aktif kullanılan bir mobil uygulamanın geliştirilmesinde aktif rol aldım.'
      },
      {
        title: 'Ürün odaklı yaklaşım',
        text: 'Sadece teknik olarak doğru değil, kullanıcı için gerçekten değer üreten çözümler geliştirmeye odaklanıyorum.'
      }
    ],
    experienceTitle: 'Deneyim',
    experienceLead: 'Web, mobil ve ürün geliştirme deneyimim',
    experiences: [
      {
        period: '2025 – Devam ediyor',
        role: 'Frontend & Mobile Developer',
        company: 'Worknitive',
        details:
          'Üretim ortamında kullanılan web ve mobil uygulamaların geliştirilmesinde aktif rol alıyorum. Vue.js ile dinamik ve performanslı arayüzler geliştirirken, Flutter ile App Store’da yayında olan mobil uygulamanın geliştirme süreçlerinde yer aldım. Backend tarafında Django ile API entegrasyonları yaparak veri akışını yönettim, kullanıcı akışlarını iyileştirdim ve performans optimizasyonları gerçekleştirdim. Canlı sistemlerde hata yönetimi, sürüm süreçleri ve kullanıcı deneyimi iyileştirmeleri üzerine çalışıyorum.'
      },
      {
        period: 'Mart 2025 – Haziran 2025',
        role: 'Frontend Developer Intern',
        company: 'GRICREATIVE',
        details:
          'Kurumsal projelerde arayüz geliştirme süreçlerine katkı sağladım. HTML, CSS ve JavaScript kullanarak responsive ve kullanıcı dostu arayüzler geliştirdim. UI/UX iyileştirmeleri yaparak kullanıcı etkileşimini artırmaya yönelik çalışmalar yaptım.'
      },
      {
        period: '2022 – 2023',
        role: 'Intern',
        company: 'Sosyopix',
        details:
          'Modern web teknolojileri ile tanışarak frontend geliştirme temelleri kazandım. Takım çalışması, kod düzeni ve geliştirme süreçleri konusunda pratik deneyim elde ettim.'
      }
    ],
    projectsTitle: 'Öne çıkan proje',
    projectsLead: 'Gerçek kullanıcıya ulaşmış ürün deneyimi',
    projects: [
      {
        title: 'Worknitive iOS App',
        subtitle: 'App Store’da yayında canlı ürün',
        description:
          'Flutter ile geliştirilen ve aktif olarak kullanılan mobil ürünün geliştirme süreçlerinde yer aldım. Arayüz iyileştirmeleri, kullanıcı akışları, hata düzeltmeleri ve ürün deneyimini güçlendiren geliştirmeler üzerinde çalıştım.',
        stack: 'Flutter • REST API • Firebase • Product Thinking',
        link: 'https://apps.apple.com/tr/app/worknitive/id6759917958?l=tr',
        linkLabel: 'App Store’da Gör'
      }
    ],
    focusTitle: 'Katkı sağlayabildiğim alanlar',
    focusLead: 'Tek bir role sıkışmadan değer üretme yaklaşımı',
    focusAreas: [
      {
        title: 'Frontend Development',
        text: 'Temiz arayüzler, akıcı kullanıcı deneyimi ve bileşen bazlı geliştirme.'
      },
      {
        title: 'Mobile Development',
        text: 'Flutter ile performanslı ve üretime uygun mobil uygulamalar geliştirme.'
      },
      {
        title: 'Backend Awareness',
        text: 'REST API, veri akışı ve servis iletişimini anlayarak daha doğru ürün kararları alma.'
      }
    ],
    skillsTitle: 'Teknoloji seti',
    skillsLead: 'Günlük iş akışımda kullandığım başlıklar',
    skills: [
      'Vue',
      'Flutter',
      'Dart',
      'JavaScript',
      'HTML/CSS',
      'REST API',
      'Firebase',
      'State Management',
      'Git',
      'Agile/Scrum'
    ],
    educationTitle: 'Eğitim & çalışma yaklaşımı',
    education: [
      {
        title: 'Erken mezuniyet',
        text: 'Hedefe odaklı ilerleyip eğitim sürecimi planlı şekilde erkenden tamamladım.'
      },
      {
        title: 'Sorumluluk alma',
        text: 'Yeni konuları hızlı öğrenip ihtiyaç olan yerde inisiyatif almayı seviyorum.'
      }
    ],
    contactTitle: 'Birlikte çalışalım',
    contactText:
      'Yeni bir ekipte frontend, mobile ya da ürün odaklı bir rolde hızlıca değer üretmeye hazırım.',
    form: {
      name: 'Ad Soyad',
      email: 'E-posta',
      message: 'Mesaj',
      send: 'Mesaj Gönder',
      note: 'Form doldurulduğunda mesaj doğrudan e-posta kutuma düşer.'
    }
  },
  en: {
    brand: 'Hazal Gelenbey',
    status: 'Frontend developer portfolio • open to new opportunities',
    profile: {
      name: 'Hazal Gelenbey',
      title: 'Frontend Developer',
      tagline: 'Building real products, not just interfaces.',
      summary:
        'I build user-focused, scalable products with Vue.js and Flutter that are actively used by real users.',
      summary2:
        'With experience contributing to a mobile app published on the App Store, I aim to create solutions that deliver real value, not just code.',
      location: 'Turkey',
      company: 'Worknitive',
      availability: 'Full-time • Remote • Hybrid',
      email: 'hazalgelenbey@gmail.com',
      linkedin: 'https://www.linkedin.com/in/hazalgelenbey/',
      github: 'https://github.com/hazalgelenbey',
      cvFile: '/HAZALGELENBEY2026.pdf'
    },
    actions: {
      contact: 'Contact Me',
      cv: 'Download CV',
      linkedin: 'LinkedIn',
      github: 'GitHub'
    },
    metrics: [
      { label: 'Primary focus', value: 'Frontend' },
      { label: 'Extra scope', value: 'Mobile + Backend' },
      { label: 'Product experience', value: 'Live Apps' }
    ],
    aboutTitle: 'About',
    aboutLead: 'My approach to product and user experience',
    aboutParagraphs: [
      'I am a developer working across frontend and mobile with a strong focus on user experience. I build modern, performant, and maintainable products using Vue.js and Flutter.',
      'At Worknitive, I actively contribute to both the web and mobile sides of a real product used by actual users. Being part of an App Store release helped me gain hands-on experience in performance, scalability, and production-grade user experience.',
      'My goal is not only to complete tasks, but to build solutions that improve the real-life impact of the product.'
    ],
    highlightsTitle: 'What makes me stand out',
    highlightsLead: 'Strong contribution beyond just technical output',
    highlights: [
      {
        title: 'Versatile development',
        text: 'I approach frontend, mobile, and backend-related flows with an end-to-end product mindset.'
      },
      {
        title: 'Real product experience',
        text: 'I actively contributed to the development of a live and actively used mobile application on the App Store.'
      },
      {
        title: 'Product-oriented mindset',
        text: 'I focus on solutions that create real value for users, not only technically correct implementations.'
      }
    ],
    experienceTitle: 'Experience',
    experienceLead: 'My web, mobile, and product development background',
    experiences: [
      {
        period: '2025 – Present',
        role: 'Frontend & Mobile Developer',
        company: 'Worknitive',
        details:
          'I actively contribute to the development of production web and mobile applications. I build dynamic and performant interfaces with Vue.js, while also taking part in the Flutter development process of a mobile app published on the App Store. I work with Django-based API integrations, improve user flows, and perform performance optimizations for live systems.'
      },
      {
        period: 'March 2025 – June 2025',
        role: 'Frontend Developer Intern',
        company: 'GRICREATIVE',
        details:
          'I supported interface development for corporate projects. Using HTML, CSS, and JavaScript, I built responsive and user-friendly interfaces and contributed to UI/UX improvements.'
      },
      {
        period: '2022 – 2023',
        role: 'Intern',
        company: 'Sosyopix',
        details:
          'I gained my frontend foundations through hands-on exposure to modern web technologies, teamwork, code organization, and development processes.'
      }
    ],
    projectsTitle: 'Featured project',
    projectsLead: 'Experience on a live product used by real users',
    projects: [
      {
        title: 'Worknitive iOS App',
        subtitle: 'Live product published on the App Store',
        description:
          'I took part in the development process of an actively used mobile product built with Flutter. I worked on interface improvements, user flows, bug fixing, and product enhancements that improved the overall user experience.',
        stack: 'Flutter • REST API • Firebase • Product Thinking',
        link: 'https://apps.apple.com/tr/app/worknitive/id6759917958?l=tr',
        linkLabel: 'View on App Store'
      }
    ],
    focusTitle: 'Where I add value',
    focusLead: 'A flexible approach beyond a single title',
    focusAreas: [
      {
        title: 'Frontend Development',
        text: 'Clean interfaces, smooth user journeys, and component-based implementation.'
      },
      {
        title: 'Mobile Development',
        text: 'Production-ready Flutter apps with a focus on performance and maintainability.'
      },
      {
        title: 'Backend Awareness',
        text: 'Understanding API flows and service communication to build better product decisions.'
      }
    ],
    skillsTitle: 'Tech stack',
    skillsLead: 'Core tools I use in day-to-day work',
    skills: [
      'Vue',
      'Flutter',
      'Dart',
      'JavaScript',
      'HTML/CSS',
      'REST API',
      'Firebase',
      'State Management',
      'Git',
      'Agile/Scrum'
    ],
    educationTitle: 'Education & work style',
    educationLead: 'Making your strong CV signals visible',
    education: [
      {
        title: 'Early graduation',
        text: 'I completed my education early through a focused and disciplined path.'
      },
      {
        title: 'Ownership mindset',
        text: 'I enjoy learning quickly and stepping in where the team needs support.'
      }
    ],
    contactTitle: 'Let’s work together',
    contactText:
      'I am ready to contribute quickly in a frontend, mobile, or product-focused role within a new team.',
    form: {
      name: 'Full Name',
      email: 'Email',
      message: 'Message',
      send: 'Send Message',
      note: 'Messages sent from this form are delivered directly to my email inbox.'
    }
  }
}

const content = computed(() => translations[currentLang.value])
</script>

<template>
  <main class="page">
    <header class="topbar">
      <p class="brand">{{ content.brand }}</p>
      <div class="lang-switch" aria-label="Language switcher">
        <button
          class="lang-btn"
          :class="{ active: currentLang === 'tr' }"
          @click="setLang('tr')"
        >
          TR
        </button>
        <button
          class="lang-btn"
          :class="{ active: currentLang === 'en' }"
          @click="setLang('en')"
        >
          EN
        </button>
      </div>
    </header>

    <section class="hero">
      <p class="eyebrow">{{ content.status }}</p>
      <h1>
        {{ content.profile.name }}
        <span>{{ content.profile.title }}</span>
      </h1>
      <p class="tagline">{{ content.profile.tagline }}</p>
      <p class="intro">{{ content.profile.summary }}</p>
      <p class="intro intro-soft">{{ content.profile.summary2 }}</p>
      <div class="hero-actions">
        <a class="btn btn-primary" :href="`mailto:${content.profile.email}`">{{ content.actions.contact }}</a>
        <a class="btn btn-ghost" :href="content.profile.cvFile" target="_blank" download="Hazal-Gelenbey-CV.pdf">{{ content.actions.cv }}</a>
        <a class="btn btn-ghost" :href="content.profile.linkedin" target="_blank" rel="noreferrer">
          {{ content.actions.linkedin }}
        </a>
      </div>
      <p class="meta">{{ content.profile.location }} • {{ content.profile.availability }}</p>
    </section>

    <section class="metrics">
      <article v-for="item in content.metrics" :key="item.label" class="metric-card">
        <p class="metric-value">{{ item.value }}</p>
        <p class="metric-label">{{ item.label }}</p>
      </article>
    </section>

    <section class="block">
      <div class="block-head">
        <h2>{{ content.aboutTitle }}</h2>
        <p>{{ content.aboutLead }}</p>
      </div>
      <div class="about-copy">
        <p v-for="paragraph in content.aboutParagraphs" :key="paragraph" class="about-paragraph">
          {{ paragraph }}
        </p>
      </div>
    </section>

    <section class="block">
      <div class="block-head">
        <h2>{{ content.highlightsTitle }}</h2>
        <p>{{ content.highlightsLead }}</p>
      </div>
      <div class="card-grid">
        <article v-for="item in content.highlights" :key="item.title" class="info-card">
          <h3>{{ item.title }}</h3>
          <p>{{ item.text }}</p>
        </article>
      </div>
    </section>

    <section class="block">
      <div class="block-head">
        <h2>{{ content.experienceTitle }}</h2>
        <p>{{ content.experienceLead }}</p>
      </div>
      <article
        v-for="exp in content.experiences"
        :key="`${exp.role}-${exp.company}`"
        class="timeline-item"
      >
        <p class="period">{{ exp.period }}</p>
        <h3>{{ exp.role }} • {{ exp.company }}</h3>
        <p>{{ exp.details }}</p>
      </article>
    </section>

    <section class="block">
      <div class="block-head">
        <h2>{{ content.projectsTitle }}</h2>
        <p>{{ content.projectsLead }}</p>
      </div>
      <div class="project-list">
        <article v-for="project in content.projects" :key="project.title" class="project-card">
          <div class="project-top">
            <div>
              <h3>{{ project.title }}</h3>
              <p class="project-subtitle">{{ project.subtitle }}</p>
            </div>
            <a class="btn btn-ghost" :href="project.link" target="_blank" rel="noreferrer">
              {{ project.linkLabel }}
            </a>
          </div>
          <p class="project-description">{{ project.description }}</p>
          <p class="project-stack">{{ project.stack }}</p>
        </article>
      </div>
    </section>

    <section class="block">
      <div class="block-head">
        <h2>{{ content.focusTitle }}</h2>
        <p>{{ content.focusLead }}</p>
      </div>
      <div class="card-grid">
        <article v-for="item in content.focusAreas" :key="item.title" class="info-card">
          <h3>{{ item.title }}</h3>
          <p>{{ item.text }}</p>
        </article>
      </div>
    </section>

    <section class="block">
      <div class="block-head">
        <h2>{{ content.skillsTitle }}</h2>
        <p>{{ content.skillsLead }}</p>
      </div>
      <ul class="skills">
        <li v-for="skill in content.skills" :key="skill">{{ skill }}</li>
      </ul>
    </section>

    <section class="block">
      <div class="block-head">
        <h2>{{ content.educationTitle }}</h2>
        <p>{{ content.educationLead }}</p>
      </div>
      <div class="card-grid">
        <article v-for="item in content.education" :key="item.title" class="info-card">
          <h3>{{ item.title }}</h3>
          <p>{{ item.text }}</p>
        </article>
      </div>
    </section>

    <section class="contact">
      <h2>{{ content.contactTitle }}</h2>
      <p>{{ content.contactText }}</p>
      <form class="contact-form" :action="formAction" method="POST">
        <input type="hidden" name="_subject" :value="`${content.profile.name} Portfolio Contact Form`" />
        <input type="hidden" name="_captcha" value="false" />
        <input type="hidden" name="_next" :value="siteUrl" />

        <label>
          <span>{{ content.form.name }}</span>
          <input type="text" name="name" required />
        </label>

        <label>
          <span>{{ content.form.email }}</span>
          <input type="email" name="email" required />
        </label>

        <label>
          <span>{{ content.form.message }}</span>
          <textarea name="message" rows="5" required></textarea>
        </label>

        <div class="form-actions">
          <button class="btn btn-primary" type="submit">{{ content.form.send }}</button>
          <a class="btn btn-ghost" :href="content.profile.github" target="_blank" rel="noreferrer">{{ content.actions.github }}</a>
        </div>
      </form>
      <p class="form-note">{{ content.form.note }}</p>
    </section>
  </main>
</template>

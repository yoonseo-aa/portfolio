<template>
  <main class="portfolio">
    <section class="hero">
      <p class="label">Frontend Developer Portfolio</p>
      <h1>안녕하세요, 성장하는 개발자 이윤서입니다.</h1>
      <p>
        Vue와 JavaScript를 중심으로 사용자 경험을 고려한 웹 서비스를 개발합니다.
      </p>
      <div class="buttons">
        <a href="#projects">프로젝트 보기</a>
        <a href="https://github.com/깃허브아이디" target="_blank">GitHub</a>
      </div>
    </section>

    <section class="section">
      <h2>About Me</h2>
      <p>
        프론트엔드 개발을 중심으로 학습하고 있으며, 프로젝트 과정에서 문제를 발견하고
        해결하는 경험을 중요하게 생각합니다.
      </p>
    </section>

    <section class="section">
      <h2>Skills</h2>
      <div class="skills">
        <span>HTML</span>
        <span>CSS</span>
        <span>JavaScript</span>
        <span>Vue</span>
        <span>Vite</span>
        <span>Git</span>
        <span>GitHub</span>
      </div>
    </section>

    <section id="projects" class="section">
      <h2>Projects</h2>

      <article class="project-card">
        <h3>문화유산 AI 해설 서비스</h3>
        <p>
          사용자 유형에 따라 문화유산을 다르게 해설하고, 퀴즈와 탐험 미션으로 학습을 돕는
          AI 기반 서비스입니다.
        </p>
        <ul>
          <li>Vue 기반 모바일 웹 UI 구현</li>
          <li>사용자 모드별 화면 구성</li>
          <li>기획안 발표용 UI 디자인 정리</li>
        </ul>
        <p class="tech">Vue · Django · AI API · Figma</p>
      </article>
    </section>

    <section class="section">
      <h2>Contact</h2>
      <p>Email: 본인이메일@example.com</p>
      <p>GitHub: github.com/깃허브아이디</p>
    </section>
  </main>
</template>

<style scoped>
.portfolio {
  max-width: 960px;
  margin: 0 auto;
  padding: 60px 24px;
  color: #1f2937;
}

.hero {
  padding: 80px 0;
}

.label {
  color: #2563eb;
  font-weight: 700;
}

.hero h1 {
  font-size: 42px;
  line-height: 1.3;
  margin: 16px 0;
}

.hero p {
  font-size: 18px;
  color: #4b5563;
}

.buttons {
  display: flex;
  gap: 12px;
  margin-top: 28px;
}

.buttons a {
  padding: 12px 18px;
  border-radius: 10px;
  background: #111827;
  color: white;
  text-decoration: none;
}

.buttons a:last-child {
  background: #e5e7eb;
  color: #111827;
}

.section {
  margin: 72px 0;
}

.section h2 {
  font-size: 28px;
  margin-bottom: 20px;
}

.skills {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
}

.skills span {
  padding: 10px 14px;
  border-radius: 999px;
  background: #f3f4f6;
  font-weight: 600;
}

.project-card {
  padding: 28px;
  border: 1px solid #e5e7eb;
  border-radius: 18px;
  background: white;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.05);
}

.project-card h3 {
  font-size: 22px;
}

.project-card li {
  margin: 8px 0;
}

.tech {
  margin-top: 16px;
  color: #2563eb;
  font-weight: 700;
}
</style>
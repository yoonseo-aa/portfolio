<script setup lang="ts">
import heroImage from './assets/hero.png'

const aiWorkflow = [
  {
    phase: '개발 전',
    title: '요구사항 정리와 작업 범위 구체화',
    points: [
      '기능 요구사항을 사용자 흐름, 화면 단위, 데이터 흐름으로 나누어 정리합니다.',
      'AI를 활용해 놓치기 쉬운 예외 상황과 필요한 검증 항목을 먼저 점검합니다.',
      '구현 전에 작업 범위를 좁혀 불필요한 수정과 재작업을 줄이는 데 집중합니다.',
    ],
  },
  {
    phase: '개발 중',
    title: '구현 속도와 검증 품질 개선',
    points: [
      '반복되는 UI 구조나 유틸 로직의 초안을 빠르게 만들고, 프로젝트 코드 스타일에 맞게 수정합니다.',
      '작성한 코드의 조건문, 상태 처리, API 연동 흐름을 다시 검토해 오류 가능성을 줄입니다.',
      'AI 결과를 그대로 사용하지 않고 요구사항, 실제 화면, 빌드 결과를 기준으로 교차 확인합니다.',
    ],
  },
]

const careers = [
  {
    company: '(주) 아이디',
    role: '소프트웨어 개발자',
    period: '2023.12 - 2025.04',
    points: [
      '자사 사이트와 관공서 웹 시스템의 운영 안정화 및 기능 개선을 담당했습니다.',
      'Webpack 개선, 중복 코드 제거, 모듈화를 통해 레거시 코드를 정리했습니다.',
      '사용자 요구사항에 맞춘 기능 최적화와 커스텀 로직을 개발했습니다.',
      'MySQL 데이터베이스 유지보수와 데이터 관리 업무를 수행했습니다.',
      '코드 리뷰와 기술 스터디를 통해 팀 내 협업 역량을 높였습니다.',
    ],
  },
  {
    company: '(주)유니컴퍼니',
    role: '프론트엔드',
    period: '2022.08 - 2023.03',
    points: [
      'ERP 연동 바코드 기반 통합 생산 및 물류 관리 시스템(MES/WMS)을 구축했습니다.',
      '데이터 수집, 정제, 라벨링을 통해 서비스 운영에 필요한 데이터베이스를 구축했습니다.',
    ],
  },
]

const certificates = [
  {
    name: '정보처리산업기사',
    status: '최종합격',
    date: '2025.09',
    issuer: '한국산업인력공단',
    number: '25202221030A',
  },
  {
    name: '정보처리기사',
    status: '필기합격',
    date: '2025.06',
    issuer: '한국산업인력공단',
  },
  {
    name: 'SQL개발자(SQLD)',
    status: '자격 취득',
    date: '2025.06',
    issuer: '한국데이터베이스진흥센터',
    number: 'SQLD-057017976',
  },
]

const skills = [
  {
    name: 'React',
    items: [
      '함수형 컴포넌트 기반 UI 개발이 가능합니다.',
      'Custom Hooks로 공통 로직을 분리해 유지보수성을 높일 수 있습니다.',
    ],
  },
  {
    name: 'Vue.js',
    items: [
      '컴포넌트 기반 구조와 SPA 개발 흐름을 이해하고 있습니다.',
      'Axios를 활용한 API 연동과 비동기 데이터 처리를 경험했습니다.',
    ],
  },
  {
    name: 'TypeScript & JavaScript',
    items: [
      'ES6 문법을 이해하고 실무 코드에 활용합니다.',
      'TypeScript로 예기치 못한 타입 오류를 줄이며 안정적인 코드를 작성합니다.',
    ],
  },
  {
    name: 'MySQL',
    items: [
      '데이터베이스 설계와 쿼리 최적화를 통해 조회 성능을 개선한 경험이 있습니다.',
      '운영 중인 서비스의 데이터 유지보수와 관리 업무를 수행했습니다.',
    ],
  },
  {
    name: 'HTML & CSS',
    items: [
      '시맨틱 HTML과 기본 태그를 활용해 화면 구조를 설계합니다.',
      'keyframes, rem, grid를 활용한 애니메이션과 반응형 웹 개발 경험이 있습니다.',
    ],
  },
  {
    name: 'Git & GitHub',
    items: [
      'Git으로 프로젝트 버전을 관리하고 협업 흐름을 정리합니다.',
      '코드 리뷰와 Git-flow 기반 협업 방식에 익숙합니다.',
    ],
  },
  {
    name: 'ETC',
    items: [
      'Axios interceptor로 공통 작업을 처리해 중복 코드를 줄인 경험이 있습니다.',
      'Emotion의 css prop을 활용해 재사용성 높은 컴포넌트를 만들 수 있습니다.',
    ],
  },
]

const projects = [
  {
    name: '이음',
    type: 'Team · Frontend Developer',
    period: '2025.06.28 - 서비스 종료',
    summary:
      '경력 있는 시니어(5070대)와 레슨이 필요한 MZ세대(2030대)를 연결하는 매칭 플랫폼입니다. 실무 경험이 풍부한 시니어가 회계, 마케팅, 음악 등 전문 분야를 바탕으로 맞춤형 수업을 제공할 수 있도록 기획했습니다.',
    contribution: '기여도 50%',
    points: [
      'React 기반 반응형 웹페이지를 제작했습니다.',
      '다양한 UI 패턴을 구현하고 A/B 테스트 기반으로 UI를 개선했습니다.',
      '공통 페이징 컴포넌트를 분리해 유지보수성과 재사용성을 높였습니다.',
      'React Hook Form으로 form 상태 관리와 validation을 구현했습니다.',
      'FormData 기반 파일 업로드 처리와 사용자 피드백을 구현했습니다.',
    ],
    stack: ['React', 'React Hook Form', 'FormData', 'Responsive UI'],
  },
  {
    name: 'MES / WMS',
    type: '(주)유니컴퍼니 · Team',
    period: '2022.08 - 2023.03',
    summary:
      'ERP와 연동해 입고, 출고, 생산계획, 품질검사 과정을 바코드 기반으로 관리하는 통합 생산 및 물류 관리 시스템입니다.',
    contribution: '기여도 40%',
    points: [
      '서브 프론트엔드 개발자로 생산 효율성 증대를 위한 반응형 웹페이지를 제작했습니다.',
      'Figma를 바탕으로 Android, iOS CSS 동기화 작업을 진행했습니다.',
      '루틴 업무를 자동화하는 기능을 개발해 생산 효율성을 약 20% 높였습니다.',
      '각 페이지에서 반복되던 페이징을 공통 컴포넌트로 분리했습니다.',
    ],
    stack: ['MES', 'WMS', 'ERP', 'Responsive UI', 'Figma'],
  },
  {
    name: '블랙박스 영상을 활용한 비대면 교통사고 과실비율 판단 AI 서비스',
    type: '스마트인재개발원 · Frontend Developer',
    period: '2022.06.01 - 2022.07.25',
    summary:
      '교통사고 처리 과정의 불만족과 스트레스를 줄이기 위해, 블랙박스 영상과 판례 정보를 활용해 과실비율 판단을 돕는 AI 서비스입니다.',
    points: [
      'UX/UI 디자인과 프론트엔드 화면 개발을 담당했습니다.',
      'Git을 활용해 소스 코드 백업, 협업, 버전 관리를 진행했습니다.',
      'Image Picker 라이브러리로 사진 첨부와 프리뷰 기능을 구현했습니다.',
      'React Slick 라이브러리를 이용해 메인 슬라이드를 구현했습니다.',
      'JDBC, MVC, DI 구조를 학습하며 Spring 프레임워크의 동작 원리를 이해했습니다.',
    ],
    stack: ['Spring Framework', 'FFmpeg', 'Git', 'HTML5', 'CSS3', 'Bootstrap4', 'Thymeleaf'],
  },
  {
    name: '긍정 심리치료 기법을 적용한 긍정화 다이어리',
    type: 'Team · Frontend Developer',
    period: '2022.04.01 - 2022.05.20',
    summary:
      '코로나 이후 우울감 경험 증가 문제에서 출발해, 긍정 심리치료 표현 방식을 적용한 다이어리 서비스입니다.',
    points: [
      '프로젝트 기획, UI 디자인, 프론트엔드 개발을 담당했습니다.',
      'Notion과 Jira로 프로젝트 task 관리와 스프린트를 진행했습니다.',
      '일기 작성, 로그인, 회원가입, 통계 보기 화면 레이아웃을 제작했습니다.',
      'Calendar API와 Chart.js를 활용해 기능 완성도를 높였습니다.',
      '사용자 경험을 위해 클릭 효과와 화면 반응에 집중했습니다.',
    ],
    stack: ['Java', 'JSP/Servlet', 'HTML/CSS', 'JavaScript', 'Chart.js'],
  },
]

const troubleshootingCases = [
  {
    project: '이음',
    title: '이미지 로딩 지연 문제 개선',
    problem:
      '프로젝트 화면에서 이미지가 많은 영역에 진입할 때 초기 로딩이 길어지고, 사용자가 화면이 멈춘 것처럼 느끼는 문제가 있었습니다.',
    cause:
      '필요한 이미지와 당장 보이지 않는 이미지가 함께 요청되면서 네트워크 요청이 몰렸고, 원본 이미지 용량도 화면 표시 목적에 비해 큰 편이었습니다.',
    actions: [
      '브라우저 개발자 도구의 Network 탭으로 이미지 요청 수, 용량, 로딩 순서를 확인했습니다.',
      '첫 화면에 필요한 이미지와 스크롤 이후 필요한 이미지를 분리해 우선순위를 정리했습니다.',
      '이미지 표시 영역에는 로딩 상태와 대체 UI를 두어 사용자가 빈 화면으로 느끼지 않도록 개선했습니다.',
      '업로드/표시 흐름에서 이미지 용량과 표시 크기를 함께 고려하도록 팀원들과 기준을 맞췄습니다.',
    ],
    result:
      '초기 화면에서 꼭 필요한 이미지부터 먼저 보여주도록 정리해 체감 대기 시간을 줄였고, 이미지 로딩 중에도 화면 흐름을 유지할 수 있게 개선했습니다.',
  },
]
</script>

<template>
  <main class="portfolio">
    <nav class="top-nav" aria-label="주요 섹션">
      <a href="#ai">AI 활용</a>
      <a href="#career">경력</a>
      <a href="#skills">기술</a>
      <a href="#projects">프로젝트</a>
      <a href="#troubleshooting">트러블슈팅</a>
      <a href="#contact">Contact</a>
    </nav>

    <section class="hero-section">
      <div class="hero-copy">
        <p class="eyebrow">Frontend Developer Portfolio</p>
        <h1>운영 경험과 AI 활용 역량을 함께 갖춘 프론트엔드 개발자</h1>
        <p class="hero-description">
          레거시 개선, 반응형 UI, 데이터 기반 기능 구현 경험을 바탕으로 사용자가 실제로 쓰기 편한
          웹 서비스를 만듭니다. 최근에는 AI를 요구사항 정리, 코드 초안 작성, 오류 검토 과정에
          활용하며 더 정확하게 구현하는 습관을 쌓고 있습니다.
        </p>
        <div class="hero-actions">
          <a class="primary-action" href="#projects">프로젝트 보기</a>
          <a class="secondary-action" href="#ai">AI 활용 방식</a>
        </div>
      </div>

      <aside class="hero-panel" aria-label="핵심 역량 요약">
        <img :src="heroImage" alt="" />
        <dl>
          <div>
            <dt>Focus</dt>
            <dd>Frontend · 운영 개선 · AI 활용 개발 프로세스</dd>
          </div>
          <div>
            <dt>Experience</dt>
            <dd>웹 시스템 운영 안정화, MES/WMS, 매칭 플랫폼</dd>
          </div>
          <div>
            <dt>Strength</dt>
            <dd>요구사항 분석부터 구현, 검증, 개선까지 이어가는 실행력</dd>
          </div>
        </dl>
      </aside>
    </section>

    <section id="ai" class="section-block ai-section">
      <div class="section-heading">
        <p class="eyebrow">Development Workflow</p>
        <h2>AI를 활용한 개발 방식</h2>
        <p>
          AI를 결과물을 대신 만들어주는 도구가 아니라, 요구사항을 정리하고 구현 품질을 점검하는
          보조 도구로 활용합니다.
        </p>
      </div>

      <div class="workflow-grid">
        <article v-for="item in aiWorkflow" :key="item.phase" class="workflow-card">
          <span>{{ item.phase }}</span>
          <h3>{{ item.title }}</h3>
          <ul>
            <li v-for="point in item.points" :key="point">{{ point }}</li>
          </ul>
        </article>
      </div>
    </section>

    <section id="career" class="section-block">
      <div class="section-heading">
        <p class="eyebrow">Career</p>
        <h2>경력</h2>
      </div>

      <div class="timeline">
        <article v-for="career in careers" :key="career.company" class="timeline-item">
          <div>
            <p class="period">{{ career.period }}</p>
            <h3>{{ career.company }}</h3>
            <p class="role">{{ career.role }}</p>
          </div>
          <ul>
            <li v-for="point in career.points" :key="point">{{ point }}</li>
          </ul>
        </article>
      </div>
    </section>

    <section class="section-block">
      <div class="section-heading">
        <p class="eyebrow">Certificates</p>
        <h2>자격증</h2>
      </div>

      <div class="certificate-grid">
        <article v-for="certificate in certificates" :key="certificate.name" class="certificate-card">
          <p class="period">{{ certificate.date }}</p>
          <h3>{{ certificate.name }}</h3>
          <p>{{ certificate.status }}</p>
          <small>{{ certificate.issuer }}</small>
          <small v-if="certificate.number">자격번호 {{ certificate.number }}</small>
        </article>
      </div>
    </section>

    <section id="skills" class="section-block">
      <div class="section-heading">
        <p class="eyebrow">Skills</p>
        <h2>사용 기술</h2>
        <p>프론트엔드 구현, 데이터 처리, 협업 도구 사용 경험을 실무 중심으로 정리했습니다.</p>
      </div>

      <div class="skills-grid">
        <article v-for="skill in skills" :key="skill.name" class="skill-card">
          <h3>{{ skill.name }}</h3>
          <ul>
            <li v-for="item in skill.items" :key="item">{{ item }}</li>
          </ul>
        </article>
      </div>
    </section>

    <section id="projects" class="section-block">
      <div class="section-heading">
        <p class="eyebrow">Projects</p>
        <h2>프로젝트</h2>
      </div>

      <div class="project-list">
        <article v-for="project in projects" :key="project.name" class="project-card">
          <div class="project-header">
            <div>
              <p class="period">{{ project.period }}</p>
              <h3>{{ project.name }}</h3>
              <p class="role">{{ project.type }}</p>
            </div>
            <span v-if="project.contribution" class="contribution">{{ project.contribution }}</span>
          </div>
          <p class="project-summary">{{ project.summary }}</p>
          <ul>
            <li v-for="point in project.points" :key="point">{{ point }}</li>
          </ul>
          <div class="stack-list">
            <span v-for="stack in project.stack" :key="stack">{{ stack }}</span>
          </div>
        </article>
      </div>
    </section>

    <section id="troubleshooting" class="section-block">
      <div class="section-heading">
        <p class="eyebrow">Troubleshooting</p>
        <h2>문제를 발견하고 개선한 경험</h2>
        <p>
          단순 구현에 그치지 않고, 사용자가 불편함을 느끼는 지점을 확인해 원인을 좁히고 개선한
          사례입니다.
        </p>
      </div>

      <div class="troubleshooting-list">
        <article
          v-for="trouble in troubleshootingCases"
          :key="trouble.title"
          class="troubleshooting-card"
        >
          <div class="trouble-layout">
            <div class="trouble-meta">
              <p class="period">{{ trouble.project }}</p>
              <h3>{{ trouble.title }}</h3>
            </div>

            <div class="trouble-content">
              <div class="trouble-detail-grid">
                <section>
                  <h4>문제</h4>
                  <p>{{ trouble.problem }}</p>
                </section>
                <section>
                  <h4>원인</h4>
                  <p>{{ trouble.cause }}</p>
                </section>
              </div>

              <section class="trouble-actions">
                <h4>개선 과정</h4>
                <ul>
                  <li v-for="action in trouble.actions" :key="action">{{ action }}</li>
                </ul>
              </section>

              <section class="trouble-result">
                <h4>결과</h4>
                <p>{{ trouble.result }}</p>
              </section>
            </div>
          </div>
        </article>
      </div>
    </section>

    <section id="contact" class="contact-section">
      <div>
        <p class="eyebrow">Contact</p>
        <h2>함께 일하기 좋은 개발자가 되겠습니다.</h2>
        <p>
          운영 안정화 경험, 프론트엔드 구현력, AI 기반 검증 습관을 바탕으로 더 나은 서비스를 만드는
          개발자가 되겠습니다.
        </p>
      </div>
    </section>
  </main>
</template>

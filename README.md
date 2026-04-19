<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, viewport-fit=cover">
  <title>Omja Ujesha Jetshree · full-stack & AI</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      background: #f6f8fa;
      font-family: 'Inter', system-ui, -apple-system, 'Segoe UI', Roboto, Helvetica, sans-serif;
      line-height: 1.5;
      color: #1a2a3f;
      padding: 2rem 1rem;
    }

    /* smooth container */
    .container {
      max-width: 1000px;
      margin: 0 auto;
      background: #ffffff;
      border-radius: 2rem;
      box-shadow: 0 12px 30px rgba(0, 0, 0, 0.03), 0 4px 8px rgba(0, 0, 0, 0.05);
      overflow: hidden;
      padding: 2rem 1.8rem;
    }

    @media (min-width: 640px) {
      body {
        padding: 2.5rem;
      }
      .container {
        padding: 2.5rem 2.8rem;
      }
    }

    /* typography */
    h1 {
      font-size: 2rem;
      font-weight: 600;
      letter-spacing: -0.02em;
      background: linear-gradient(135deg, #0a2b4e 0%, #1e4a76 100%);
      background-clip: text;
      -webkit-background-clip: text;
      color: transparent;
      margin-bottom: 0.25rem;
    }

    .tagline {
      font-size: 1rem;
      color: #4b6f8c;
      border-left: 3px solid #2c7da0;
      padding-left: 0.9rem;
      margin: 0.5rem 0 1.8rem 0;
      font-weight: 450;
    }

    /* section styling */
    .section {
      margin-bottom: 2.2rem;
    }

    .section-title {
      font-size: 1.25rem;
      font-weight: 600;
      color: #0f3b5c;
      letter-spacing: -0.2px;
      display: inline-block;
      margin-bottom: 1rem;
      border-bottom: 2px solid #e2e8f0;
      padding-bottom: 0.25rem;
    }

    /* minimal lists */
    .clean-list {
      list-style: none;
      padding: 0;
      display: flex;
      flex-direction: column;
      gap: 0.6rem;
    }

    .clean-list li {
      position: relative;
      padding-left: 1.3rem;
      font-size: 0.95rem;
      color: #1f3b4c;
    }

    .clean-list li::before {
      content: "—";
      position: absolute;
      left: 0;
      color: #2c7da0;
      font-weight: 500;
      opacity: 0.7;
    }

    strong {
      color: #1a5d7d;
      font-weight: 600;
    }

    /* bio text minimal */
    .bio-text {
      background: #f9fbfd;
      padding: 1rem 1.2rem;
      border-radius: 1.2rem;
      font-size: 0.95rem;
      color: #1f3b4c;
      margin-top: 0.5rem;
      border: 1px solid #edf2f7;
    }

    .bio-text p + p {
      margin-top: 0.8rem;
    }

    /* social row — clean & minimal */
    .social-row {
      display: flex;
      flex-wrap: wrap;
      gap: 0.8rem;
      margin: 1.5rem 0 1rem 0;
      align-items: center;
    }

    .social-badge {
      display: inline-flex;
      align-items: center;
      background: #f1f5f9;
      padding: 0.3rem 0.8rem;
      border-radius: 40px;
      font-size: 0.8rem;
      font-weight: 500;
      transition: all 0.2s ease;
      text-decoration: none;
      color: #1e4663;
      gap: 6px;
    }

    .social-badge img {
      width: 16px;
      height: 16px;
      vertical-align: middle;
    }

    .social-badge:hover {
      background: #e6edf4;
      transform: translateY(-1px);
    }

    /* tech stack grid — clean, compact, minimal */
    .tech-grid {
      display: flex;
      flex-wrap: wrap;
      gap: 0.55rem;
      margin-top: 0.5rem;
    }

    .tech-badge {
      background: #f1f5f9;
      padding: 0.25rem 0.8rem;
      border-radius: 30px;
      font-size: 0.75rem;
      font-weight: 500;
      color: #1f5e7e;
      letter-spacing: -0.2px;
      transition: all 0.1s ease;
      white-space: nowrap;
    }

    /* For shield.io images - we keep original but make them compact */
    .tech-shield {
      height: 26px;
      transition: opacity 0.1s;
    }

    /* stats row minimal */
    .stats-wrapper {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 1.2rem;
      margin: 1.8rem 0 1rem;
    }

    .stats-card {
      background: #fafcff;
      border-radius: 1.2rem;
      padding: 0.5rem;
      border: 1px solid #eef3fc;
      overflow: hidden;
    }

    .stats-card img {
      max-width: 100%;
      height: auto;
      display: block;
      border-radius: 0.8rem;
    }

    .visit-count {
      text-align: center;
      margin-top: 1rem;
      opacity: 0.7;
      font-size: 0.75rem;
    }

    hr {
      margin: 1rem 0 1.5rem;
      border: 0;
      height: 1px;
      background: linear-gradient(to right, #e2e8f0, transparent);
    }

    /* responsive tweaks */
    @media (max-width: 700px) {
      .container {
        padding: 1.5rem;
      }
      .stats-wrapper {
        flex-direction: column;
        align-items: center;
      }
      .tech-shield {
        height: 24px;
      }
    }

    a {
      text-decoration: none;
    }

    /* inline badges for social (preserve look but cleaner) */
    .inline-icon {
      vertical-align: middle;
    }
  </style>
</head>
<body>
<div class="container">
  
  <!-- header: name + minimal role -->
  <h1>Omja Ujesha Jetshree</h1>
  <div class="tagline">full-stack · AI integrations · system design</div>

  <!-- 1. What I'm building -->
  <div class="section">
    <div class="section-title">▸ building</div>
    <ul class="clean-list">
      <li>Scalable full-stack apps using <strong>MERN</strong> & <strong>Django</strong></li>
      <li>AI-powered tools — <strong>OpenAI API</strong>, <strong>GPT-4</strong>, <strong>LangChain</strong></li>
      <li>Content summarization platforms & booking applications</li>
    </ul>
  </div>

  <!-- 2. Open to collaborate -->
  <div class="section">
    <div class="section-title">▸ collaborate</div>
    <ul class="clean-list">
      <li>Cloud-first applications with <strong>MERN</strong>, <strong>Django</strong> or hybrid stacks</li>
      <li>AI/ML-integrated web applications</li>
      <li>Real-time systems & chatbot architectures</li>
    </ul>
  </div>

  <!-- 3. Currently exploring -->
  <div class="section">
    <div class="section-title">▸ exploring</div>
    <ul class="clean-list">
      <li>Agentic AI & goal-driven workflows</li>
      <li><strong>LangChain</strong> for chaining LLM calls</li>
      <li>Vector DBs — <strong>Pinecone</strong>, <strong>ChromaDB</strong></li>
      <li>Prompt engineering & <strong>LLMOps</strong></li>
      <li>Immersive UIs with <strong>Three.js</strong> + <strong>Next.js</strong></li>
    </ul>
  </div>

  <!-- 4. Where I’d appreciate insight -->
  <div class="section">
    <div class="section-title">▸ insight welcome</div>
    <ul class="clean-list">
      <li>Feedback on AI / health-tech product ideas</li>
      <li>Creating a hybrid tech + design portfolio</li>
      <li>Optimizing MERN stacks for scale & performance</li>
    </ul>
  </div>

  <!-- 5. What you can ask me -->
  <div class="section">
    <div class="section-title">▸ ask me about</div>
    <ul class="clean-list">
      <li>Real-time apps with MERN / Django</li>
      <li>Integrating AI in React + Python environments</li>
      <li>End-to-end deployments on AWS, GCP, DigitalOcean</li>
      <li>UI/UX systems for growth-ready apps</li>
      <li>Remote work & agile team workflows</li>
    </ul>
  </div>

  <!-- 6. Who I am – condensed but same meaning -->
  <div class="section">
    <div class="section-title">▸ who I am</div>
    <div class="bio-text">
      <p><strong>Omja Ujesha Jetshree</strong> — full-stack developer crafting scalable, AI-powered products. My work bridges MERN & Python ecosystems with intelligent features (NLP pipelines, multilingual support). From real-time booking systems to GPT-driven platforms: clarity, performance, usability at the core.</p>
      <p>Currently diving into agentic AI, LangChain, advanced retrieval systems. Always excited to collaborate at the intersection of design, intelligence, and user experience.</p>
    </div>
  </div>

  <!-- social links: minimal but exact same profiles -->
  <div class="social-row">
    <a href="https://instagram.com/omja.sharmaaa" class="social-badge" target="_blank" rel="noopener">
      <svg width="14" height="14" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M12 2.98c2.28 0 2.55.01 3.44.05 1.08.05 1.79.22 2.2.38.52.2.9.44 1.29.83.39.39.63.77.83 1.29.16.41.33 1.12.38 2.2.04.89.05 1.16.05 3.44s-.01 2.55-.05 3.44c-.05 1.08-.22 1.79-.38 2.2-.2.52-.44.9-.83 1.29-.39.39-.77.63-1.29.83-.41.16-1.12.33-2.2.38-.89.04-1.16.05-3.44.05s-2.55-.01-3.44-.05c-1.08-.05-1.79-.22-2.2-.38-.52-.2-.9-.44-1.29-.83-.39-.39-.63-.77-.83-1.29-.16-.41-.33-1.12-.38-2.2-.04-.89-.05-1.16-.05-3.44s.01-2.55.05-3.44c.05-1.08.22-1.79.38-2.2.2-.52.44-.9.83-1.29.39-.39.77-.63 1.29-.83.41-.16 1.12-.33 2.2-.38.89-.04 1.16-.05 3.44-.05zM12 7.21a4.79 4.79 0 100 9.58 4.79 4.79 0 000-9.58zm0 7.9a3.11 3.11 0 110-6.22 3.11 3.11 0 010 6.22zm6.11-8.11a1.12 1.12 0 10-2.24 0 1.12 1.12 0 002.24 0z" fill="currentColor"/></svg>
      Instagram
    </a>
    <a href="https://linkedin.com/in/omjasharma" class="social-badge" target="_blank" rel="noopener">
      <svg width="14" height="14" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433a2.062 2.062 0 01-2.063-2.065 2.064 2.064 0 112.063 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C0.792 0 0 0.774 0 1.729v20.542C0 23.227 0.792 24 1.771 24h20.451c0.979 0 1.771-0.773 1.771-1.729V1.729C24 0.774 23.208 0 22.225 0z" fill="currentColor"/></svg>
      LinkedIn
    </a>
    <a href="mailto:omjasharma15@gmail.com" class="social-badge">
      <svg width="14" height="14" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M20 4H4c-1.1 0-2 .9-2 2v12c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V6c0-1.1-.9-2-2-2zm0 4l-8 5-8-5V6l8 5 8-5v2z" fill="currentColor"/></svg>
      omjasharma15@gmail.com
    </a>
  </div>

  <!-- Tech stack – minimal but complete (all original badges) -->
  <div class="section">
    <div class="section-title">▸ tech stack</div>
    <div class="tech-grid" style="display: flex; flex-wrap: wrap; gap: 0.45rem; margin-top: 0.5rem;">
      <!-- we embed original badge images but keep them clean and responsive (same tech content) -->
      <img src="https://img.shields.io/badge/c-%2300599C.svg?style=flat&logo=c&logoColor=white" alt="C" class="tech-shield">
      <img src="https://img.shields.io/badge/css3-%231572B6.svg?style=flat&logo=css3&logoColor=white" alt="CSS3" class="tech-shield">
      <img src="https://img.shields.io/badge/python-3670A0?style=flat&logo=python&logoColor=ffdd54" alt="Python" class="tech-shield">
      <img src="https://img.shields.io/badge/html5-%23E34F26.svg?style=flat&logo=html5&logoColor=white" alt="HTML5" class="tech-shield">
      <img src="https://img.shields.io/badge/java-%23ED8B00.svg?style=flat&logo=openjdk&logoColor=white" alt="Java" class="tech-shield">
      <img src="https://img.shields.io/badge/javascript-%23323330.svg?style=flat&logo=javascript&logoColor=%23F7DF1E" alt="JS" class="tech-shield">
      <img src="https://img.shields.io/badge/typescript-%23007ACC.svg?style=flat&logo=typescript&logoColor=white" alt="TS" class="tech-shield">
      <img src="https://img.shields.io/badge/vercel-%23000000.svg?style=flat&logo=vercel&logoColor=white" alt="Vercel" class="tech-shield">
      <img src="https://img.shields.io/badge/AWS-%23FF9900.svg?style=flat&logo=amazon-aws&logoColor=white" alt="AWS" class="tech-shield">
      <img src="https://img.shields.io/badge/GoogleCloud-%234285F4.svg?style=flat&logo=google-cloud&logoColor=white" alt="GCP" class="tech-shield">
      <img src="https://img.shields.io/badge/DigitalOcean-%230167ff.svg?style=flat&logo=digitalOcean&logoColor=white" alt="DigitalOcean" class="tech-shield">
      <img src="https://img.shields.io/badge/firebase-%23039BE5.svg?style=flat&logo=firebase" alt="Firebase" class="tech-shield">
      <img src="https://img.shields.io/badge/netlify-%23000000.svg?style=flat&logo=netlify&logoColor=#00C7B7" alt="Netlify" class="tech-shield">
      <img src="https://img.shields.io/badge/heroku-%23430098.svg?style=flat&logo=heroku&logoColor=white" alt="Heroku" class="tech-shield">
      <img src="https://img.shields.io/badge/-AntDesign-%230170FE?style=flat&logo=ant-design&logoColor=white" alt="AntD" class="tech-shield">
      <img src="https://img.shields.io/badge/Bun-%23000000.svg?style=flat&logo=bun&logoColor=white" alt="Bun" class="tech-shield">
      <img src="https://img.shields.io/badge/daisyui-5A0EF8?style=flat&logo=daisyui&logoColor=white" alt="DaisyUI" class="tech-shield">
      <img src="https://img.shields.io/badge/django-%23092E20.svg?style=flat&logo=django&logoColor=white" alt="Django" class="tech-shield">
      <img src="https://img.shields.io/badge/express.js-%23404d59.svg?style=flat&logo=express&logoColor=%2361DAFB" alt="Express" class="tech-shield">
      <img src="https://img.shields.io/badge/FastAPI-005571?style=flat&logo=fastapi" alt="FastAPI" class="tech-shield">
      <img src="https://img.shields.io/badge/flask-%23000.svg?style=flat&logo=flask&logoColor=white" alt="Flask" class="tech-shield">
      <img src="https://img.shields.io/badge/Flutter-%2302569B.svg?style=flat&logo=Flutter&logoColor=white" alt="Flutter" class="tech-shield">
      <img src="https://img.shields.io/badge/JWT-black?style=flat&logo=JSON%20web%20tokens" alt="JWT" class="tech-shield">
      <img src="https://img.shields.io/badge/MUI-%230081CB.svg?style=flat&logo=mui&logoColor=white" alt="MUI" class="tech-shield">
      <img src="https://img.shields.io/badge/NODEMON-%23323330.svg?style=flat&logo=nodemon&logoColor=%BBDEAD" alt="Nodemon" class="tech-shield">
      <img src="https://img.shields.io/badge/node.js-6DA55F?style=flat&logo=node.js&logoColor=white" alt="NodeJS" class="tech-shield">
      <img src="https://img.shields.io/badge/Next-black?style=flat&logo=next.js&logoColor=white" alt="Next.js" class="tech-shield">
      <img src="https://img.shields.io/badge/NPM-%23CB3837.svg?style=flat&logo=npm&logoColor=white" alt="NPM" class="tech-shield">
      <img src="https://img.shields.io/badge/react-%2320232a.svg?style=flat&logo=react&logoColor=%2361DAFB" alt="React" class="tech-shield">
      <img src="https://img.shields.io/badge/react_native-%2320232a.svg?style=flat&logo=react&logoColor=%2361DAFB" alt="React Native" class="tech-shield">
      <img src="https://img.shields.io/badge/-React%20Query-FF4154?style=flat&logo=react%20query&logoColor=white" alt="React Query" class="tech-shield">
      <img src="https://img.shields.io/badge/redux-%23593d88.svg?style=flat&logo=redux&logoColor=white" alt="Redux" class="tech-shield">
      <img src="https://img.shields.io/badge/React%20Hook%20Form-%23EC5990.svg?style=flat&logo=reacthookform&logoColor=white" alt="React Hook Form" class="tech-shield">
      <img src="https://img.shields.io/badge/React_Router-CA4245?style=flat&logo=react-router&logoColor=white" alt="React Router" class="tech-shield">
      <img src="https://img.shields.io/badge/Socket.io-black?style=flat&logo=socket.io&badgeColor=010101" alt="Socket.io" class="tech-shield">
      <img src="https://img.shields.io/badge/styled--components-DB7093?style=flat&logo=styled-components&logoColor=white" alt="Styled" class="tech-shield">
      <img src="https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=flat&logo=tailwind-css&logoColor=white" alt="Tailwind" class="tech-shield">
      <img src="https://img.shields.io/badge/threejs-black?style=flat&logo=three.js&logoColor=white" alt="Three.js" class="tech-shield">
      <img src="https://img.shields.io/badge/vite-%23646CFF.svg?style=flat&logo=vite&logoColor=white" alt="Vite" class="tech-shield">
      <img src="https://img.shields.io/badge/web3.js-F16822?style=flat&logo=web3.js&logoColor=white" alt="Web3" class="tech-shield">
      <img src="https://img.shields.io/badge/nginx-%23009639.svg?style=flat&logo=nginx&logoColor=white" alt="Nginx" class="tech-shield">
      <img src="https://img.shields.io/badge/apache-%23D42029.svg?style=flat&logo=apache&logoColor=white" alt="Apache" class="tech-shield">
      <img src="https://img.shields.io/badge/gunicorn-%298729.svg?style=flat&logo=gunicorn&logoColor=white" alt="Gunicorn" class="tech-shield">
      <img src="https://img.shields.io/badge/Prisma-3982CE?style=flat&logo=Prisma&logoColor=white" alt="Prisma" class="tech-shield">
      <img src="https://img.shields.io/badge/redis-%23DD0031.svg?style=flat&logo=redis&logoColor=white" alt="Redis" class="tech-shield">
      <img src="https://img.shields.io/badge/firebase-a08021?style=flat&logo=firebase&logoColor=ffcd34" alt="Firebase2" class="tech-shield">
      <img src="https://img.shields.io/badge/mysql-4479A1.svg?style=flat&logo=mysql&logoColor=white" alt="MySQL" class="tech-shield">
      <img src="https://img.shields.io/badge/planetscale-%23000000.svg?style=flat&logo=planetscale&logoColor=white" alt="PlanetScale" class="tech-shield">
      <img src="https://img.shields.io/badge/postgres-%23316192.svg?style=flat&logo=postgresql&logoColor=white" alt="Postgres" class="tech-shield">
      <img src="https://img.shields.io/badge/Canva-%2300C4CC.svg?style=flat&logo=Canva&logoColor=white" alt="Canva" class="tech-shield">
      <img src="https://img.shields.io/badge/figma-%23F24E1E.svg?style=flat&logo=figma&logoColor=white" alt="Figma" class="tech-shield">
      <img src="https://img.shields.io/badge/Dribbble-EA4C89?style=flat&logo=dribbble&logoColor=white" alt="Dribbble" class="tech-shield">
      <img src="https://img.shields.io/badge/Framer-black?style=flat&logo=framer&logoColor=blue" alt="Framer" class="tech-shield">
      <img src="https://img.shields.io/badge/Keras-%23D00000.svg?style=flat&logo=Keras&logoColor=white" alt="Keras" class="tech-shield">
      <img src="https://img.shields.io/badge/numpy-%23013243.svg?style=flat&logo=numpy&logoColor=white" alt="NumPy" class="tech-shield">
      <img src="https://img.shields.io/badge/pandas-%23150458.svg?style=flat&logo=pandas&logoColor=white" alt="Pandas" class="tech-shield">
      <img src="https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=flat&logo=PyTorch&logoColor=white" alt="PyTorch" class="tech-shield">
      <img src="https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=flat&logo=TensorFlow&logoColor=white" alt="TF" class="tech-shield">
      <img src="https://img.shields.io/badge/git-%23F05033.svg?style=flat&logo=git&logoColor=white" alt="Git" class="tech-shield">
      <img src="https://img.shields.io/badge/github-%23121011.svg?style=flat&logo=github&logoColor=white" alt="GitHub" class="tech-shield">
      <img src="https://img.shields.io/badge/Postman-FF6C37?style=flat&logo=postman&logoColor=white" alt="Postman" class="tech-shield">
    </div>
  </div>

  <!-- GitHub stats minimal row (same content) -->
  <div class="stats-wrapper">
    <div class="stats-card">
      <img src="https://github-readme-stats.vercel.app/api?username=sharmaomja&theme=dark&hide_border=true&include_all_commits=true&count_private=true" alt="GitHub Stats">
    </div>
    <div class="stats-card">
      <img src="https://nirzak-streak-stats.vercel.app/?user=sharmaomja&theme=dark&hide_border=true" alt="GitHub Streak">
    </div>
    <div class="stats-card">
      <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=sharmaomja&theme=dark&hide_border=true&include_all_commits=true&count_private=true&layout=compact" alt="Top Langs">
    </div>
  </div>

  <!-- visit count (minimal) -->
  <div class="visit-count">
    <img src="https://visitcount.itsvg.in/api?id=sharmaomja&icon=0&color=0" alt="visitor counter" style="opacity:0.7">
  </div>

  <!-- subtle spacer -->
  <hr style="margin-top: 1.8rem;">
  <div style="height: 0.25rem;"></div>
</div>
</body>
</html>

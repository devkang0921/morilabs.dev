<script lang="ts">
  import Logo from '$lib/Logo.svelte';
  import ThemeToggle from '$lib/ThemeToggle.svelte';
</script>

<svelte:head>
  <title>MoriLabs.dev — 쓸모 있는 아이디어를, 일상에.</title>
  <meta name="description" content="일상의 작은 불편을, 매일 쓰고 싶은 서비스로 바꿉니다. MoriLabs.dev는 쓰는 순간부터 차이를 느낄 수 있도록, 보이지 않는 디테일까지 다듬습니다." />
  <link rel="canonical" href="https://morilabs.dev/" />
  <meta property="og:title" content="MoriLabs.dev — Ideas into everyday." />
  <meta property="og:description" content="일상의 작은 불편을, 매일 쓰고 싶은 서비스로. 필요한 서비스를 직접 만들고 꾸준히 개선하는 MoriLabs.dev의 제품을 만나보세요." />
  <meta property="og:type" content="website" />
  <meta property="og:url" content="https://morilabs.dev/" />
  <meta property="og:locale" content="ko_KR" />
</svelte:head>

<a class="skip-link" href="#main">본문으로 바로가기</a>
<div class="site-shell" id="top">
  <header>
    <a class="wordmark" href="#top" aria-label="MoriLabs.dev 홈"><Logo /></a>
    <nav aria-label="주요 메뉴">
      <a href="#work">WORK</a>
      <a href="#about">ABOUT</a>
    </nav>
    <div class="header-actions"><a class="header-contact" href="#contact">CONTACT</a><ThemeToggle /></div>
  </header>

  <main id="main">
    <section class="hero" aria-labelledby="hero-title">
      <div class="section-meta"><span>ML—001 / DIGITAL PRODUCTS</span><span class="availability"><i></i> BUILDING WHAT’S NEXT</span></div>
      <div class="hero-center">
        <a class="announcement" href="https://morigram.com" target="_blank" rel="noopener noreferrer"><span>LIVE</span> MEET OUR FIRST PRODUCT — MORIGRAM</a>
        <p class="eyebrow">LESS FRICTION. MORE POSSIBILITY.</p>
        <h1 id="hero-title">IDEAS INTO<br /><span>EVERYDAY.</span></h1>
        <div class="hero-bottom">
          <div><h2>디테일을 다듬고, 쓸모를 만듭니다.</h2><p>일상의 작은 불편을, 매일 쓰고 싶은 서비스로 바꿉니다.<br />MoriLabs.dev는 쓰는 순간부터 차이를 느낄 수 있도록,<br />보이지 않는 디테일까지 다듬습니다.</p></div>
          <a class="button primary" href="#work">직접 만드는 서비스</a>
        </div>
      </div>
      <div class="hero-foot"><span>THOUGHTFULLY BUILT. CONTINUOUSLY GROWING.</span><a href="#work">SCROLL TO EXPLORE</a></div>
    </section>

    <section class="work section" id="work" aria-labelledby="work-title">
      <div class="section-heading"><div><p class="eyebrow">01 / OUR PRODUCTS</p><h2 id="work-title">작은 시작.<br /><span>이어지는 가능성.</span></h2></div><p class="section-description">직접 만들고, 운영하며, 더 나아갑니다.<br />MoriLabs.dev의 첫 번째 제품을 만나보세요.</p></div>
      <a class="project" href="https://morigram.com" target="_blank" rel="noopener noreferrer" aria-label="모리그램 사이트 새 탭에서 보기">
        <div class="project-art">
          <div class="art-top"><span>MORIGRAM / PRODUCT 001</span><span>● LIVE</span></div>
          <div class="archive-visual" aria-hidden="true"><div class="archive-card back"><span>OUR STORIES</span><div class="landscape"></div></div><div class="archive-card front"><div class="card-heading"><span>SUMMER, TOGETHER</span><span>＋</span></div><div class="photo-grid"><div class="photo photo-one"></div><div class="photo photo-two"></div><div class="photo photo-three"></div></div><div class="card-footer"><span>순간은 모이고, 이야기는 남는다.</span><span>01 — 03</span></div></div><span class="orbit-star">✳</span></div>
          <div class="art-bottom"><span>morigram<span class="small-dot">®</span></span><p>MOMENTS BECOME STORIES.</p></div>
        </div>
        <div class="project-info"><div><span class="tag">WEB PLATFORM</span><h3>모리그램 <span>Morigram</span></h3><p>흩어진 순간을 모아, 오래 남을 이야기로.<br />사진·영상부터 관련 자료까지, 한곳에 남기는 행사 아카이브 플랫폼.</p></div><span class="project-link">서비스 방문하기</span></div>
      </a>
      <div class="next-project"><span class="next-number">002</span><div><h3>다음 이야기도, 이곳에서.</h3><p>MoriLabs.dev가 만들어갈 제품들이 하나씩 쌓입니다.</p></div><span class="eyebrow">MORE TO COME</span></div>
    </section>

    <section class="about section" id="about" aria-labelledby="about-title">
      <div class="section-heading"><div><p class="eyebrow">02 / THE WAY WE BUILD</p><h2 id="about-title">필요에서 시작해,<br /><span>쓰임으로 완성합니다.</span></h2></div><p class="section-description">필요한 서비스를 직접 만들고,<br />사용자의 일상 속에서 더 나아지도록 꾸준히 개선합니다.</p></div>
      <div class="principles">
        <article><div class="principle-top"><span>PRINCIPLE / 01</span><span>⌕</span></div><h3>일상의 문제를 발견합니다.</h3><p>익숙해서 지나쳤던 불편함을 들여다봅니다. 실제로 필요한 것이 무엇인지 묻는 것부터 시작합니다.</p><span class="principle-label">START WITH A REAL NEED</span></article>
        <article><div class="principle-top"><span>PRINCIPLE / 02</span><span>＋</span></div><h3>디테일로 완성도를 높입니다.</h3><p>한 줄의 문구, 버튼의 반응, 자연스러운 흐름까지. 기능을 더하기 전에 작은 불편을 덜어내고, 쓰기 편한 경험으로 다듬습니다.</p><span class="principle-label">CARE IN EVERY DETAIL</span></article>
        <article><div class="principle-top"><span>PRINCIPLE / 03</span><span>↻</span></div><h3>출시 이후에도 이어갑니다.</h3><p>출시는 끝이 아닌 시작입니다. 직접 운영하고 사용자의 이야기를 들으며, 더 나은 제품으로 다듬어갑니다.</p><span class="principle-label">BUILD. LISTEN. IMPROVE.</span></article>
      </div>
      <div class="studio-note"><p class="eyebrow">MADE FOR YOUR EVERYDAY</p><p>좋은 서비스는, 일상을 조금 더 편하게 만드니까.<br /><strong>작은 불편을 발견하고, 끝까지 다듬습니다.</strong><br />매일의 작은 순간에 자연스럽게 스며들도록.</p><span class="note-signature">작은 질문을, 다음 제품으로. <span>MoriLabs.dev</span></span></div>
    </section>

    <section class="contact section" id="contact" aria-labelledby="contact-title">
      <p class="eyebrow">03 / SAY HELLO</p>
      <div class="contact-heading">
        <div>
          <h2 id="contact-title">좋은 이야기는,<br /><span>작은 인사에서.</span></h2>
          <p>서비스에 대한 질문이나 피드백을 편하게 보내주세요.<br />더 편리한 일상을 위한 이야기를 기다립니다.</p>
        </div>
        <a class="email-link" href="mailto:support@morilabs.dev">support@morilabs.dev</a>
      </div>
    </section>
  </main>
  <footer><a class="wordmark" href="#top"><Logo /></a><span>© {new Date().getFullYear()} MoriLabs.dev</span><a href="https://morigram.com" target="_blank" rel="noopener noreferrer">MORIGRAM</a><a href="#top">BACK TO TOP</a></footer>
</div>

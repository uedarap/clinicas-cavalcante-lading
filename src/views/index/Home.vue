<script setup>

import U3Carousel from '../../components/UCarousel.vue';

const slidesConsulta = [
  {
    title: 'Cardiologia',
    details: 'Na nossa clínica, o atendimento em cardiologia é focado no cuidado integral do coração e do sistema cardiovascular. Oferecemos consultas, exames preventivos e tratamentos de condições como hipertensão, insuficiência cardíaca, arritmias e doenças coronarianas. Estamos aqui para cuidar da sua saúde cardíaca de forma personalizada.',
  },
  {
    title: 'Psiquiatria',
    details: 'O atendimento em psiquiatria é centrado no bem-estar mental e emocional dos nossos pacientes. Nossos profissionais estão preparados para diagnosticar e tratar condições como depressão, ansiedade, transtorno bipolar e esquizofrenia, sempre com empatia e uma abordagem humanizada.',
  },
  {
    title: 'Otorrino<br>laringologia',
    details: 'Oferecemos atendimento especializado em otorrinolaringologia, cuidando de problemas no ouvido, nariz e garganta. Nossa equipe trata condições como sinusite, alergias respiratórias, perda auditiva e apneia do sono, garantindo diagnósticos precisos e tratamentos eficazes.',
  },
  {
    title: 'Pediatria',
    details: 'O atendimento pediátrico na nossa clínica é voltado para o cuidado integral de crianças e adolescentes. Nossos pediatras acompanham o desenvolvimento físico e emocional, oferecendo prevenção, diagnóstico e tratamento de diversas condições, sempre em um ambiente acolhedor.',
  },
  {
    title: 'Ortopedia',
    details: 'Na área de ortopedia, nossos especialistas cuidam de doenças e lesões musculoesqueléticas. Atendemos pacientes com fraturas, dores crônicas, lesões esportivas e doenças como artrose, oferecendo tratamentos modernos e individualizados.',
  },
  {
    title: 'Oftalmologia',
    details: 'Nosso serviço de oftalmologia é dedicado à saúde dos olhos. Realizamos consultas, exames e tratamentos para miopia, astigmatismo, glaucoma e outras condições oculares, garantindo um acompanhamento completo e eficaz para a melhor qualidade de visão.',
  },
  {
    title: 'Nutrição',
    details: 'Oferecemos atendimento nutricional personalizado para promover uma alimentação saudável e equilibrada. Nossos nutricionistas elaboram planos alimentares específicos para prevenção de doenças, controle de peso e melhoria do bem-estar geral.',
  },
  {
    title: 'Hematologia',
    details: 'Na hematologia, nosso atendimento abrange o diagnóstico e tratamento de condições relacionadas ao sangue, como anemias, leucemias e distúrbios de coagulação. Trabalhamos com equipamentos modernos e protocolos seguros para garantir o melhor cuidado.',
  },
  {
    title: 'Ginecologia',
    details: 'Nosso atendimento ginecológico é voltado para a saúde integral da mulher, abordando prevenção, diagnóstico e tratamento de condições relacionadas ao sistema reprodutor. Oferecemos orientação em todas as fases da vida, sempre com acolhimento e cuidado.',
  },
  {
    title: 'Gastren<br>terologia',
    details: 'Na área de gastrenterologia, cuidamos da saúde do sistema digestivo, tratando condições como gastrite, refluxo e doenças inflamatórias intestinais. Oferecemos consultas e exames especializados para garantir o melhor cuidado ao paciente.',
  },
  {
    title: 'Endocrinologia',
    details: 'O atendimento em endocrinologia na nossa clínica é focado em tratamentos para diabetes, obesidade, problemas hormonais e disfunções da tireoide. Priorizamos uma abordagem individualizada para melhorar a qualidade de vida dos nossos pacientes.',
  },
  {
    title: 'Dermatologia',
    details: 'Na dermatologia, cuidamos da saúde da pele, cabelos e unhas. Tratamos condições como acne, psoríase e alergias cutâneas, além de realizarmos procedimentos estéticos e preventivos para o bem-estar do paciente.',
  },
  {
    title: 'Clínico Geral',
    details: 'Nosso atendimento clínico geral é voltado para a avaliação inicial e o acompanhamento integral dos pacientes. Oferecemos diagnóstico, tratamento e, se necessário, encaminhamento para outras especialidades, sempre com foco na saúde preventiva.',
  },
  {
    title: 'Cirurgia Vascular',
    details: 'Na cirurgia vascular, oferecemos atendimento especializado para o diagnóstico e tratamento de condições como varizes, tromboses e aneurismas. Utilizamos técnicas modernas para garantir segurança e eficácia nos procedimentos.',
  },
];
const slidesExame = [
  {
    title: 'Laboratório de Analises Clínicas',
    details: '',
  },
  {
    title: 'Colposcopia',
    details: 'A colposcopia é um exame ginecológico que permite a visualização detalhada do colo',
  },
  {
    title: 'Vulvoscopia',
    details: '',
  },
  {
    title: 'Ultrasonografia',
    details: '',
  },
  {
    title: 'Papanicolau',
    details: '',
  },
  {
    title: 'Laringoscopia',
    details: '',
  },
  {
    title: 'Nasofibro<br>laringoscopia',
    details: '',
  },
];
const slidesEstetica = [
  {
    title: 'Estética Facial',
    details: '',
  },
  {
    title: 'Estética Corporal',
    details: '',
  },
  {
    title: 'Criolipólise',
    details: '',
  },
  {
    title: 'Tratamento Ozonio Terapia',
    details: '',
  },
];

</script>

<template>
  <!-- ***** Preloader Start ***** -->
  <div id="js-preloader" class="js-preloader">
    <div class="preloader-inner">
      <span class="dot"></span>
      <div class="dots">
        <span></span>
        <span></span>
        <span></span>
      </div>
    </div>
  </div>
  <!-- ***** Preloader End ***** -->

  <!-- ***** Header Area Start ***** -->
  <header class="header-area header-sticky wow slideInDown" data-wow-duration="0.75s" data-wow-delay="0s">
    <div class="container">
      <div class="row">
        <div class="col-12">
          <nav class="main-nav">
            <!-- ***** Logo Start ***** -->
            <a href="index.html" class="logo">
              <img src="../../assets/images/logo.png" alt="">
            </a>
            <!-- ***** Logo End ***** -->
            <!-- ***** Menu Start ***** -->
            <ul class="nav">
              <li class="scroll-to-section"><a href="#top" class="active">Home</a></li>
              <li class="scroll-to-section"><a href="#features">Features</a></li>
              <li class="scroll-to-section"><a href="#about">About Us</a></li>
              <li class="scroll-to-section"><a href="#services">Services</a></li>
              <li class="scroll-to-section"><a href="#portfolio">Portfolio</a></li>
              <li class="scroll-to-section"><a href="#contact">Contact Us</a></li>
              <li class="scroll-to-section">
                <div class="main-blue-button"><a href="#contact">Whats App</a></div>
              </li>
            </ul>
            <a class='menu-trigger'>
              <span>Menu</span>
            </a>
            <!-- ***** Menu End ***** -->
          </nav>
        </div>
      </div>
    </div>
  </header>
  <!-- ***** Header Area End ***** -->

  <div class="main-banner wow fadeIn" id="top" data-wow-duration="1s" data-wow-delay="0.5s">
    <div class="container">
      <div class="row">
        <div class="col-lg-12">
          <div class="row">
            <div class="col-lg-6 align-self-center">
              <div class="left-content header-text wow fadeInLeft" data-wow-duration="1s" data-wow-delay="1s">
                <div class="row">
                  <!-- <div class="col-lg-4 col-sm-4">
                    <div class="info-stat">
                      <h6>Agency Status:</h6>
                      <h4>Ready Work</h4>
                    </div>
                  </div>
                  <div class="col-lg-4 col-sm-4">
                    <div class="info-stat">
                      <h6>Price:</h6>
                      <h4>$720/Month</h4>
                    </div>
                  </div>
                  <div class="col-lg-4 col-sm-4">
                    <div class="info-stat">
                      <h6>Schedules</h6>
                      <h4>$450/Meeting</h4>
                    </div>
                  </div> -->
                  <div class="col-lg-12">
                    <h2>Centro de Especialidades Médicas</h2>
                  </div>
                  <div class="col-lg-12">
                    <div class="main-green-button scroll-to-section">
                      <a href="#contact">Fale com nossos atendentes</a>
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <div class="col-lg-6">
              <div class="right-image wow fadeInRight" data-wow-duration="1s" data-wow-delay="0.5s">
                <img src="../../assets/images/doctor_green.png" alt="">
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>

  <div id="services" class="our-services section">
    <div class="container">
      <div class="row justify-content-center">
        <div class="col-lg-9">
          <div class="section-heading wow bounceIn" data-wow-duration="1s" data-wow-delay="0.2s">
            <h6>Cuidando de você, com qualidade e coração</h6>
            <h2>Desde 2011, o Centro Médico <span>Cavalcante</span> cuida da <em>saúde</em> da nossa região</h2>
          </div>
        </div>
      </div>
    </div>
    <div class="container">
      <div class="row">
        <div class="col-lg-12">
          <div class="section-heading wow bounceIn" data-wow-duration="1s" data-wow-delay="0.2s">
            <p>Desde 2011, o Centro Médico Cavalcante cuida da saúde da nossa região, com médicos especializados,
              exames de ponta e muita dedicação ao bem-estar e à prevenção da saúde dos nossos pacientes. Aqui, todo
              mundo é tratado com respeito e acolhimento.<br /><br />

              Além de atender vários convênios, fomos os pioneiros no Guarujá a oferecer consultas populares. Isso
              facilita para quem não tem plano de saúde, mas precisa de um médico de confiança.

              Em maio de 2017, abrimos nossa segunda unidade em Praia Grande, com 14 médicos atendendo em diferentes
              especialidades. Hoje, temos uma parceria com a Prefeitura e cuidamos de muitos pacientes do SUS.

              Já em 2021, inauguramos nossa segunda unidade no Guarujá para atender ainda mais pessoas, gerar empregos e
              trazer novos médicos para a cidade.
            </p>
          </div>
        </div>
      </div>
    </div>
    <div class="container-fluid">
      <div class="row">
        <div class="col-lg-4" data-bs-toggle="modal" data-bs-target="#modalConsulta" style="cursor: pointer;">
          <div class="service-item wow bounceInUp" data-wow-duration="1s" data-wow-delay="0.3s">
            <div class="row">
              <div class="col-lg-4">
                <div class="icon">
                  <img src="../../assets/images/service-icon-01.png" alt="">
                </div>
              </div>
              <div class="col-lg-8">
                <div class="right-content">
                  <h4>Consultas Médicas</h4>
                  <p>Consultas com profissionais qualificados e prontos para cuidar de você.</p>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="col-lg-4" data-bs-toggle="modal" data-bs-target="#modalExame" style="cursor: pointer;">
          <div class="service-item wow bounceInUp" data-wow-duration="1s" data-wow-delay="0.4s">
            <div class="row">
              <div class="col-lg-4">
                <div class="icon">
                  <img src="../../assets/images/service-icon-02.png" alt="">
                </div>
              </div>
              <div class="col-lg-8">
                <div class="right-content">
                  <h4>Exames Laboratoriais</h4>
                  <p>Exames laboratoriais completos para diagnósticos seguros e precisos.</p>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="col-lg-4" data-bs-toggle="modal" data-bs-target="#modalEstetica" style="cursor: pointer;">
          <div class="service-item wow bounceInUp" data-wow-duration="1s" data-wow-delay="0.5s">
            <div class="row">
              <div class="col-lg-4">
                <div class="icon">
                  <img src="../../assets/images/service-icon-03.png" alt="">
                </div>
              </div>
              <div class="col-lg-8">
                <div class="right-content">
                  <h4>Estética</h4>
                  <p>Serviços de estética para realçar sua beleza e promover bem-estar.</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- <div id="features" class="features section">
    <div class="container">
      <div class="row">
        <div class="col-lg-12">
          <div class="features-content">
            <div class="row">
              <div class="col-lg-3">
                <div class="features-item first-feature wow fadeInUp" data-wow-duration="1s" data-wow-delay="0s">
                  <div class="first-number number">
                    <h6>01</h6>
                  </div>
                  <div class="icon"></div>
                  <h4>Reach Out</h4>
                  <div class="line-dec"></div>
                  <p>This HTML5 template is based on Bootstrap 5 CSS. You are free to customize anything.</p>
                </div>
              </div>
              <div class="col-lg-3">
                <div class="features-item second-feature wow fadeInUp" data-wow-duration="1s" data-wow-delay="0.2s">
                  <div class="second-number number">
                    <h6>02</h6>
                  </div>
                  <div class="icon"></div>
                  <h4>Develop a Strategy</h4>
                  <div class="line-dec"></div>
                  <p>Lorem ipsum dolor sit ameter consectetur adipiscing li elit sed do eiusmod.</p>
                </div>
              </div>
              <div class="col-lg-3">
                <div class="features-item first-feature wow fadeInUp" data-wow-duration="1s" data-wow-delay="0.4s">
                  <div class="third-number number">
                    <h6>03</h6>
                  </div>
                  <div class="icon"></div>
                  <h4>Implementation</h4>
                  <div class="line-dec"></div>
                  <p>If this template is useful for your website, please consider to <a rel="nofollow" href="https://www.paypal.me/templatemo" target="_blank">support us</a> a little.</p>
                </div>
              </div>
              <div class="col-lg-3">
                <div class="features-item second-feature last-features-item wow fadeInUp" data-wow-duration="1s" data-wow-delay="0.6s">
                  <div class="fourth-number number">
                    <h6>04</h6>
                  </div>
                  <div class="icon"></div>
                  <h4>Analyze the result</h4>
                  <div class="line-dec"></div>
                  <p>Below circular progress bar animation supports those CSS values 10, 20, 30, till 100.</p>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="col-lg-12">
          <div class="skills-content">
            <div class="row">
              <div class="col-lg-3">
                <div class="skill-item wow fadeIn" data-wow-duration="1s" data-wow-delay="0s">
                  <div class="progress" data-percentage="80">
                    <span class="progress-left">
                      <span class="progress-bar"></span>
                    </span>
                    <span class="progress-right">
                      <span class="progress-bar"></span>
                    </span>
                    <div class="progress-value">
                      <div>
                        80%<br>
                        <span>HTML/CSS/JS</span>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
              <div class="col-lg-3">
                <div class="skill-item wow fadeIn" data-wow-duration="1s" data-wow-delay="0.2s">
                  <div class="progress" data-percentage="60">
                    <span class="progress-left">
                      <span class="progress-bar"></span>
                    </span>
                    <span class="progress-right">
                      <span class="progress-bar"></span>
                    </span>
                    <div class="progress-value">
                      <div>
                        60%<br>
                        <span>Wordpress</span>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
              <div class="col-lg-3">
                <div class="skill-item wow fadeIn" data-wow-duration="1s" data-wow-delay="0.4s">
                  <div class="progress" data-percentage="90">
                    <span class="progress-left">
                      <span class="progress-bar"></span>
                    </span>
                    <span class="progress-right">
                      <span class="progress-bar"></span>
                    </span>
                    <div class="progress-value">
                      <div>
                        90%<br>
                        <span>Marketing</span>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
              <div class="col-lg-3">
                <div class="skill-item last-skill-item wow fadeIn" data-wow-duration="1s" data-wow-delay="0.6s">
                  <div class="progress" data-percentage="70">
                    <span class="progress-left">
                      <span class="progress-bar"></span>
                    </span>
                    <span class="progress-right">
                      <span class="progress-bar"></span>
                    </span>
                    <div class="progress-value">
                      <div>
                        70%<br>
                        <span>Photoshop</span>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div> -->

  <div id="about" class="about-us section">
    <div class="container">
      <div class="row">
        <div class="col-lg-6">
          <div class="left-image wow fadeInLeft" data-wow-duration="1s" data-wow-delay="0.5s">
            <img src="../../assets/images/about-left-image.png" alt="">
          </div>
        </div>
        <div class="col-lg-6 align-self-center wow fadeInRight" data-wow-duration="1s" data-wow-delay="0.5s">
          <div class="section-heading">
            <h6>About Us</h6>
            <h2>Top <em>marketing</em> agency &amp; consult your website <span>with us</span></h2>
          </div>
          <div class="row">
            <div class="col-lg-4 col-sm-4">
              <div class="about-item">
                <h4>750+</h4>
                <h6>projects finished</h6>
              </div>
            </div>
            <div class="col-lg-4 col-sm-4">
              <div class="about-item">
                <h4>340+</h4>
                <h6>happy clients</h6>
              </div>
            </div>
            <div class="col-lg-4 col-sm-4">
              <div class="about-item">
                <h4>128+</h4>
                <h6>awards</h6>
              </div>
            </div>
          </div>
          <p><a rel="nofollow" href="https://templatemo.com/tm-563-seo-dream" target="_parent">SEO Dream</a> is free
            digital marketing CSS template provided by TemplateMo website. You are allowed to use this template for your
            business websites. Please DO NOT redistribute this template ZIP file on any Free CSS collection websites.
            You may contact us for more information. Thank you.</p>
          <div class="main-green-button"><a href="#">Discover company</a></div>
        </div>
      </div>
    </div>
  </div>

  <div id="services" class="our-services section">
    <div class="container">
      <div class="row">
        <div class="col-lg-6 offset-lg-3">
          <div class="section-heading wow bounceIn" data-wow-duration="1s" data-wow-delay="0.2s">
            <h6>Our Services</h6>
            <h2>Discover What We Do &amp; <span>Offer</span> To Our <em>Clients</em></h2>
          </div>
        </div>
      </div>
    </div>
    <div class="container-fluid">
      <div class="row">
        <div class="col-lg-4">
          <div class="service-item wow bounceInUp" data-wow-duration="1s" data-wow-delay="0.3s">
            <div class="row">
              <div class="col-lg-4">
                <div class="icon">
                  <img src="../../assets/images/service-icon-01.png" alt="">
                </div>
              </div>
              <div class="col-lg-8">
                <div class="right-content">
                  <h4>Similar Websites</h4>
                  <p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium dormque laudantium.</p>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="col-lg-4">
          <div class="service-item wow bounceInUp" data-wow-duration="1s" data-wow-delay="0.4s">
            <div class="row">
              <div class="col-lg-4">
                <div class="icon">
                  <img src="../../assets/images/service-icon-02.png" alt="">
                </div>
              </div>
              <div class="col-lg-8">
                <div class="right-content">
                  <h4>Website Trends</h4>
                  <p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium dormque laudantium.</p>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="col-lg-4">
          <div class="service-item wow bounceInUp" data-wow-duration="1s" data-wow-delay="0.5s">
            <div class="row">
              <div class="col-lg-4">
                <div class="icon">
                  <img src="../../assets/images/service-icon-03.png" alt="">
                </div>
              </div>
              <div class="col-lg-8">
                <div class="right-content">
                  <h4>Traffic Analysis</h4>
                  <p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium dormque laudantium.</p>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="col-lg-4">
          <div class="service-item wow bounceInUp" data-wow-duration="1s" data-wow-delay="0.6s">
            <div class="row">
              <div class="col-lg-4">
                <div class="icon">
                  <img src="../../assets/images/service-icon-03.png" alt="">
                </div>
              </div>
              <div class="col-lg-8">
                <div class="right-content">
                  <h4>Optimizing Keywords</h4>
                  <p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium dormque laudantium.</p>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="col-lg-4">
          <div class="service-item wow bounceInUp" data-wow-duration="1s" data-wow-delay="0.7s">
            <div class="row">
              <div class="col-lg-4">
                <div class="icon">
                  <img src="../../assets/images/service-icon-01.png" alt="">
                </div>
              </div>
              <div class="col-lg-8">
                <div class="right-content">
                  <h4>Page Optimizations</h4>
                  <p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium dormque laudantium.</p>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="col-lg-4">
          <div class="service-item wow bounceInUp" data-wow-duration="1s" data-wow-delay="0.8s">
            <div class="row">
              <div class="col-lg-4">
                <div class="icon">
                  <img src="../../assets/images/service-icon-02.png" alt="">
                </div>
              </div>
              <div class="col-lg-8">
                <div class="right-content">
                  <h4>Deep URL Analysis</h4>
                  <p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium dormque laudantium.</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>

  <div id="portfolio" class="our-portfolio section">
    <div class="container">
      <div class="row">
        <div class="col-lg-5">
          <div class="section-heading wow fadeInLeft" data-wow-duration="1s" data-wow-delay="0.3s">
            <h6>Our Portofolio</h6>
            <h2>Discover Our Recent <em>Projects</em> And <span>Showcases</span></h2>
          </div>
        </div>
      </div>
    </div>
    <div class="container-fluid wow fadeIn" data-wow-duration="1s" data-wow-delay="0.7s">
      <div class="row">
        <div class="col-lg-12">
          <div class="loop owl-carousel">
            <div class="item">
              <div class="portfolio-item">
                <div class="thumb">
                  <img src="../../assets/images/portfolio-01.jpg" alt="">
                  <div class="hover-content">
                    <div class="inner-content">
                      <a href="#">
                        <h4>Awesome Project 101</h4>
                      </a>
                      <span>Marketing</span>
                    </div>
                  </div>
                </div>
              </div>
              <div class="portfolio-item">
                <div class="thumb">
                  <img src="../../assets/images/portfolio-04.jpg" alt="">
                  <div class="hover-content">
                    <div class="inner-content">
                      <a href="#">
                        <h4>Awesome Project 102</h4>
                      </a>
                      <span>Branding</span>
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <div class="item">
              <div class="portfolio-item">
                <div class="thumb">
                  <img src="../../assets/images/portfolio-02.jpg" alt="">
                  <div class="hover-content">
                    <div class="inner-content">
                      <a href="#">
                        <h4>Awesome Project 103</h4>
                      </a>
                      <span>Consulting</span>
                    </div>
                  </div>
                </div>
              </div>
              <div class="portfolio-item">
                <div class="thumb">
                  <img src="../../assets/images/portfolio-05.jpg" alt="">
                  <div class="hover-content">
                    <div class="inner-content">
                      <a href="#">
                        <h4>Awesome Project 104</h4>
                      </a>
                      <span>Artwork</span>
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <div class="item">
              <div class="portfolio-item">
                <div class="thumb">
                  <img src="../../assets/images/portfolio-03.jpg" alt="">
                  <div class="hover-content">
                    <div class="inner-content">
                      <a href="#">
                        <h4>Awesome Project 105</h4>
                      </a>
                      <span>Branding</span>
                    </div>
                  </div>
                </div>
              </div>
              <div class="portfolio-item">
                <div class="thumb">
                  <img src="../../assets/images/portfolio-06.jpg" alt="">
                  <div class="hover-content">
                    <div class="inner-content">
                      <a href="#">
                        <h4>Awesome Project 106</h4>
                      </a>
                      <span>Artwork</span>
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <div class="item">
              <div class="portfolio-item">
                <div class="thumb">
                  <img src="../../assets/images/portfolio-04.jpg" alt="">
                  <div class="hover-content">
                    <div class="inner-content">
                      <a href="#">
                        <h4>Awesome Project 107</h4>
                      </a>
                      <span>Creative</span>
                    </div>
                  </div>
                </div>
              </div>
              <div class="portfolio-item">
                <div class="thumb">
                  <img src="../../assets/images/portfolio-01.jpg" alt="">
                  <div class="hover-content">
                    <div class="inner-content">
                      <a href="#">
                        <h4>Awesome Project 108</h4>
                      </a>
                      <span>Consulting</span>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>

  <div id="contact" class="contact-us section">
    <div class="container">
      <div class="row">
        <div class="col-lg-12 wow fadeInUp" data-wow-duration="0.5s" data-wow-delay="0.25s">
          <form id="contact" action="" method="post">
            <div class="row">
              <div class="col-lg-6 offset-lg-3">
                <div class="section-heading">
                  <h6>Contact Us</h6>
                  <h2>Fill Out The Form Below To <span>Get</span> In <em>Touch</em> With Us</h2>
                </div>
              </div>
              <div class="col-lg-9">
                <div class="row">
                  <div class="col-lg-6">
                    <fieldset>
                      <input type="name" name="name" id="name" placeholder="Name" autocomplete="on" required>
                    </fieldset>
                  </div>
                  <div class="col-lg-6">
                    <fieldset>
                      <input type="surname" name="surname" id="surname" placeholder="Surname" autocomplete="on"
                        required>
                    </fieldset>
                  </div>
                  <div class="col-lg-6">
                    <fieldset>
                      <input type="text" name="email" id="email" pattern="[^ @]*@[^ @]*" placeholder="Your Email"
                        required="">
                    </fieldset>
                  </div>
                  <div class="col-lg-6">
                    <fieldset>
                      <input type="subject" name="subject" id="subject" placeholder="Subject" autocomplete="on">
                    </fieldset>
                  </div>
                  <div class="col-lg-12">
                    <fieldset>
                      <textarea name="message" type="text" class="form-control" id="message" placeholder="Message"
                        required=""></textarea>
                    </fieldset>
                  </div>
                  <div class="col-lg-12">
                    <fieldset>
                      <button type="submit" id="form-submit" class="main-button ">Send Message Now</button>
                    </fieldset>
                  </div>
                </div>
              </div>
              <div class="col-lg-3">
                <div class="contact-info">
                  <ul>
                    <li>
                      <div class="icon">
                        <img src="../../assets/images/contact-icon-01.png" alt="email icon">
                      </div>
                      <a href="#">info@company.com</a>
                    </li>
                    <li>
                      <div class="icon">
                        <img src="../../assets/images/contact-icon-02.png" alt="phone">
                      </div>
                      <a href="#">+001-002-0034</a>
                    </li>
                    <li>
                      <div class="icon">
                        <img src="../../assets/images/contact-icon-03.png" alt="location">
                      </div>
                      <a href="#">26th Street, Digital Villa</a>
                    </li>
                  </ul>
                </div>
              </div>
            </div>
          </form>
        </div>
      </div>
    </div>
  </div>

  <footer>
    <div class="container">
      <div class="row">
        <div class="col-lg-12">
          <p>Copyright © 2021 SEO Dream Co., Ltd. All Rights Reserved.

            <br>Web Designed by <a rel="nofollow" href="https://templatemo.com"
              title="free CSS templates">TemplateMo</a>
          </p>
        </div>
      </div>
    </div>
  </footer>

  // #region Modals
  <!-- Modal -->
  <div class="modal fade" id="modalConsulta" tabindex="-1" aria-labelledby="modalConsultaLabel" aria-hidden="true">
    <div class="modal-dialog modal-dialog-centered modal-dialog-scrollable modal-xl">
      <div class="modal-content">
        <!-- <div class="modal-header">
          <h5 class="modal-title" id="modalConsultaLabel">Consultas Médicas</h5>
          <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
        </div> -->
        <div class="modal-body">
          <U3Carousel :slides="slidesConsulta"></U3Carousel>
        </div>
        <!-- <div class="modal-footer">
          <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Fechar</button>
          <button type="button" class="btn btn-primary">Salvar mudanças</button>
        </div> -->
      </div>
    </div>
  </div>

  <div class="modal fade" id="modalExame" tabindex="-2" aria-labelledby="modalExameLabel" aria-hidden="true">
    <div class="modal-dialog modal-dialog-centered modal-dialog-scrollable modal-xl">
      <div class="modal-content">

        <div class="modal-body">
          <U3Carousel :slides="slidesExame"></U3Carousel>
        </div>

      </div>
    </div>
  </div>

  <div class="modal fade" id="modalEstetica" tabindex="-3" aria-labelledby="modalEsteticaLabel" aria-hidden="true">
    <div class="modal-dialog modal-dialog-centered modal-dialog-scrollable modal-xl">
      <div class="modal-content">

        <div class="modal-body">
          <U3Carousel :slides="slidesEstetica"></U3Carousel>
        </div>

      </div>
    </div>
  </div>

  // #endregion Modals
</template>

<style scoped lang="scss">
@use '../../style.scss';
</style>

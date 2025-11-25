
<html lang="hi">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Motion Detector — सरल और विस्तृत मार्गदर्शिका | Brocool</title>
  <meta name="description" content="Motion Detector क्या है, कैसे काम करता है, इसके प्रकार, उपयोग, DIY प्रोजेक्ट, installation tips और आम समस्याएँ — बच्चों और आरम्भिक उपयोगकर्ताओं के लिए सरल भाषा में।" />
  <meta name="keywords" content="motion detector, motion sensor, PIR, ultrasonic, microwave sensor, Brocool, स्मार्ट होम, DIY, PIR sensor, Arduino sensor" />
  <meta name="author" content="Pravin / Brocool" />
  <meta name="robots" content="index, follow" />
  
  <!-- Open Graph / Twitter -->
  <meta property="og:title" content="Motion Detector — सरल और विस्तृत मार्गदर्शिका | Brocool" />
  <meta property="og:description" content="Motion Detector क्या है, कैसे काम करता है, प्रकार, उपयोग और DIY प्रोजेक्ट — आसान भाषा में।" />
  <meta property="og:image" content="https://images.unsplash.com/photo-1558089687-b23f0c311e62?ixlib=rb-4.0.3&auto=format&fit=crop&w=1200&q=80" />
  <meta property="og:type" content="article" />
  <meta property="og:url" content="https://brocool.in/motion-detector-guide.html" />
  <meta name="twitter:card" content="summary_large_image" />
  <meta name="twitter:title" content="Motion Detector — सरल और विस्तृत मार्गदर्शिका | Brocool" />
  <meta name="twitter:description" content="Motion Detector क्या है, कैसे काम करता है, प्रकार, उपयोग और DIY प्रोजेक्ट — आसान भाषा में।" />

  <!-- Structured data -->
  <script type="application/ld+json">
  {
    "@context": "https://schema.org",
    "@type": "Article",
    "headline": "Motion Detector — सरल और विस्तृत मार्गदर्शिका",
    "description": "Motion Detector क्या है, कैसे काम करता है, प्रकार, उपयोग और DIY प्रोजेक्ट — आसान भाषा में।",
    "author": {"@type":"Person","name":"Pravin / Brocool"},
    "publisher": {"@type":"Organization","name":"Brocool","logo":{"@type":"ImageObject","url":"https://brocool.in/logo.png"}},
    "datePublished": "2025-11-25",
    "dateModified": "2025-11-25",
    "mainEntityOfPage": {"@type":"WebPage","@id":"https://brocool.in/motion-detector-guide.html"},
    "image": "https://images.unsplash.com/photo-1558089687-b23f0c311e62?ixlib=rb-4.0.3&auto=format&fit=crop&w=1200&q=80"
  }
  </script>

  <!-- AdSense placeholder (replace publisher id) -->
  <!-- NOTE: change ca-pub- 4319423225607012 to your AdSense ID -->
  <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-4319423225607012" crossorigin="anonymous"></script>

  <style>
    :root{
      --bg: linear-gradient(180deg,#f7fbff,#f0fcf8);
      --card:#ffffff;
      --muted:#5b7d82;
      --accent1:#06b6d4;
      --accent2:#7c3aed;
      --radius:14px;
      --maxw:980px;
      font-family: "Inter", system-ui, -apple-system, "Segoe UI", Roboto, "Noto Sans", "Helvetica Neue", Arial;
    }
    *{box-sizing:border-box}
    body{margin:0;background:var(--bg);padding:28px;display:flex;justify-content:center;color:#05323a;}
    .wrap{max-width:var(--maxw);width:100%}
    header{display:flex;align-items:center;gap:14px;margin-bottom:16px}
    .logo{width:60px;height:60px;border-radius:12px;background:linear-gradient(135deg,var(--accent1),var(--accent2));display:flex;align-items:center;justify-content:center;color:#012;font-weight:800}
    .title{font-size:20px;font-weight:1200}
    .subtitle{font-size:13px;color:var(--muted)}
    .card{background:var(--card);padding:22px;border-radius:var(--radius);box-shadow:0 8px 30px rgba(4,20,30,0.06)}
    .hero{display:grid;grid-template-columns:1fr 260px;gap:18px;align-items:start}
    @media(max-width:920px){.hero{grid-template-columns:1fr}}
    .hero .main-img{width:100%;height:260px;object-fit:cover;border-radius:10px}
    h1{margin:0 0 6px 0;font-size:26px}
    .meta{color:var(--muted);font-size:13px;margin-bottom:12px}
    .toc{background:linear-gradient(90deg,rgba(6,182,212,0.06),rgba(124,58,237,0.03));padding:12px;border-radius:10px}
    .toc a{display:block;color:var(--accent2);text-decoration:none;padding:6px 0}
    .content{margin-top:18px;line-height:1.8;color:#07323a}
    .section{margin:26px 0}
    .section h2{margin:0 0 10px 0;font-size:20px}
    
    /* Image Styles */
    .image-grid{display:grid;grid-template-columns:repeat(2,1fr);gap:12px;margin:16px 0}
    .image-card{background:var(--card);padding:12px;border-radius:10px;text-align:center;border:1px solid rgba(0,0,0,0.05)}
    .image-card img{width:100%;height:140px;object-fit:cover;border-radius:8px}
    .image-card .caption{font-size:12px;color:var(--muted);margin-top:6px}
    
    ul{margin-left:18px}
    .controls{display:flex;gap:10px;align-items:center;margin-bottom:16px}
    .btn{padding:8px 12px;border-radius:10px;border:none;background:linear-gradient(90deg,var(--accent1),var(--accent2));color:#012;font-weight:700;cursor:pointer}
    .small{font-size:13px;color:var(--muted)}
    .adbox{display:block;text-align:center;padding:12px;margin:16px 0;border-radius:10px;background:linear-gradient(180deg,rgba(3,105,118,0.03),rgba(124,58,237,0.02));color:var(--muted);border:1px dashed var(--accent1)}
    .backlink{display:inline-block;margin-top:10px;text-decoration:none;color:var(--accent2);font-weight:700}
    footer{margin-top:20px;color:var(--muted);font-size:13px;text-align:center}
    mark{background:linear-gradient(90deg,#fff7cc,#ffe4b5);padding:3px 6px;border-radius:6px}
    
    /* AdSense responsive ads */
    .adsbygoogle {
      display: block;
      margin: 20px 0;
      border-radius: 8px;
      overflow: hidden;
    }
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <div class="logo">BC</div>
      <div>
        <div class="title">Motion Detector — सरल और विस्तृत मार्गदर्शिका</div>
        <div class="subtitle">Brocool • आसान भाषा में टेक्नोलॉजी</div>
      </div>
    </header>

    <article class="card" id="post">
      <div class="hero">
        <img class="main-img" src="https://images.unsplash.com/photo-1558089687-b23f0c311e62?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Motion detector technology" />
        <aside class="toc">
          <div style="font-weight:800;margin-bottom:8px">इस पोस्ट में</div>
          <a href="#sec1">1. Motion Detector क्या है?</a>
          <a href="#sec2">2. कैसे काम करता है</a>
          <a href="#sec3">3. प्रमुख प्रकार</a>
          <a href="#sec4">4. उपयोग और Installation</a>
          <a href="#sec5">5. DIY प्रोजेक्ट</a>
          <div style="margin-top:12px" class="small">Published: 25 Nov 2025 • पढ़ने का समय: ~8-10 मिनट</div>
        </aside>
      </div>

      <div class="content">
        <!-- AdSense Header Ad -->
        <ins class="adsbygoogle"
             style="display:block"
             data-ad-client="ca-pub-4319423225607012"
             data-ad-slot="1234567890"
             data-ad-format="auto"
             data-full-width-responsive="true"></ins>
        <script>
             (adsbygoogle = window.adsbygoogle || []).push({});
        </script>

        <!-- SECTION 1 -->
        <section id="sec1" class="section">
          <h2>1. Motion Detector क्या है?</h2>
          <p><strong>Motion Detector</strong> एक ऐसा डिवाइस है जो उसके सामने होने वाली गतिविधि (movement) का पता लगाता है। यह सरल शब्दों में 'नज़र रखने वाला छोटा चश्मा' है — जो किसी स्थान में कोई हरकत होने पर signal देता है। आधुनिक घरों में motion detector लाइट्स, security cameras, alarm systems, और smart home automation का मुख्य भाग बन चुके हैं।</p>

          <div class="image-grid">
            <div class="image-card">
              <img src="https://images.unsplash.com/photo-1581094794329-c8112a89af12?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80" alt="PIR Sensor Module" />
              <div class="caption">PIR Sensor Module</div>
            </div>
            <div class="image-card">
              <img src="https://images.unsplash.com/photo-1558618666-fcd25856cd63?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80" alt="Motion Activated Light" />
              <div class="caption">Motion Activated Light</div>
            </div>
          </div>

          <p>बच्चों के लिए आसान समझ: मान लीजिए कमरे में एक sentinel बैठा है — जब कोई चलता है तो वह चिल्लाकर कहता है "कोई आया!" — और फिर एक light या कैमरा अपने-आप चालू हो जाता है। यही कार्य motion detector करता है।</p>
        </section>

        <!-- SECTION 2 -->
        <section id="sec2" class="section">
          <h2>2. कैसे काम करता है — तकनीक और सिद्धांत</h2>
          <p>Motion detectors अलग-अलग तरीकों से काम कर सकते हैं, पर मुख्य उद्देश्य है: <em>परिवर्तन</em> (change) को पकड़ना — यह परिवर्तन वातावरण में किसी चीज़ के आने से होता है।</p>

          <div class="image-card" style="max-width:400px;margin:12px 0">
            <img src="https://images.unsplash.com/photo-1562408590-e32931084e23?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80" alt="Ultrasonic Sensor Working" />
            <div class="caption">Ultrasonic Sensor - Sound Waves</div>
          </div>

          <p>कुछ आम तरीके:</p>
          <ul>
            <li><strong>Temperature-based detection</strong>: जब कोई इंसान आता है तो उसका body-heat आसपास के तापमान को बदलता है — इसे PIR sensors detect करते हैं।</li>
            <li><strong>Sound/echo based</strong>: Ultrasonic sensors high-frequency waves भेजते हैं और echo timing में बदलाव से movement समझते हैं।</li>
            <li><strong>Radio wave based</strong>: Microwave sensors micro-waves भेजते और वापस आने वाले signal में बदलाव पकड़ते हैं — दूर तक और तेज़ गति वाले movements के लिए उपयोगी।</li>
          </ul>
        </section>

        <!-- AdSense In-Article Ad -->
        <ins class="adsbygoogle"
             style="display:block; text-align:center;"
             data-ad-layout="in-article"
             data-ad-format="fluid"
             data-ad-client="ca-pub-4319423225607012"
             data-ad-slot="9876543210"></ins>
        <script>
             (adsbygoogle = window.adsbygoogle || []).push({});
        </script>

        <!-- SECTION 3 -->
        <section id="sec3" class="section">
          <h2>3. प्रमुख प्रकार — PIR, Ultrasonic, Microwave</h2>

          <div class="image-grid">
            <div class="image-card">
              <img src="https://images.unsplash.com/photo-1597852075232-839700f7f28e?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80" alt="Security Camera with Motion Detection" />
              <div class="caption">Security Camera with Motion Detection</div>
            </div>
            <div class="image-card">
              <img src="https://images.unsplash.com/photo-1507146153580-69a1fe6d8aa1?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80" alt="DIY Electronics Project" />
              <div class="caption">DIY Electronics Project</div>
            </div>
          </div>

          <p><strong>PIR (Passive Infrared):</strong> सबसे आम। यह active नहीं होता — सिर्फ infrared radiation (body heat) को पढ़ता है। घरों की automated lights, corridor sensors और basic alarm systems में PIR बहुत प्रचलित है।</p>

          <p><strong>Ultrasonic:</strong> ultrasound pulses भेजकर distance बदलने पर detect करता है। बड़े खुले क्षेत्र में echo clutter हो सकता है; पर confined spaces में अच्छा काम करता है।</p>

          <p><strong>Microwave:</strong> Doppler effect पर काम करता है — micro waves भेजकर समय/phase में बदलाव detect करता है। यह दीवारों के पीछे से भी movement detect कर सकता है।</p>
        </section>

        <!-- SECTION 4 -->
        <section id="sec4" class="section">
          <h2>4. उपयोग, Installation और सुरक्षा सम्मत सुझाव</h2>

          <p><strong>कहाँ-कहाँ उपयोग होता है:</strong> घर की lights, street lighting, CCTV, store automatic doors, energy-saving HVAC control, और interactive exhibits आदि।</p>

          <div class="image-card" style="max-width:500px;margin:12px 0">
            <img src="https://images.unsplash.com/photo-1558089687-b23f0c311e62?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80" alt="Smart Home Automation" />
            <div class="caption">Smart Home Automation System</div>
          </div>

          <p><strong>Installation tips:</strong></p>
          <ul>
            <li>ऊँचाई और angle चुनें — आमतौर पर 2.1–2.5 मीटर से अच्छा कवरेज मिलता है।</li>
            <li>PIR को heater, AC vents और direct sunlight से दूर रखें।</li>
            <li>Microwave sensors को sensitive एरिया में अधिक सावधानी से लगाएँ</li>
          </ul>
        </section>

        <!-- AdSense Bottom Ad -->
        <ins class="adsbygoogle"
             style="display:block"
             data-ad-client="ca-pub-4319423225607012"
             data-ad-slot="5678901234"
             data-ad-format="auto"
             data-full-width-responsive="true"></ins>
        <script>
             (adsbygoogle = window.adsbygoogle || []).push({});
        </script>

        <!-- SECTION 5 -->
        <section id="sec5" class="section">
          <h2>5. DIY प्रोजेक्ट, Troubleshooting और अंतिम सुझाव</h2>

          <p><strong>Simple DIY (बच्चों के साथ):</strong> एक छोटा automatic night-light बनाना आसान है — सामग्री: PIR module (HC-SR501), LED, 220Ω resistor, breadboard, और एक 5V power supply (USB)। PIR जब motion detect करता है तो LED ON रहेगा कुछ seconds के लिए।</p>

          <div class="image-card" style="max-width:400px;margin:12px 0">
            <img src="https://images.unsplash.com/photo-1507146153580-69a1fe6d8aa1?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80" alt="Arduino PIR Project" />
            <div class="caption">Arduino with PIR Sensor</div>
          </div>

          <p><strong>Troubleshooting सामान्य समस्याएँ:</strong></p>
          <ul>
            <li>False triggers: sources — heater, sunlight, pets</li>
            <li>No detection: wiring या power issue</li>
            <li>Intermittent behavior: firmware/ageing या electrical noise</li>
          </ul>

          <a class="backlink" href="index.html">← Brocool मुख्य पेज पर वापस जाएँ</a>
        </section>

        <hr />

        <footer>
          <div class="small">© Brocool • Pravin — Motion Detector Guide • Published: 25 Nov 2025</div>
          <div class="small">Brocool - Technology for Everyone | आसान भाषा में टेक्नोलॉजी</div>
        </footer>
      </div>
    </article>
  </div>

  <script>
    // AdSense initialization
    (function(){
      // Smooth scrolling for TOC links
      document.querySelectorAll('.toc a').forEach(a => {
        a.addEventListener('click', (e) => {
          e.preventDefault();
          const target = document.querySelector(a.getAttribute('href'));
          if(target){
            window.scrollTo({
              top: target.offsetTop - 20,
              behavior: 'smooth'
            });
          }
        });
      });

      // Initialize AdSense (if not already done)
      if(window.adsbygoogle){
        (adsbygoogle = window.adsbygoogle || []).push({});
      }
    })();
  </script>
</body>
</html>

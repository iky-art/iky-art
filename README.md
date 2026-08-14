<!--
  README.md for: iky-art
  Style: Dark · Futuristic · 3D · CLI · Minimal · Premium
  Single code block — drop this entire content into README.md
-->

<div align="center">

<!-- 3D HERO SVG -->
<svg width="100%" height="360" viewBox="0 0 1200 360" preserveAspectRatio="xMidYMid slice" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="IKY 3D Hero">
  <defs>
    <linearGradient id="bgGrad" x1="0" x2="1">
      <stop offset="0" stop-color="#050505"/>
      <stop offset="1" stop-color="#0A0A0A"/>
    </linearGradient>

    <linearGradient id="neon" x1="0" x2="1">
      <stop offset="0" stop-color="#6366F1"/>
      <stop offset="0.5" stop-color="#8B5CF6"/>
      <stop offset="1" stop-color="#00D4FF"/>
    </linearGradient>

    <radialGradient id="glow" cx="50%" cy="30%" r="50%">
      <stop offset="0%" stop-color="#00D4FF" stop-opacity="0.25"/>
      <stop offset="50%" stop-color="#8B5CF6" stop-opacity="0.08"/>
      <stop offset="100%" stop-color="#050505" stop-opacity="0"/>
    </radialGradient>

    <filter id="softGlow" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="8" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>

    <!-- wireframe sphere stroke -->
    <linearGradient id="wireStroke" x1="0" x2="1">
      <stop offset="0" stop-color="#00D4FF"/>
      <stop offset="1" stop-color="#8B5CF6"/>
    </linearGradient>

    <!-- grid pattern -->
    <pattern id="grid" width="40" height="40" patternUnits="userSpaceOnUse">
      <path d="M40 0 L0 0 0 40" fill="none" stroke="#0E0E0E" stroke-width="0.6"/>
    </pattern>

    <!-- subtle vignette -->
    <radialGradient id="vignette" cx="50%" cy="50%">
      <stop offset="60%" stop-color="#000000" stop-opacity="0"/>
      <stop offset="100%" stop-color="#000000" stop-opacity="0.45"/>
    </radialGradient>
  </defs>

  <!-- background -->
  <rect width="100%" height="100%" fill="url(#bgGrad)"/>
  <rect width="100%" height="100%" fill="url(#vignette)" />

  <!-- perspective grid -->
  <g transform="translate(0,180) scale(1,0.6)">
    <rect x="0" y="0" width="1200" height="180" fill="url(#grid)" opacity="0.28" />
    <!-- perspective lines -->
    <g stroke="#071023" stroke-width="1" opacity="0.45">
      <!-- radial vanishing lines -->
      <path d="M600 0 L600 180" stroke="#071023"/>
      <path d="M600 0 L900 180" stroke="#08102A" />
      <path d="M600 0 L300 180" stroke="#08102A" />
      <path d="M600 0 L1200 180" stroke="#06101B" />
      <path d="M600 0 L0 180" stroke="#06101B" />
    </g>
  </g>

  <!-- floating isometric cube (left) -->
  <g transform="translate(180,120) scale(0.9) rotate(-12)">
    <polygon points="0,30 45,0 90,30 45,60" fill="rgba(139,92,246,0.06)"/>
    <polygon points="0,30 45,60 45,120 0,90" fill="rgba(99,102,241,0.04)"/>
    <polygon points="90,30 45,60 45,120 90,90" fill="rgba(0,212,255,0.03)"/>
    <polygon points="0,30 45,0 45,60 0,90" stroke="url(#neon)" stroke-width="1.4" fill="none" opacity="0.9"/>
  </g>

  <!-- wireframe sphere (center) -->
  <g transform="translate(620,140)" filter="url(#softGlow)">
    <!-- glow under sphere -->
    <ellipse cx="0" cy="120" rx="220" ry="30" fill="url(#glow)" opacity="0.18" />
    <!-- latitudes -->
    <g stroke="url(#wireStroke)" stroke-width="1.1" fill="none">
      <ellipse rx="120" ry="60" transform="rotate(0)" opacity="0.55"/>
      <ellipse rx="120" ry="40" transform="rotate(14)" opacity="0.38"/>
      <ellipse rx="120" ry="20" transform="rotate(-14)" opacity="0.26"/>
      <ellipse rx="120" ry="5" transform="rotate(28)" opacity="0.16"/>
      <!-- longitudes via rotated paths -->
      <g stroke-width="0.9" opacity="0.7">
        <path d="M-120 0 A120 120 0 0 0 120 0" transform="scale(1,0.6)"/>
        <path d="M-120 10 A120 120 0 0 0 120 10" transform="rotate(22) scale(1,0.6)"/>
        <path d="M-120 -10 A120 120 0 0 0 120 -10" transform="rotate(-22) scale(1,0.6)"/>
        <path d="M-120 20 A120 120 0 0 0 120 20" transform="rotate(44) scale(1,0.6)" opacity="0.5"/>
      </g>
    </g>
    <!-- small floating nodes -->
    <g fill="#00D4FF" opacity="0.9">
      <circle cx="-62" cy="-28" r="3.6"/>
      <circle cx="84" cy="-8" r="3.2"/>
      <circle cx="26" cy="34" r="2.8"/>
    </g>
  </g>

  <!-- floating holographic panel (right) -->
  <g transform="translate(940,80)">
    <rect x="-20" y="-40" width="240" height="140" rx="12" fill="#0A0A0A" stroke="url(#neon)" stroke-opacity="0.12" stroke-width="1.6"/>
    <rect x="-14" y="-34" width="228" height="54" rx="8" fill="#0B0B0B" opacity="0.9"/>
    <text x="10" y="-8" fill="#00D4FF" font-family="monospace" font-size="12">SYSTEM • IKY</text>
    <g transform="translate(10,10)">
      <rect x="0" y="0" width="200" height="6" rx="3" fill="#111111" />
      <rect x="0" y="16" width="200" height="6" rx="3" fill="#0D0D0D"/>
      <rect x="0" y="32" width="120" height="6" rx="3" fill="#080808"/>
      <g fill="none" stroke="url(#neon)" stroke-width="0.8" opacity="0.5">
        <path d="M0 0 L200 0" />
        <path d="M0 16 L200 16" />
        <path d="M0 32 L200 32" />
      </g>
    </g>
  </g>

  <!-- title overlay -->
  <g transform="translate(600,46)">
    <text x="0" y="0" text-anchor="middle" font-family="Inter, Roboto, Helvetica, Arial, sans-serif" font-size="36" fill="#E6E6F6" font-weight="700">IKY</text>
    <text x="0" y="34" text-anchor="middle" font-family="Inter, Roboto, monospace" font-size="14" fill="#9AA0FF" letter-spacing="3">FULL-STACK DEVELOPER</text>
    <text x="0" y="56" text-anchor="middle" font-family="Inter, Roboto, monospace" font-size="12" fill="#A6F1FF" opacity="0.88">WEB • AI • DEVELOPER TOOLS • CREATIVE TECHNOLOGY</text>
  </g>

</svg>

</div>

<!-- Quick intro -->
<p align="center">
  <b style="color:#8B5CF6">Iky</b> — Full-Stack Developer · Web · AI · 3D Web · Developer Tools
</p>

---

<!-- CLI ASCII ART (IKY) -->
<div align="left">

<pre style="background:#050505;border-radius:8px;padding:18px;color:#CFEFFF;border:1px solid rgba(99,102,241,0.06);font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, "Consolas", "Liberation Mono", monospace;">
  __ ___   __  __  ____ 
 / // _ \ / / / / / __ \
/ // // // /_/ / / / / /
/__\___/ \____/ /_/ /_/   IKY
</pre>

<pre style="background:#050505;border-radius:8px;padding:12px 18px;margin-top:8px;color:#A9B9FF;border:1px solid rgba(139,92,246,0.06);font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, "Consolas", "Liberation Mono", monospace;">
╭────────────────────────────────────────────────────────────╮
│ IKY CLI · Developer Environment                            │
├────────────────────────────────────────────────────────────┤
│ STATUS       : ONLINE                                      │
│ MODE         : BUILD                                       │
│ SYSTEM       : IKY                                         │
│ VERSION      : 1.0.0                                       │
│ FOCUS        : WEB / AI / TOOLS / 3D                       │
╰────────────────────────────────────────────────────────────╯
</pre>

</div>

---

<!-- Terminal-like interactive demo -->
<details open>
<summary><strong style="color:#8B5CF6">Simulated Terminal — try commands</strong></summary>

<div style="background:#050505;padding:14px;border-radius:8px;margin-top:10px;border:1px solid rgba(0,212,255,0.06);">
<pre style="color:#B8E9FF;font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, monospace;line-height:1.45;">
$ whoami
iky

$ role
Full-Stack Developer · Creative Developer

$ focus
Web • AI • Developer Tools • 3D Web • CLI

$ iky --about
I build web apps, AI integrations, developer tooling, and experimental 3D interfaces.
I design clean developer experiences with a futuristic aesthetic.

$ iky --stack
JavaScript • TypeScript • Python • PHP • Go • Rust • SQL
React • Vite • Tailwind • Node.js • Express • Laravel • MySQL • MongoDB • Supabase

$ iky --projects
> Apollo AI     · AI tools & document analysis
> NexForge      · Developer ecosystem & experiments
> CipherLab     · Cybersecurity learning platform
> SkyCast       · Modern weather PWA
> IKY Toolkit   · Developer toolkit / Acode plugin

$ status
SYSTEM: ONLINE  |  MODE: BUILDING  |  CREATIVITY: ACTIVE
</pre>
</div>
</details>

---

<!-- ABOUT ME -->
### whoami
Iky — I'm a Full-Stack & Creative Developer who builds elegant web applications, AI projects, developer tools, CLI utilities, and experimental 3D interfaces. I focus on performance, UX, and pushing modern developer experiences.

---

<!-- TECH STACK with icons (skillicons.dev) -->
### Tech Stack
<p>
  <img src="https://skillicons.dev/icons?i=js,ts,py,php,go,rust,sql,html,css,react,vite,tailwind,threejs,nodejs,express,laravel,mysql,mongodb,supabase,git,github,linux,vscode,vercel" alt="stack" />
</p>

---

<!-- WHAT I BUILD -->
### WHAT I BUILD
<table>
  <tr>
    <td width="200" valign="top">
      <b>Web Development</b><br/>
      Modern, responsive web apps and PWAs with clean UX.
    </td>
    <td width="200" valign="top">
      <b>AI & Automation</b><br/>
      Tooling for AI workflows, integrations, and pipelines.
    </td>
    <td width="200" valign="top">
      <b>Developer Tools</b><br/>
      CLI utilities, plugins, and productivity tooling.
    </td>
  </tr>
  <tr>
    <td valign="top">
      <b>3D Web Experiences</b><br/>
      Isometric & wireframe visuals, interactive 3D UIs (SVG / Web-ready).
    </td>
    <td valign="top">
      <b>CLI Tools</b><br/>
      Terminal-first utilities and UX-focused CLIs.
    </td>
    <td valign="top">
      <b>Open Source</b><br/>
      Tools and libraries crafted for other devs to reuse.
    </td>
  </tr>
</table>

---

<!-- FEATURED PROJECTS (cards) -->
### FEATURED PROJECTS

<table width="100%" style="border-collapse:collapse;">
  <tr>
    <td width="50%" valign="top" style="padding:8px;">
      <div style="background:#0A0A0A;border-radius:10px;padding:12px;border:1px solid rgba(139,92,246,0.06);">
        <h4 style="margin:0;color:#8B5CF6">Apollo AI</h4>
        <p style="margin:6px 0 0;color:#CFEFFF">AI-powered platform for AI tools and document analysis.</p>
      </div>
    </td>
    <td width="50%" valign="top" style="padding:8px;">
      <div style="background:#0A0A0A;border-radius:10px;padding:12px;border:1px solid rgba(99,102,241,0.06);">
        <h4 style="margin:0;color:#00D4FF">NexForge</h4>
        <p style="margin:6px 0 0;color:#CFEFFF">Developer ecosystem for software development and experiments.</p>
      </div>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top" style="padding:8px;">
      <div style="background:#0A0A0A;border-radius:10px;padding:12px;border:1px solid rgba(139,92,246,0.04);">
        <h4 style="margin:0;color:#8B5CF6">CipherLab</h4>
        <p style="margin:6px 0 0;color:#CFEFFF">Platform for modern cybersecurity learning.</p>
      </div>
    </td>
    <td width="50%" valign="top" style="padding:8px;">
      <div style="background:#0A0A0A;border-radius:10px;padding:12px;border:1px solid rgba(0,212,255,0.04);">
        <h4 style="margin:0;color:#00D4FF">SkyCast</h4>
        <p style="margin:6px 0 0;color:#CFEFFF">Modern weather PWA with smooth UI.</p>
      </div>
    </td>
  </tr>
  <tr>
    <td colspan="2" valign="top" style="padding:8px;">
      <div style="background:#0A0A0A;border-radius:10px;padding:12px;border:1px solid rgba(99,102,241,0.04);">
        <h4 style="margin:0;color:#8B5CF6">IKY Toolkit</h4>
        <p style="margin:6px 0 0;color:#CFEFFF">Developer toolkit and Acode plugin to accelerate workflows.</p>
      </div>
    </td>
  </tr>
</table>

---

<!-- GITHUB STATS -->
### GitHub Stats
<p>
  <img src="https://github-readme-stats.vercel.app/api?username=iky-art&show_icons=true&theme=default&hide_border=true&bg_color=0A0A0A&title_color=8B5CF6&icon_color=00D4FF" alt="GitHub Stats" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=iky-art&layout=compact&hide_border=true&bg_color=0A0A0A&title_color=8B5CF6&text_color=CFEFFF" alt="Top Languages" />
</p>
<p>
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=iky-art&theme=dark-green" alt="GitHub Streak" />
  <img src="https://activity-graph.herokuapp.com/graph?username=iky-art&theme=react-dark&hide_border=true" alt="Activity Graph" />
</p>

---

<!-- CURRENTLY EXPLORING -->
### CURRENTLY EXPLORING
<p style="color:#CFEFFF">AI Engineering · Full-Stack Architecture · Developer Tooling · 3D Web · Cybersecurity · Cloud Deployment</p>

---

<!-- SYSTEM STATUS PANEL -->
### SYSTEM STATUS
<div style="background:#050505;padding:12px;border-radius:8px;border:1px solid rgba(99,102,241,0.05);">
<table width="100%">
  <tr>
    <td style="color:#8B5CF6"><b>Frontend</b></td>
    <td style="color:#CFF4FF">ONLINE</td>
    <td style="color:#8B5CF6"><b>Backend</b></td>
    <td style="color:#CFF4FF">ONLINE</td>
  </tr>
  <tr>
    <td style="color:#8B5CF6"><b>AI Systems</b></td>
    <td style="color:#CFF4FF">ONLINE</td>
    <td style="color:#8B5CF6"><b>Cloud</b></td>
    <td style="color:#CFF4FF">ONLINE</td>
  </tr>
  <tr>
    <td style="color:#8B5CF6"><b>Creativity</b></td>
    <td colspan="3" style="color:#CFF4FF">ACTIVE</td>
  </tr>
</table>
</div>

---

<!-- DEVELOPER PHILOSOPHY -->
### DEVELOPER PHILOSOPHY
<pre style="background:#050505;padding:10px;border-radius:8px;color:#D9ECFF;border:1px solid rgba(0,212,255,0.04);font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, monospace;">
BUILD · BREAK · LEARN · IMPROVE · SHIP
"Ship small, learn fast, keep the system beautiful."
</pre>

---

<!-- CONTRIBUTION GRAPH -->
### Contribution Activity
<p>
  <img src="https://activity-graph.herokuapp.com/graph?username=iky-art&theme=react-dark&area=true&hide_border=true" alt="Contribution Graph" />
</p>

---

<!-- CONNECT -->
### CONNECT WITH ME
- GitHub: https://github.com/iky-art

---

<!-- FOOTER -->
<p align="center" style="color:#8B98FF;margin-top:12px;font-weight:600;">
  BUILDING DIGITAL EXPERIENCES — ONE PROJECT AT A TIME.
</p>

<!-- small note: all visuals are SVG/HTML-only, no JS, no external CSS. -->

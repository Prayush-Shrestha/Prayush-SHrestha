
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 280" width="1200" height="280">
  <defs>
    <linearGradient id="background" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#101B18">
        <animate attributeName="stop-color"
          values="#101B18;#183B32;#101B18"
          dur="12s" repeatCount="indefinite"/>
      </stop>
      <stop offset="55%" stop-color="#183B32">
        <animate attributeName="stop-color"
          values="#183B32;#244D40;#183B32"
          dur="12s" repeatCount="indefinite"/>
      </stop>
      <stop offset="100%" stop-color="#244D40"/>
    </linearGradient>

    <linearGradient id="light" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#8FCBB0" stop-opacity="0"/>
      <stop offset="50%" stop-color="#A8DCC2"/>
      <stop offset="100%" stop-color="#8FCBB0" stop-opacity="0"/>
    </linearGradient>

    <radialGradient id="glow">
      <stop offset="0%" stop-color="#A8DCC2" stop-opacity=".22"/>
      <stop offset="100%" stop-color="#A8DCC2" stop-opacity="0"/>
    </radialGradient>

    <filter id="softGlow">
      <feGaussianBlur stdDeviation="5"/>
    </filter>
  </defs>

  <!-- Background -->
  <rect width="1200" height="280" rx="18" fill="url(#background)"/>

  <!-- Ambient glow -->
  <circle cx="1020" cy="65" r="150" fill="url(#glow)">
    <animate attributeName="r"
      values="130;170;130" dur="8s" repeatCount="indefinite"/>
    <animate attributeName="opacity"
      values=".5;1;.5" dur="8s" repeatCount="indefinite"/>
  </circle>

  <circle cx="130" cy="220" r="130" fill="url(#glow)">
    <animate attributeName="r"
      values="110;145;110" dur="10s" repeatCount="indefinite"/>
  </circle>

  <!-- Floating decorative circles -->
  <g fill="#A8DCC2">
    <circle cx="170" cy="65" r="2" opacity=".5">
      <animate attributeName="cy"
        values="65;48;65" dur="5s" repeatCount="indefinite"/>
      <animate attributeName="opacity"
        values=".2;.8;.2" dur="5s" repeatCount="indefinite"/>
    </circle>

    <circle cx="1020" cy="190" r="2.5" opacity=".5">
      <animate attributeName="cy"
        values="190;170;190" dur="6s" repeatCount="indefinite"/>
      <animate attributeName="opacity"
        values=".2;.8;.2" dur="6s" repeatCount="indefinite"/>
    </circle>

    <circle cx="900" cy="55" r="2" opacity=".4">
      <animate attributeName="cy"
        values="55;70;55" dur="7s" repeatCount="indefinite"/>
    </circle>

    <circle cx="280" cy="205" r="2" opacity=".4">
      <animate attributeName="cy"
        values="205;188;205" dur="6s" repeatCount="indefinite"/>
    </circle>

    <circle cx="750" cy="225" r="1.8" opacity=".5">
      <animate attributeName="cy"
        values="225;210;225" dur="5s" repeatCount="indefinite"/>
    </circle>
  </g>

  <!-- Moving background waves -->
  <path d="M0 220 Q300 160 600 220 T1200 205"
    fill="none"
    stroke="#A8DCC2"
    stroke-opacity=".18"
    stroke-width="2">
    <animate attributeName="d"
      values="M0 220 Q300 160 600 220 T1200 205;M0 205 Q300 245 600 195 T1200 220;M0 220 Q300 160 600 220 T1200 205"
      dur="12s" repeatCount="indefinite"/>
  </path>

  <path d="M0 240 Q300 180 600 240 T1200 225"
    fill="none"
    stroke="#A8DCC2"
    stroke-opacity=".10"
    stroke-width="2">
    <animate attributeName="d"
      values="M0 240 Q300 180 600 240 T1200 225;M0 225 Q300 265 600 215 T1200 240;M0 240 Q300 180 600 240 T1200 225"
      dur="14s" repeatCount="indefinite"/>
  </path>

  <!-- Main heading -->
  <g opacity="0">
    <animate attributeName="opacity"
      from="0" to="1" dur="1.5s" fill="freeze"/>
    <text x="600" y="110"
      text-anchor="middle"
      fill="#F4F4E9"
      font-family="Arial, sans-serif"
      font-size="52"
      font-weight="700"
      letter-spacing="4">
      PRAYUSH SHRESTHA
    </text>
  </g>

  <!-- Animated accent line -->
  <rect x="390" y="140" width="420" height="2" fill="url(#light)">
    <animate attributeName="opacity"
      values=".35;1;.35" dur="3s" repeatCount="indefinite"/>
  </rect>

  <rect x="390" y="140" width="0" height="2"
    fill="#F4F4E9" opacity=".7">
    <animate attributeName="width"
      values="0;420;0" dur="7s" repeatCount="indefinite"/>
  </rect>

  <!-- Role -->
  <g opacity="0">
    <animate attributeName="opacity"
      from="0" to="1" begin=".6s" dur="1.5s" fill="freeze"/>
    <text x="600" y="180"
      text-anchor="middle"
      fill="#A8DCC2"
      font-family="Arial, sans-serif"
      font-size="17"
      letter-spacing="5">
      SOFTWARE DEVELOPER
    </text>
  </g>

  <!-- Specialization -->
  <g opacity="0">
    <animate attributeName="opacity"
      from="0" to="1" begin="1.1s" dur="1.5s" fill="freeze"/>
    <text x="600" y="210"
      text-anchor="middle"
      fill="#F4F4E9"
      opacity=".75"
      font-family="Arial, sans-serif"
      font-size="13"
      letter-spacing="2.5">
      AI/ML · DATA ANALYTICS · DATA ENGINEERING · CLOUD
    </text>
  </g>

  <!-- Small location label -->
  <g opacity="0">
    <animate attributeName="opacity"
      from="0" to=".7" begin="1.5s" dur="1.5s" fill="freeze"/>
    <text x="600" y="246"
      text-anchor="middle"
      fill="#A8DCC2"
      font-family="Arial, sans-serif"
      font-size="11"
      letter-spacing="4">
      KATHMANDU, NEPAL
    </text>
  </g>

  <!-- Subtle moving light -->
  <ellipse cx="-100" cy="0" rx="80" ry="220"
    fill="#A8DCC2"
    opacity=".035"
    filter="url(#softGlow)">
    <animate attributeName="cx"
      values="-100;1300" dur="14s" repeatCount="indefinite"/>
  </ellipse>

</svg>

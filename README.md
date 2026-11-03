<svg xmlns="http://www.w3.org/2000/svg" width="800" height="90" viewBox="0 0 800 90">
  <defs>
    <linearGradient id="trackR" x1="0" x2="1">
      <stop offset="0" stop-color="#E50914" stop-opacity="0"/>
      <stop offset="1" stop-color="#E50914"/>
    </linearGradient>
    <linearGradient id="trackB" x1="0" x2="1">
      <stop offset="0" stop-color="#0A66FF" stop-opacity="0"/>
      <stop offset="1" stop-color="#0A66FF"/>
    </linearGradient>
    <filter id="glow"><feGaussianBlur stdDeviation="3" result="b"/>
      <feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
  </defs>

  <!-- tracks -->
  <line x1="0" y1="25" x2="800" y2="25" stroke="#E50914" stroke-opacity=".25" stroke-width="2" stroke-dasharray="10 8">
    <animate attributeName="stroke-dashoffset" from="0" to="-36" dur="0.6s" repeatCount="indefinite"/>
  </line>
  <line x1="0" y1="65" x2="800" y2="65" stroke="#0A66FF" stroke-opacity=".25" stroke-width="2" stroke-dasharray="10 8">
    <animate attributeName="stroke-dashoffset" from="0" to="-36" dur="0.8s" repeatCount="indefinite"/>
  </line>

  <!-- red runner + trail -->
  <rect x="0" y="22" height="6" rx="3" fill="url(#trackR)" filter="url(#glow)">
    <animate attributeName="width" values="0;150;0" dur="4s" repeatCount="indefinite"/>
    <animate attributeName="x" values="0;780;800" dur="4s" repeatCount="indefinite"/>
  </rect>
  <circle r="9" cy="25" fill="#E50914" filter="url(#glow)">
    <animate attributeName="cx" values="10;790" dur="4s" repeatCount="indefinite"/>
    <animate attributeName="r" values="9;11;9" dur="0.5s" repeatCount="indefinite"/>
  </circle>

  <!-- blue runner + trail -->
  <rect x="0" y="62" height="6" rx="3" fill="url(#trackB)" filter="url(#glow)">
    <animate attributeName="width" values="0;150;0" dur="5s" repeatCount="indefinite"/>
    <animate attributeName="x" values="0;780;800" dur="5s" repeatCount="indefinite"/>
  </rect>
  <circle r="9" cy="65" fill="#0A66FF" filter="url(#glow)">
    <animate attributeName="cx" values="10;790" dur="5s" repeatCount="indefinite"/>
    <animate attributeName="r" values="9;11;9" dur="0.6s" repeatCount="indefinite"/>
  </circle>
</svg>

<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 900 200" width="900" height="200">
  <defs>
    <filter id="r" x="-3%" y="-3%" width="106%" height="106%">
      <feTurbulence type="fractalNoise" baseFrequency="0.028" numOctaves="4" seed="12" result="n"/>
      <feDisplacementMap in="SourceGraphic" in2="n" scale="2" xChannelSelector="R" yChannelSelector="G"/>
    </filter>
    <style>
      .ln { fill: none; stroke-linecap: round; stroke-linejoin: round; }
      .w1 { stroke: #D8D2C8; }
      .w2 { stroke: #B0AAA0; }
      .w3 { stroke: #E8E4DC; }

      .bo { stroke-dasharray: 2220; stroke-dashoffset: 2220; animation: d 2s cubic-bezier(.5,0,.5,1) 0s forwards; }
      .bi { stroke-dasharray: 2100; stroke-dashoffset: 2100; animation: d 2s cubic-bezier(.5,0,.5,1) 0.18s forwards; }

      .bm { stroke-dasharray: 310; stroke-dashoffset: 310; animation: d 1.2s ease 0.2s forwards; }
      .bc { stroke-dasharray: 140; stroke-dashoffset: 140; animation: d 0.7s ease 0.85s forwards; }
      .bt { stroke-dasharray: 290; stroke-dashoffset: 290; animation: d 1.1s ease 0.3s forwards; }

      .lv { stroke-dasharray: 110; stroke-dashoffset: 110; }
      .la { animation: d .44s ease 0.75s forwards; }
      .lb { animation: d .44s ease 0.90s forwards; }
      .lc { animation: d .44s ease 1.05s forwards; }
      .ld { animation: d .44s ease 1.18s forwards; }
      .le { animation: d .44s ease 1.30s forwards; }
      .lf { animation: d .44s ease 1.42s forwards; }
      .lg { animation: d .44s ease 1.55s forwards; }
      .lh { animation: d .44s ease 0.80s forwards; }
      .li { animation: d .44s ease 0.95s forwards; }

      .bd { stroke-dasharray: 65; stroke-dashoffset: 65; }
      .b1 { animation: d .55s ease 1.35s forwards; }
      .b2 { animation: d .55s ease 1.55s forwards; }
      .b3 { animation: d .55s ease 1.75s forwards; }
      .b4 { animation: d .55s ease 1.95s forwards; }
      .b5 { animation: d .55s ease 2.05s forwards; }
      .b6 { animation: d .55s ease 2.18s forwards; }
      .b7 { animation: d .55s ease 2.30s forwards; }
      .b8 { animation: d .55s ease 1.45s forwards; }

      .sp { stroke-dasharray: 330; stroke-dashoffset: 330; animation: d .7s ease 2.4s forwards; }

      .t1 { opacity: 0; animation: fi .9s ease 2.5s forwards; }
      .t2 { opacity: 0; animation: fi .8s ease 3.0s forwards; }
      .t3 { opacity: 0; animation: fi .7s ease 3.4s forwards; }

      @keyframes d { to { stroke-dashoffset: 0; } }
      @keyframes fi { to { opacity: 1; } }
    </style>
  </defs>

  <rect width="900" height="200" fill="#0D1117"/>

  <!-- Outer frame -->
  <rect x="11" y="11" width="878" height="178" rx="3"
        class="ln w2 bo" stroke-width="1.4" filter="url(#r)"/>
  <!-- Inner frame -->
  <rect x="19" y="19" width="862" height="162" rx="2"
        class="ln w2 bi" stroke-width="0.75" opacity="0.45" filter="url(#r)"/>

  <!-- Main branch: bottom-left rising upward -->
  <path d="M 35 194 C 40 178 46 161 53 145 C 59 129 66 113 73 97
           C 80 81 86 65 92 49 C 96 37 97 27 97 24"
        class="ln w1 bm" stroke-width="1.3" filter="url(#r)"/>

  <!-- Secondary twig off main branch -->
  <path d="M 58 140 C 54 127 52 113 56 100"
        class="ln w2 bc" stroke-width="0.95" filter="url(#r)"/>

  <!-- Leaves off main branch -->
  <path d="M 55 142 C 46 135 38 130 32 125" class="ln w1 lv la" stroke-width="1"   filter="url(#r)"/>
  <path d="M 55 138 C 63 132 71 129 78 125" class="ln w1 lv la" stroke-width="1"   filter="url(#r)"/>
  <path d="M 64 117 C 55 111 47 107 41 102" class="ln w1 lv lb" stroke-width="1"   filter="url(#r)"/>
  <path d="M 68 106 C 77 100 85 97 92 93"   class="ln w1 lv lc" stroke-width="1"   filter="url(#r)"/>
  <path d="M 77 82  C 67 76 60 72 55 68"    class="ln w1 lv ld" stroke-width="0.95" filter="url(#r)"/>
  <path d="M 83 68  C 91 62 98 60 104 56"   class="ln w1 lv le" stroke-width="0.95" filter="url(#r)"/>
  <path d="M 90 48  C 82 42 78 35 76 29"    class="ln w1 lv lf" stroke-width="0.9"  filter="url(#r)"/>
  <path d="M 57 132 C 48 125 42 120 36 116" class="ln w2 lv lg" stroke-width="0.85" filter="url(#r)"/>

  <!-- Top-right corner branch -->
  <path d="M 862 22 C 854 35 848 50 842 64 C 836 77 832 90 828 102"
        class="ln w1 bt" stroke-width="1.1" filter="url(#r)"/>
  <path d="M 844 62 C 852 56 860 53 866 49" class="ln w1 lv lh" stroke-width="0.9" filter="url(#r)"/>
  <path d="M 832 89 C 840 83 848 81 855 77" class="ln w1 lv li" stroke-width="0.9" filter="url(#r)"/>
  <path d="M 826 102 C 818 108 812 114 810 120" class="ln w2 lv li" stroke-width="0.85" filter="url(#r)"/>

  <!-- Bird flock: flying upper-right, fading into distance -->
  <!-- Lead bird (largest, lowest) -->
  <path d="M 644 98 Q 662 85 662 98 Q 662 85 680 98"
        class="ln w3 bd b8" stroke-width="1.9"/>
  <!-- 2nd -->
  <path d="M 676 72 Q 692 60 692 72 Q 692 60 708 72"
        class="ln w3 bd b1" stroke-width="1.75"/>
  <!-- 3rd -->
  <path d="M 703 53 Q 717 42 717 53 Q 717 42 731 53"
        class="ln w3 bd b2" stroke-width="1.55"/>
  <!-- 4th -->
  <path d="M 729 38 Q 741 28 741 38 Q 741 28 753 38"
        class="ln w3 bd b3" stroke-width="1.35"/>
  <!-- Side bird -->
  <path d="M 718 76 Q 729 66 729 76 Q 729 66 740 76"
        class="ln w3 bd b4" stroke-width="1.45"/>
  <!-- Small bird -->
  <path d="M 746 59 Q 756 50 756 59 Q 756 50 766 59"
        class="ln w3 bd b5" stroke-width="1.2"/>
  <!-- Tiny bird -->
  <path d="M 760 42 Q 768 35 768 42 Q 768 35 776 42"
        class="ln w3 bd b6" stroke-width="1.1"/>
  <!-- Highest/furthest tiny bird -->
  <path d="M 746 26 Q 753 20 753 26 Q 753 20 760 26"
        class="ln w3 bd b7" stroke-width="1"/>

  <!-- Separator line (hand-drawn) -->
  <path d="M 236 116 C 274 114 328 118 390 116 C 452 114 506 118 544 116"
        class="ln w2 sp" stroke-width="0.8" filter="url(#r)" opacity="0.65"/>

  <!-- Main title: ブレント -->
  <text x="390" y="100" text-anchor="middle"
        font-family="'Noto Serif JP','Hiragino Mincho Pro','Yu Mincho','Times New Roman',serif"
        font-size="44" font-weight="300"
        fill="#E8E4DC" class="t1">ブレント</text>

  <!-- Subtitle -->
  <text x="390" y="144" text-anchor="middle"
        font-family="'Courier New',Courier,monospace"
        font-size="11.5" letter-spacing="5.5"
        fill="#7A9A7A" class="t2">Brent001 · 開発者</text>

  <!-- Tag line -->
  <text x="390" y="162" text-anchor="middle"
        font-family="Arial,Helvetica,sans-serif"
        font-size="9.5" letter-spacing="3"
        fill="#3E5A3E" class="t3">cs student · builder · 作る者</text>
</svg>

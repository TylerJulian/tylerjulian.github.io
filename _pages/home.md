---
layout: splash
permalink: /
hidden: true
excerpt: home page
author_profile: true

carousels:
- images:
- image: /assets/img/beeclick_toast.jpg
- image: /assets/img/person_1_sq.jpg

header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: {% include carousel.html height="50" unit="%" duration="7" number="1" %}



feature_row:
  - image_path: /assets/img/scr.png
    alt: "SCR"
    title: "Sooner Competitive Robotics"
    excerpt: "I am a mentor for Sooner Competitive Robotics at the University of Oklahoma."
    url: "/SCR/"
    btn_class: "btn--primary"
    btn_label: "Learn more"  
  
  - image_path: /assets/img/toast.jpg
    alt: "toaster"
    title: "Wifi Toaster"
    excerpt: "The wifi toaster was born from laziness. It was from a student's desire to not get up to toast bread."
    url: "/Toaster/"
    btn_class: "btn--primary"
    btn_label: "Learn more"  

---

{% include feature_row %}
---
title:  "Slideshow"
permalink: "/slideshow/"
layout: post
---

Some pictures from my work/observations  

<div style="text-align: center;">
  <img id="slideshow" src="/images/Nancay_HI_spectra.jpg" alt="Slideshow" style="width: 80%; max-width: 600px; border-radius: 10px; box-shadow: 0 0 10px #0004;">
  <p id="caption" style="font-style: italic; margin-top: 10px;">Optical images and corresponding HI 21 cm line profiles of galaxies I observed in 2022 with the Nançay Radio Telescope. The optical images are 5 minutes squared fields from the Digitized Sky Survey (DSS2, B band). Each HI spectrum shows the flux density (in mJy) as a function of radial velocity (in km/s).</p>
</div>

<script>
  const images = [
    "/images/Nancay_HI_spectra.jpg",
    "/images/Andromeda.jpg"
  ];
  const descriptions = [
    "Optical images and corresponding HI 21 cm line profiles of galaxies I observed in 2022 with the Nançay Radio Telescope. The optical images are 5 minutes squared fields from the Digitized Sky Survey (DSS2, B band). Each HI spectrum shows the flux density (in mJy) as a function of radial velocity (in km/s).",
    "My bolometric observation of M31 taken with E.A. device and upscaled with AI."
  ];

  let index = 0;
  const imgElement = document.getElementById("slideshow");
  const captionElement = document.getElementById("caption");

  setInterval(() => {
    index = (index + 1) % images.length;
    imgElement.src = images[index];
  }, 10000); // 10s
</script>

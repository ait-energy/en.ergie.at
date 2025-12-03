---
title: "Flexibilität"
topics: []
authors: ["sstroemer"]
---

<style>
.floating-iframe-wrapper {
  position: fixed; /* Position the wrapper fixed relative to the viewport */
  top: 0;          /* Stick it to the top of the page */
  left: 0;         /* Align it to the left */
  width: 100vw;    /* Make it span the full width of the viewport */
  height: 100vh;   /* Make it span the full height of the viewport */
  z-index: 99;     /* Ensure it floats above other content, but below the header at z-index 100 */
  overflow: hidden; /* Hide anything that exceeds the iframe's boundaries */
}

.floating-iframe {
  width: 100%;      /* Make iframe take the full width */
  height: 100%;     /* Make iframe take the full height */
  border: none;     /* Remove iframe border */
}
</style>

<div class="floating-iframe-wrapper">
  <iframe src="https://ies-tools.ait.ac.at/flex/?lang=de" frameborder="0" class="floating-iframe"></iframe>
</div>

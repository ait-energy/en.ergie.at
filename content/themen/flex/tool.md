---
title: "Flex Tool"
topics: []
authors: ["sstroemer"]
---

<style>
.loading-container {
    display: flex;
    align-items: center;
}
.spinner {
    border: 4px solid #f3f3f3; /* Light grey */
    border-top: 4px solid #3498db; /* Blue */
    border-radius: 50%;
    width: 2em;
    height: 2em;
    margin-left: 2em;
    animation: spin 1s linear infinite;
}
@keyframes spin {
    0% { transform: rotate(0deg); }
    100% { transform: rotate(360deg); }
}
</style>

<div class="loading-container">
    <span>Das AIT Flex Tool lädt ...</span>
    <div class="spinner"></div>
</div>

<style>
.floating-iframe-wrapper {
  position: fixed; /* Position the wrapper fixed relative to the viewport */
  top: 53px;          /* Stick it to the top of the page */
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
  border-top: 1px solid rgb(41, 37, 36); /* Add a top border to separate from header */
}
</style>

<div class="floating-iframe-wrapper">
  <iframe src="https://ies-tools.ait.ac.at/flex/?lang=de" frameborder="0" class="floating-iframe"></iframe>
</div>

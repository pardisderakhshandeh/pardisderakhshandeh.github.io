---
layout: cv
permalink: /cv/
title: CV
nav: true
nav_order: 7
cv_pdf: /assets/pdf/example_pdf.pdf # you can also use external links here
cv_format: rendercv # options: rendercv, jsonresume
description: This is a description of the page. You can modify it in '_pages/cv.md'. You can also change or remove the top pdf download button.
toc:
  sidebar: left
---
---
layout: page
title: CV
permalink: /cv/
nav: true
nav_order: 6
---

<div class="row">
  <div class="col-sm-12">
    <object data="{{ '/assets/pdf/cv.pdf' | relative_url }}" type="application/pdf" width="100%" height="1000px">
        <p>Your browser does not support viewing PDFs. Please download the PDF to view it: <a href="{{ '/assets/pdf/cv.pdf' | relative_url }}">Download PDF</a>.</p>
    </object>
  </div>
</div>

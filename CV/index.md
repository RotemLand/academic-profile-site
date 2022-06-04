---
layout: layouts/base.njk
title: Resume
templateClass: tmpl-post
eleventyNavigation:
  key: CV
  order: 4
---

<div id="adobe-dc-view"></div>
<script src="https://documentcloud.adobe.com/view-sdk/main.js"></script>
<script type="text/javascript">
  document.addEventListener("adobe_dc_view_sdk.ready", function(){
    var adobeDCView = new AdobeDC.View({clientId: process.env.ADOBE_API_KEY, divId: "adobe-dc-view"});
    adobeDCView.previewFile({
      content:{location: {url: "https://rotemland.github.io/img/resume.pdf"}},
      metaData:{fileName: "resume.pdf"}
    }, {});
  });
</script>

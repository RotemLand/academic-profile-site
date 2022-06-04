---
layout: layouts/base.njk
title: Resume
templateClass: tmpl-post
eleventyNavigation:
  key: CV
  order: 4
---

<html>
<head>
 <title>Adobe Document Services PDF Embed API Sample</title>
 <meta charset="utf-8"/>
 <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1"/>
 <meta id="viewport" name="viewport" content="width=device-width, initial-scale=1"/>
</head>
<body style="margin: 0px">
 <div id="adobe-dc-view"></div>
 <script src="https://documentcloud.adobe.com/view-sdk/main.js"></script>
 <script type="text/javascript">
    document.addEventListener("adobe_dc_view_sdk.ready", function()
    {
        var adobeDCView = new AdobeDC.View({clientId: "%ADOBE_API_KEY%", divId: "adobe-dc-view"});
        adobeDCView.previewFile(
       {
          content:   {location: {url: "https://rotemland.github.io/img/resume.pdf"}},
          metaData: {fileName: "Rotem Landesman CV.pdf"}
       });
    });
 </script>
</body>
</html>
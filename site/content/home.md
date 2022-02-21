---
title: "home"
date: 2018-11-14T19:02:50-07:00
draft: false
---

<!doctype html>
<html lang="{{ $.Site.Language.Lang }}">


  {{ block "header" . }}{{end}}
  <body>
    

  {{ block "main" . }}{{end}}
</body>

  {{ block "footer" . }}{{ partial "footer" . }}{{end}}

  {{ $script := .Site.Data.webpack.main }}
  {{ with $script.js }}
    <script src="{{ relURL . }}"></script>
  {{ end }}



</html>
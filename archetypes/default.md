---
date: {{ .Date }}
type: "posts"
draft: true
title: {{ replace .File.ContentBaseName "-" " " | title }}
hideReadingTime: true
hideWordCount: true
---

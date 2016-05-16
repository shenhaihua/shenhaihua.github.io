---
layout: post
title:  "rails form有错误信息时生成class为field_with_errors的div，如何解决？"
date:   2016-05-16 23:16:20 +0800
---

在application.rb文件里面加入以下配置即可

	config.action_view.field_error_proc = proc {|html, instance| html }
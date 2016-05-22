---
layout: post
title:  "rails form有错误信息时生成class为field_with_errors的div，如何解决？"
date:   2016-05-16
excerpt: "今天写rails form的时候碰到一个问题，当有错误信息的时候form下会生成class为field_with_errors的div，导致样式错乱。"
tags: [ruby,rails,form,error]
comments: true
---
今天写rails form的时候碰到一个问题，当有错误信息的时候form下会生成```<div class="field_with_errors"></div>```，导致样式错乱。

在application.rb文件里面加入以下配置即可

	config.action_view.field_error_proc = proc {|html, instance| html }
+++
categories = ["blog"]
date = "2017-05-15T23:54:06+02:00"
description = "Markup Reference"
draft = false
images = ["https://upload.wikimedia.org/wikipedia/commons/2/21/Hello_World_Brian_Kernighan_1978.jpg"]
slug = "markup"
tags = ["blog", "markdown"]
title = "Markup Reference"
toc = false

+++

This post is a reference for myself. I can lookup all the markup for future postings. One of my next post will include the technology behind this blog.

<!--more-->

## Markup

Code (of course Go):

<pre>
<code class="language-go">
// Hello There
package main

import (
  "fmt"
  "log"
  "net/http"
)

func main() {
  http.HandleFunc("/", func(w http.ResponseWriter, req *http.Request) {
    fmt.Fprintln(w, "I are digital!")
  })
  log.Fatal(http.ListenAndServe(":8080", nil))
}
</code>
</pre>


Boxes:

{{< hackcss-alert type="info">}}
Box Info
{{< /hackcss-alert>}}

{{< hackcss-alert type="error">}}
Box Error
{{< /hackcss-alert>}}

{{< hackcss-alert type="warning">}}
Box Warning
{{< /hackcss-alert>}}

{{< hackcss-alert type="success">}}
Box Success
{{< /hackcss-alert>}}

 Blockquote:

<blockquote >
 “One of they key problems today is that politics is such a disgrace. Good people don’t go into government.”</br></br>
 Donald Trump
</blockquote>

<img data-src="https://upload.wikimedia.org/wikipedia/commons/f/fe/Donald_Trump_Signature.svg" class="lazyload">

Some buttons:

{{< hackcss-buttongroup >}}
  {{< hackcss-button text="Left" />}}
  {{< hackcss-button text="Middle" type="info" />}}
  {{< hackcss-button text="Right" isghost="true" />}}
{{< /hackcss-buttongroup >}}

A Tweet:

{{< tweet 761672994376806400>}}

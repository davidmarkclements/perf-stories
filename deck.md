<!--
master: title-page
notes: |
  Hi my name's Dave

  I'm from nearForm

  I'd like to tell you a story
-->

# perf<br> stories
### [@davidmarkclem](http://twitter.com/davidmarkclem)

<h2 style="font-weight: bold; opacity: 0.4; position:absolute; bottom: 10px; font-size: 32px"> 
  <a href=http://davidmarkclements.github.io/perf-stories> davidmarkclements.github.io/perf-stories </a>
</h2>


---
<!--
master: section-title
notes: |
  a talk about performance,
  told in a series of stories
  framed in the vernacular of metaliterature, for self amusement

  to employ a magguffin, techniques that won't feature
  include the predestination paradox (requires a time machine)
  the quibble (because I'm not a lawyer)
  the unreliable narrator (because I never lie)
  on that note..
  I'm also absolutely avoiding allegory, amplification, anagrams, 
  asyndetons, alliteration and assonance

-->

# Stories<br>in<br>Stories
### [@davidmarkclem](http://twitter.com/davidmarkclem)


---
<!--
master: section-title
notes: |
  Matteo Collina and I have a mission

  To help people with performance problems

  And simplify the optimization process, 

  Wherever we go
-->

# Flashback:<br> January 2016
## The Frame Story
### [@davidmarkclem](http://twitter.com/davidmarkclem)


---
<!--
master: section-title
notes: |
  Little bit of prose to set the scene

  It was a golden crisp morning in Italy,
  the smell of rich coffee
  lingered pleasantly in the air
  as I made my way along the marbled porticos
  of Bologna's ancient palaces
  toward Matteo's apartment

-->

# Sensory Detail
## (exposition)
### [@davidmarkclem](http://twitter.com/davidmarkclem)

<div id=sens-det-bg></div>

<details><summary></summary><style>
#-exposition- {
  font-weight: bold;
  font-variant: small-caps;
  letter-spacing: .2em;
  font-style: italic;

}
#sensory-detail {
  margin-top: -20px;
  font-size: 70px;
  text-shadow: 2px 1px 2px #bbb;
}
#sensory-detail::before {
  display: block;
  content: '';
  border: 2px solid #111;
  border-left: none;
  border-right: none;
  display: -webkit-box;
  display: -webkit-flex;
  display: -ms-flexbox;
  display: flex;
  content: '';
  height: 0;
  margin-bottom: -65px;
  margin-left: 4px;
  width: 264px;
  box-shadow: 2px 1px 2px #bbb;
}
#sensory-detail::after {
  display: block;
  content: '';
  border: 2px solid #111;
  border-left: none;
  border-right: none;
  display: -webkit-box;
  display: -webkit-flex;
  display: -ms-flexbox;
  display: flex;
  content: '';
  height: 0;
  margin-top: -16px;
  margin-left: 340px;
  width: 250px;
  box-shadow: 2px 1px 2px #bbb;
}
#sens-det-bg {
  background: url(images/bologna.jpg);
  background-size: cover;
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  height: 100%;
  z-index: -1;
  opacity: 0.5;
}
</style>
</details>

---
<!--
master: section-title
notes: |
  as we settled down to the business of
  preparation 
  
  Matteo told me a story about
  his recent work with NewsCorp for The Times and
  The Sunday Times

  
-->

# Narrative Hook
## via hypodiegesis
### telling a story within a story

<details><summary></summary><style>
  #telling-a-story-within-a-story {
    font-size: 16px;
    width: 76px;
    right: 5px;
  }
</style>
</details>

---
<!--
master: section-title
notes: |
  I got the code to a point where we couldn't
  optimize it anymore, because our I/O was
  going faster than the capacity of the network card

  The network card became the bottlneck

  Emulated network, 720Mb/s - AWS
-->
<div id=quote-bg></div>

<blockquote id=quote>
The network card...<br> became the bottleneck!
</blockquote>

<img id=times-logo src=images/logo-the-times.png onload="javascript:document.querySelectorAll('a').forEach((a) => a.setAttribute('target', '_blank'));document.querySelectorAll('details').forEach((d) => d.outerHTML = d.innerHTML);">

### [@davidmarkclem](http://twitter.com/davidmarkclem)

<div id=news-uk-cs> 
<a target=_blank href=http://www.nearform.com/nodecrunch/client-case-study-news-uk/> &nbsp;http://www.nearform.com/ <br> &nbsp;&nbsp;nodecrunch/client-case-&nbsp;<br>&nbsp; &nbsp; &nbsp; &nbsp;study-news-uk &nbsp; &nbsp; &nbsp;</a>
</div>
<details><summary></summary><style>
#news-uk-cs a {
  font-family: 'Cutive Mono', monospace;
  background: white;
  position: relative;
}

#news-uk-cs {
  position: absolute;
  bottom: 10px;
  right: 10px;
}

#times-logo {
  width: 180px;
  position: absolute;
  left: 10px;
  top: 10px;

}

#quote {
  font-size: 36px;
  font-weight: bold;
  font-style: normal;
  width: 80%;
  text-shadow: 2px 1px 2px #bbb;
  margin-top: -30px;
}
#quote-bg {
  background: url(images/matteo.jpg) -540px -54px;
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  height: 100%;
  z-index: -1;
  opacity: 0.5;
}
</style>
</details>

---
<!--
master: section-title
notes: |  
  As I pondered this incredible story, and looked
  through the code that was responsible for this 
  extremely efficient throughput an angel appeared
  on one shoulder and a demon (fallen angel) appeared 
  on the other

  Angel: This is amazing, but to the untrained eye
  this code looks exactly like a novice wrote it

  Devil: Who cares, it's fast isn't it? It's what 
  they wanted, what they neeeded, high performance 


-->

# Angels<br>on my<br>Shoulders
### [@davidmarkclem](http://twitter.com/davidmarkclem)

---
<!--
master: section-title
notes: |  
  they were both right, instead of a moral dilema,
  what was needed was a moral solution

  once you learn to optimize, pay it forward and 
  protect your work, by commenting in relevant cases

  however (foreshadowing) - don't put comments *inside*
  hot functions, put them just above  
-->

# Moral:
## Comment Optimized Code
### [@davidmarkclem](http://twitter.com/davidmarkclem)

---
<!--
master: section-title
notes: |
  as much as I was enjoying contemplation, 
  a sense of urgency had crept in
  
  we had a lot to prepare, and precious little time

  the purpose of our gathering, was to codify our
  performance knowledge into training material and
  consultancy planning for a client engagement the
  following week
-->

# Ticking Clock Scenario
### [@davidmarkclem](http://twitter.com/davidmarkclem)

---
<!--
master: section-title
notes: |
  Net-A-Porter and Mr Porter had several internal 
  projects that they wanted help with, 
  
  but they wanted the kind of help that empowers them
  to make changes, rather than relying on us

  2 days showing techniques and tools
  2 days applying techniques in groups to code bases

  1/3 servers, 2x throughput 1/2 latency 


-->

<img id=net-a-porter style="width:80%;margin-top: -100px" src=images/nap.svg>
### [@davidmarkclem](http://twitter.com/davidmarkclem)

<div id=nap-bg>
<div id=nap-cs> 
<a target=_blank href=http://www.nearform.com/nodecrunch/client-case-study-net-a-porter/> &nbsp;http://www.nearform.com/ <br> &nbsp;&nbsp;nodecrunch/client-case-&nbsp;<br>&nbsp; &nbsp;study-net-a-porter &nbsp; &nbsp;&nbsp;</a>
</div>
<details><summary></summary><style>
#nap-cs a {
  font-family: 'Cutive Mono', monospace;
  background: white;
  position: relative;
}

#nap-cs {
  position: absolute;
  bottom: 10px;
  right: 10px;
}

#nap-bg {
  background: url(images/nap-bg.jpg);
  background-size: cover;
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  height: 100%;
  z-index: -1;
  opacity: 0.5;
}
</style>
</details>


---
<!--
master: section-title
notes: |
  Matteo and I came away from Net-A-Porter inspired
  we now had a very good idea of things our community really
  needed when it comes to profiling and performance
-->

# Time for a Metaphor
## (and hyperbole)
### [@davidmarkclem](http://twitter.com/davidmarkclem)


---
<!--
master: section-title
notes: |
  + autopsy
  + fast-safe-strinfgy
  + quick-format
  + fastify
  also steed but that was precursor
-->

# Our Cambrian Explosion

<a id=campino class=camlnk href=https://github.com/pinojs target="_blank">
  <img class=camlogo src=images/pino.png>
</a>
<a id=cam0x class=camlnk href=https://github.com/davidmarkclements/0x target="_blank">
  <img class=camlogo src=images/0x.png>
</a>
<a id=camac class=camlnk href=https://github.com/mcollina/autocannon target="_blank">
  <img class=camlogo src=images/autocannon.png>
</a>

<div id=cam-bg>
<details><summary></summary><style>
.camlnk {
  padding-left: 4px;
  padding-right: 4px;
}
.camlogo {
  width: 130px
}
#campino:hover {
  box-shadow: 0px -50px 50px rgb(161, 191, 100);

}
#cam0x:hover {
  box-shadow: 0px -50px 50px rgb(218, 154, 81);
}

#camac:hover {
  box-shadow: 0px -50px 50px rgb(103, 161, 177);
}

#our-cambrian-explosion {
  font-size: 45px;
  position: absolute;
  top: 70px;
  width: 100%;
}

#cam-bg {
  background: url(images/explosion.png) no-repeat center bottom rgb(40,51,72);
  background-size: auto 80%;
  padding-left: 100px;
  padding-right: 100px;
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  height: 100%;
  z-index: -1;
  opacity: 0.5;
}
</style>
</details>

---
<!--
master: section-title
notes: |
  god from the machine -> 
    when the impossible suddenly becomes possible
    due to some new event
-->

# Deus Ex Machina
## The 0x Story
### [@davidmarkclem](http://twitter.com/davidmarkclem)

<details><summary></summary><style id=dem-bg>
#dem-bg {
  text-indent: 100%;
  white-space: nowrap;
  overflow: hidden;
  display: block;
  background: url(images/dem.jpg);
  background-size: cover;
  padding-left: 100px;
  padding-right: 100px;
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  height: 100%;
  z-index: -1;
  opacity: .25;
  filter: blur(10px) sepia(70%) contrast(150%);
}
</style>
</details>

---
<!--
master: section-title
notes: |
  I had been generating flamegraphs for over a year,
  at one point it worked on OS X but an Apple upgrade
  with reduced dtrace functionality made it impossible again

  Since the Net-A-Porter teams were mostly on macbooks we wanted
  to make flamegraph generation possible on OS X 
-->

# Flamegraph

<div id=bg-fg></div>
<h3 id=fg-h3> 
  <a href=http://twitter.com/davidmarkclem>@davidmarkclem</a>
</h3>

<details>
<summary></summary>
<style>
#flamegraph {
  color: rgb(209,115,57);
  position: absolute;
  top: 128px;
  text-shadow: 0px 3px 10px rgb(189, 55, 30);
}

#fg-h3 a {
  color:  #eee;
}
#bg-fg {
  background: url(images/flamegraph.png);
  background-size: cover;
  opacity: 1;
  z-index: -1;
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  width: 100%;
}
</style>
</details>

---
<!--
master: section-title
notes: |
 At the time the highest version was v.12 
 which introduced --perf-basic-prof flag
 this generates a hex address to function name map
 in the /tmp folder. 

 The discovery of this mapping file was our eureka moment

 we were able to use dtrace take samples of the cpu
 where each callframe was a hex address then map those
 hex addresses to the mapping file created by --perf-basic-prof
-->

# [perf-sym](http://npm.im/perf-sym)

### [@davidmarkclem](http://twitter.com/davidmarkclem)

---
<!--
master: section-title
notes: |
  it still took around 5-7 steps to succesfully
  generate a flamegraph, and only on a Linux machine

  realising the need for simplification we wrote 0x 
  after the engagement, and the NaP teams used it moving
  forward to implement suggested changes

  0x works on Linux and OS X/macOS and thanks to tips from 
  Aaron Robinson & Brian Terlson we're very close to getting
  0x working on Windows 
  "0x" because I was staring at hex addresses so much

-->

<a href=http://npm.im/0x target="_blank">
  <img id=logo0x src=images/0x-logo.png>
</a>

### [@davidmarkclem](http://twitter.com/davidmarkclem)

<details><summary></summary><style>
  #logo0x {
    width: 50%;
    margin-top: -40px;
  }
</style>
</details>


---
<!--
master: section-title
notes: |
  an autocannon is a a machinegun in cannon form
  it's an HTTP benchmarking tool
  used by core
  uses `net` instead of `http`
  native-hdr-historgram < 5 nanoseconds per entry 
-->

# Fighting<br>Red Herrings
## Autocannon Origins
### [@davidmarkclem](http://twitter.com/davidmarkclem)

<details><summary></summary><style id=rh-bg>
#rh-bg {
  text-indent: 100%;
  white-space: nowrap;
  overflow: hidden;
  display: block;
  background: url(images/red-herring.jpg) 0 -50px;
  background-size: cover;
  padding-left: 100px;
  padding-right: 100px;
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  height: 100%;
  z-index: -1;
  opacity: .25;
  filter: blur(10px) saturate(4500%);
}
</style>
</details>

---
<!--
master: section-title
notes: |
  automated benchmarking
  ci pipeline 
  automating a workflow
  percentiles
  
-->

<a href=http://npm.im/autocannon target="_blank">
  <img style="width: 95%;margin-top: -60px;" src=images/autocannon-banner.png>
</a>
### [@davidmarkclem](http://twitter.com/davidmarkclem)

---
<!--
master: section-title
notes: |
 Pino is a high performance logger, 
 with a highly compatible bunyan interface,
 it's the fastest logger in town, Bole comes close in *some* cases

 Less time spent logging, the more time
 spent processing I/O for the intended case

 Matteo called it Pino because he's Italian 
 and there's a pine tree outside his house

 time for some rapid fire lazy clichès
-->

# Science & Magic
## The Birth of Pino
### [@davidmarkclem](http://twitter.com/davidmarkclem)

<details><summary></summary><style id=sm-bg>
#sm-bg {
  text-indent: 100%;
  white-space: nowrap;
  overflow: hidden;
  display: block;
  background: url(images/s&m.jpg);
  background-size: cover;
  padding-left: 100px;
  padding-right: 100px;
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  height: 100%;
  z-index: -1;
  opacity: .6;
  filter: invert(75%) brightness(130%) sepia(60%) blur(3px) ;
}
</style>
</details>

---
<!--
master: section-title
notes: |
 Initially used eval to precompile values into a function - 
 this can be way faster than dynamically creating functions that
 reference closure variables 

 however we knew that eval would be a deal breaker even though no 
 user input would touch this statement its just too freaky, to be 
 a serious logger we had to find another way

 we were able to rewrite without eval and get the same perf by 
 avoiding the arguments object literally a function sig of 
 pino.info(a, b, c, d, e, f, g, h, i, j, k)

-->

# Deliver us<br>from eval
### [@davidmarkclem](http://twitter.com/davidmarkclem)
<h2 style="margin-bottom: -126px; font-size: 128px;">
  <a style="color:blue" href=https://github.com/pinojs/pino/pull/1>
    #1
  </a>
</h2>

<details><summary></summary><style id=eval-bg>
#eval-bg {
  text-indent: 100%;
  white-space: nowrap;
  overflow: hidden;
  display: block;
  background: url(images/pr1.png);
  background-size: cover;
  padding-left: 100px;
  padding-right: 100px;
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  height: 100%;
  z-index: -1;
  opacity: .5;
  filter: blur(1px) sepia(110%) contrast(80%);
}
</style>
</details>

---
<!--
master: section-title
notes: |
  pino was one of the first test cases for 0x
  we discovered that JSON.stringify was our bottleneck,

  so we built strings manually whenever we could,
  for instance all top level properties that had primitive
  values could simply be concatanted onto a strings

  this gave us a 20-25% performance increase
-->

# "String Theory"
### [@davidmarkclem](http://twitter.com/davidmarkclem)
<h2 style="margin-bottom: -126px; font-size: 128px;">
  <a style="color:blue" href=https://github.com/pinojs/pino/pull/2>
    #2
  </a>
</h2>

<details><summary></summary><style id=st-bg>
#st-bg {
  text-indent: 100%;
  white-space: nowrap;
  overflow: hidden;
  display: block;
  background: url(images/pr2.png);
  background-size: cover;
  padding-left: 100px;
  padding-right: 100px;
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  height: 100%;
  z-index: -1;
  opacity: .5;
  filter: blur(1px) sepia(110%) contrast(80%);
}
</style>
</details>

---
<!--
master: section-title
notes: |
  pino has a github org, 
  where official supporting modules can be found

  like pino-http, pino-socket, pino-elasticsearch
  express-pino-logger, restify-pino-logger, hapi-pino
  pino-noir, pino-multi-stream

  we used autocannon for web integration modules
-->

<a href=http://npm.im/pino target="_blank">
  <img style="width: 94%;margin-top: 20px;" src=images/pino-eco.png>
</a>

### [@davidmarkclem](http://twitter.com/davidmarkclem)



---
<!--
master: section-title
notes: |
 so that's the pino story
-->

<a href=http://npm.im/pino target="_blank">
  <img style="width: 55%;margin-top: -20px;" src=images/pino-banner.png>
</a>

https://github.com/pinojs

### [@davidmarkclem](http://twitter.com/davidmarkclem)

---
<!--
master: section-title
notes: |
  full system end to end benchmarking
  large initial dynamically generated payload
  followed by mass-user realtime (websocket) updates 
-->

# Behind the Veil
## Of whom we speak not
### [@davidmarkclem](http://twitter.com/davidmarkclem)

---
<!--
master: section-title
notes: |
  setting up a benchmark machine (config settings)
  
  don't use AWS T2 instances for running benchmarks!
  ideal: m3.large

  avoid jumping to a clustered profiling solution, 
  often an m3.large set up correctly can supply necessary load

  check load balancer, machine and container settings,
  cloud health checks, measure cpu, mem, disk usage,
  check caching layers, then check the actual node process
-->

# Rigging
### [@davidmarkclem](http://twitter.com/davidmarkclem)

---
<!--
master: section-title
notes: |
  setting up a benchmark machine (config settings)
  
  don't use AWS T2 instances for running benchmarks!
  ideal: m3.large

  avoid jumping to a clustered profiling solution, 
  often an m3.large set up correctly can supply necessary load

  check load balancer, machine and container settings,
  cloud health checks, measure cpu, mem, disk usage,
  check caching layers, then check the actual node process
custom:
  0:
    height: 380px
    width: 550px
    margin-top: 20px
    font-size: 16px
-->

```javascript
sysctl net.core.rmem_default=268435456
sysctl net.core.wmem_default=268435456
sysctl net.core.rmem_max=268435456
sysctl net.core.wmem_max=268435456
sysctl net.core.netdev_max_backlog=100000
sysctl "net.ipv4.tcp_rmem=4096 16384 134217728"
sysctl "net.ipv4.tcp_wmem=4096 16384 134217728"
sysctl "net.ipv4.tcp_mem=786432 1048576 268435456"
sysctl net.ipv4.tcp_max_tw_buckets=360000
sysctl net.ipv4.tcp_max_syn_backlog=10000
sysctl vm.min_free_kbytes=65536
sysctl vm.swappiness=0
sysctl net.core.somaxconn=10000
sysctl net.netfilter.nf_conntrack_max=1000000
sysctl fs.file-max=65536
```

[gist.github.com/mcollina/23c788bf2f7e8da10b9c](https://gist.github.com/mcollina/23c788bf2f7e8da10b9c)

### [@davidmarkclem](http://twitter.com/davidmarkclem)


---
<!--
master: section-title
notes: |
 anger

 fan-out testing, 
 load testing vs user emulation
 (what need is there for user emulation?)
-->

# Realtime<br>Profiling
### [@davidmarkclem](http://twitter.com/davidmarkclem)

---
<!--
master: section-title
notes: |
 they've since built an automated ci 
 pipeline using autocannon
-->

# Automated<br>Reports
### [@davidmarkclem](http://twitter.com/davidmarkclem)


---
<!--
master: section-title
notes: |
  scene: a utopian future
  many people have contributed to pino, 
  0x, autocannon, autopsy and more
  others have cut their own paths,
  
  all have learned the ways of NodePerf
  
  we live in an enlightened age where the tension between
  elegance and performance is perfectly balanced by adhering
  to measurement and well established practices, and there
  is harmony among the devs

-->

# Epilogue
## A Prophecy
### [@davidmarkclem](http://twitter.com/davidmarkclem)

---
<!--
master: section-title
notes: |
  scene: a utopian future
  many people have contributed to pino, 
  0x, autocannon, autopsy and more
  others have cut their own paths,
  
  all have learned the ways of NodePerf
  
  we live in an enlightened age where the tension between
  elegance and performance is perfectly balanced by adhering
  to measurement and well established practices, and there
  is harmony among the devs
-->
<h1 id=fin> fin </h1>
<div id=creds>
  <h1> <a style="text-decoration: underline" href=http://davidmarkclements.github.io/perf-stories> Perf Stories </a> </h1>
  <h2 class=credlnk> <a href=http://davidmarkclements.github.io/perf-stories> davidmarkclements.github.io/perf-stories </a> </h2>
  <h2> <a href=http://twitter.com/davidmarkclem> @davidmarkclem </a> </h2>
  <h2> <a href=http://twitter.com/matteocollina> @matteocollina </a> </h2>  
  <h2 class=credlnk> <a href=http://npm.im/0x> npm.im/0x </a> </h2>
  <h2 class=credlnk> <a href=http://npm.im/autocannon> npm.im/autocannon </a> </h2>
  <h2 class=credlnk> <a href=http://npm.im/pino> npm.im/pino </a> </h2>
  <h2 class=credlnk> <a href=http://npm.im/autopsy> npm.im/autopsy </a> </h2>
  <h2 class=credlnk> <a href=http://github.com/pinojs> github.com/pinojs </a> </h2>
  <h2 class=credlnk> <a href=http://github.com/mcollina> github.com/mcollina </a> </h2>
  <h2 class=credlnk> <a href=http://github.com/davidmarkclements> github.com/davidmarkclements </a> </h2>
  <a href=http://nearform.com>
    <img src=images/nearform.png width=50% style='margin-top:60px;margin-bottom:-20px'>
  </a>
  <h2 class=credlnk style="font-weight: bold; margin-top: 0px"> 
    <a href=http://nearform.com>
     nearform.com
    </a> 
  </h2>

</div>

<details><summary></summary><style>
.credlnk a {
  font-size: 26px;
  font-weight: bold;
}

#creds {
  position: absolute;
  top: 110%;
  left: 0%;
  width: 100%;
  padding: 10px;
  margin-left: -5px;
  text-align: center;
}

.bespoke-active {
  overflow: hidden
}

.bespoke-active #creds {
  animation: 22s credits linear infinite;
}

.bespoke-active #fin {
  animation: 2s fin linear;
  animation-iteration-count: 1;
  opacity: 0;
  font-size: 120px;
}
@keyframes fin {
  0% {
    opacity: 1
  }
  100% {
    opacity: 0
  }
}

@keyframes credits {
  0% {
    top: 110%;
  }
  100% {
    top: -220%;
  }
}
</style>
</details>



<link href="https://fonts.googleapis.com/css?family=Cutive+Mono|Source+Sans+Pro" rel="stylesheet">
<style>
#flamegraph::before {
  display: block;
  content: '';
  border: 1px solid rgb(209,115,57);
  border-left: none;
  border-right: none;
  display: -webkit-box;
  display: -webkit-flex;
  display: -ms-flexbox;
  display: flex;
  content: '';
  height: 0;
  margin-bottom: -55px;
  margin-left: 1px;
  width: 176px;
  box-shadow: 0px 3px 10px rgb(189, 55, 30);
}


#flamegraph::after {
  display: block;
  content: '';
  border: 1px solid rgb(209,115,57);
  border-left: none;
  border-right: none;
  display: -webkit-box;
  display: -webkit-flex;
  display: -ms-flexbox;
  display: flex;
  content: '';
  height: 0;
  margin-top: -9px;
  margin-left: 201px;
  width: 76px;
  box-shadow: 0px 3px 10px rgb(189, 55, 30);
}

#fg-h3::after {
  display: block;
  content: '';
  border: 1px solid rgb(209,115,57);
  border-left: none;
  border-right: none;
  display: -webkit-box;
  display: -webkit-flex;
  display: -ms-flexbox;
  display: flex;
  content: '';
  height: 0;
  margin-top: 48px;
  margin-left: -74px;
  width: 47px;
  box-shadow: 0px 3px 10px rgb(189, 55, 30);
}
</style>
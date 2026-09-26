[x_live_demo.html](https://github.com/user-attachments/files/32689206/x_live_demo.html)
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
Phase 4: Security Headers + SSL<html><head>>

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

# OneDorkForAll

An insane list of all dorks collected from various sources including Google, Shodan, GitHub, and more.

It includes:
- Bug bounty dorks (even from private programs)
- CCTV, CMS, LFI, SQLi, XSS, and other vulnerability dorks
- 1M+ additional dorks
- Dark web dorks (📚 For **educational purposes** only!)
- Advanced job search dorks for targeted role hunting


## 📚 Recommended Resources

-  [Exploit DB Google Hacking Database](https://www.exploit-db.com/google-hacking-database)
- [Dorki.io](https://dorki.io)
-  [DorkSearch](https://dorksearch.com)
-  [DorkMe](https://dorkme.com)
-  [DorkGenius](https://dorkgenius.com)
-  [Faisal Ahmed’s Google Dork Archive](https://dorks.faisalahmed.me)
-  [Taksec's Bug Bounty Dorks](https://taksec.github.io/google-dorks-bug-bounty)
-  [BigBountyRecon (Windows App)](https://github.com/Viralmaniar/BigBountyRecon)
-  [Advanced Job Dorking Techniques (Twitter/X Thread)](https://x.com/ott3rly/status/1805173582101627035)

## 🔐 Exposed Configuration Files

```bash
filetype:config inurl:config site:http://site.com
filetype:ini inurl:wp-config.php site:http://site.com
filetype:json inurl:credentials site:http://site.com

🧠 Discovering Exposed Files
intitle:"index of" site:http://site.com
filetype:log inurl:log site:http://site.com
filetype:sql inurl:sql site:http://site.com
filetype:env inurl:.env site:http://site.com

🗂️ Sensitive Directories
inurl:/phpinfo.php site:http://site.com

🔐 Usernames and Passwords
intext:"password" filetype:log site:http://site.com
intext:"username" filetype:log site:http://site.com
filetype:sql "password" site:http://site.com

🧩 Database Files
filetype:sql inurl:db site:http://site.com
filetype:sql inurl:dump site:http://site.com
filetype:bak inurl:db site:http://site.com

🧬 Exposed Git Repositories
inurl:".git" site:http://site.com
inurl:"/.git/config" site:http://site.com
intitle:"index of" ".git" site:http://site.com

📧 Publicly Exposed Emails
intext:"email" site:http://site.com
inurl:"contact" intext:"@site.com" -www.site.com
filetype:xls inurl:"email" site:http://site.com

🧱 Vulnerable Web Servers
intitle:"Apache2 Ubuntu Default Page: It works" site:http://site.com
intitle:"Index of /" "Apache Server" site:http://site.com
intitle:"Welcome to nginx" site:http://site.com

🔑 API Key Disclosures
filetype:env "DB_PASSWORD" site:http://site.com
intext:"api_key" filetype:env site:http://site.com
intext:"AWS_ACCESS_KEY_ID" filetype:env site:http://site.com

💾 Backup Files
filetype:bak inurl:backup site:http://site.com
filetype:zip inurl:backup site:http://site.com
filetype:tgz inurl:backup site:http://site.com

🔓 Common Vulnerable Paths
inurl:/admin site:http://site.com
inurl:/backup site:http://site.com
inurl:wp- site:http://site.com




NOTE: This project is for educational and research purposes only.
Misuse of any information is strictly discouraged.
You are responsible for your actions.



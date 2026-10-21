&lt;!DOCTYPE html&gt;
&lt;html lang=&quot;en&quot;&gt;
&lt;head&gt;
&lt;meta charset=&quot;UTF-8&quot;&gt;
&lt;meta name=&quot;viewport&quot; content=&quot;width=device-width, initial-scale=1.0&quot;&gt;
&lt;title&gt;LegalEase | AI-Powered Legal Document Generator&lt;/title&gt;
&lt;style&gt;
:root{--navy:#102a43;--blue:#2563eb;--cyan:#06b6d4;--bg:#f5f8fc;--
card:#fff;--text:#172033;--muted:#667085;--border:#dce3ed;--
success:#0f766e}
*{box-sizing:border-box}html{scroll-behavior:smooth}body{margin:0;font-
family:Inter,Segoe UI,Arial,sans-serif;background:var(--bg);color:var(--
text)}
header{position:sticky;top:0;z-
index:20;background:rgba(255,255,255,.96);backdrop-
filter:blur(10px);border-bottom:1px solid var(--border)}
nav{max-width:1180px;margin:auto;display:flex;align-items:center;justify-
content:space-between;padding:15px 20px}
.logo{font-size:25px;font-weight:800;color:var(--navy)}.logo
span{color:var(--blue)}
nav a{color:#475467;text-decoration:none;margin-left:20px;font-
weight:600;font-size:14px}nav a:hover{color:var(--blue)}
.hero{background:linear-gradient(135deg,#0d2742,#173f72
55%,#0e7490);color:#fff;padding:76px 20px}
.hero-inner{max-width:1180px;margin:auto;display:grid;grid-template-
columns:1.3fr .7fr;gap:45px;align-items:center}
.badge{display:inline-block;padding:7px 12px;border:1px solid
rgba(255,255,255,.25);border-
radius:99px;background:rgba(255,255,255,.1);font-size:13px;font-
weight:700}
h1{font-size:54px;line-height:1.04;margin:18px 0}.hero p{font-
size:18px;line-height:1.7;color:#dbeafe;max-width:680px}
.btn{border:0;border-radius:10px;padding:12px 17px;font-
weight:750;cursor:pointer;text-decoration:none;display:inline-
block;margin:6px 5px 6px 0}
.primary{background:var(--
blue);color:#fff}.secondary{background:#fff;color:var(--
navy)}.ghost{background:#eaf1ff;color:#174ea6}
.hero .primary{background:#fff;color:#12345b}.hero
.secondary{background:transparent;color:#fff;border:1px solid
rgba(255,255,255,.45)}
.hero-card{background:rgba(255,255,255,.1);border:1px solid
rgba(255,255,255,.2);border-radius:18px;padding:25px;box-shadow:0 20px
50px rgba(0,0,0,.16)}
.hero-card h3{margin-top:0}.check{padding:10px 0;border-bottom:1px solid
rgba(255,255,255,.13)}
section{max-width:1180px;margin:auto;padding:65px 20px}.section-
title{font-size:32px;margin:0 0 8px;color:var(--navy)}.section-
sub{color:var(--muted);margin:0 0 28px}
.stats{display:grid;grid-template-
columns:repeat(4,1fr);gap:15px}.stat,.card,.step,.panel{background:var(--
card);border:1px solid var(--border);border-radius:16px;padding:22px;box-
shadow:0 8px 25px rgba(16,42,67,.05)}

.stat strong{display:block;font-size:28px;color:var(--blue)}.stat
span{color:var(--muted);font-size:14px}
.cards{display:grid;grid-template-
columns:repeat(3,1fr);gap:18px}.icon{font-size:30px}.card h3{margin:10px 0
7px}.card p{color:var(--muted);line-height:1.6;font-size:14px}
.steps{display:grid;grid-template-
columns:repeat(5,1fr);gap:14px}.step{text-
align:center}.num{width:42px;height:42px;border-
radius:50%;background:#eaf1ff;color:var(--blue);display:grid;place-
items:center;margin:auto;font-weight:800}
.generator-wrap{background:#eef5ff;border-top:1px solid #d9e7fb;border-
bottom:1px solid #d9e7fb}
.workspace{display:grid;grid-template-columns:360px 1fr;gap:20px}.panel
h3{margin-top:0}.form-grid{display:grid;grid-template-columns:1fr
1fr;gap:14px}
label{display:block;font-weight:700;font-size:13px;margin-
bottom:6px;color:#344054}input,select,textarea{width:100%;padding:11px
12px;border:1px solid #cfd8e3;border-
radius:9px;background:#fff;font:inherit}textarea{min-
height:100px;resize:vertical}.full{grid-column:1/-1}
.progress{height:8px;background:#e7edf5;border-
radius:99px;overflow:hidden;margin:15px 0}.progress
div{height:100%;width:33%;background:linear-gradient(90deg,var(--
blue),var(--cyan));transition:.25s}
.preview{min-height:520px;background:#fff;border:1px solid #d5dce7;border-
radius:10px;padding:38px;white-space:pre-wrap;line-height:1.75;box-
shadow:0 12px 30px rgba(16,42,67,.08)}
.preview.empty{display:grid;place-items:center;color:#98a2b3;text-
align:center}
.toolrow{display:flex;flex-wrap:wrap;gap:6px;margin-top:15px}.small{font-
size:12px;color:var(--muted);line-height:1.5}
.history{display:grid;gap:10px}.history-item{display:flex;justify-
content:space-between;gap:15px;align-items:center;border:1px solid var(--
border);background:#fff;border-radius:10px;padding:13px}
.history-item small{color:var(--muted)}.history-actions
button{border:0;background:none;color:var(--blue);font-
weight:700;cursor:pointer}
.notice{padding:12px 14px;background:#fff8e7;border:1px solid
#f3d58b;border-radius:10px;color:#76510b;font-size:13px;line-height:1.5}
details{background:#fff;border:1px solid var(--border);border-
radius:10px;padding:15px;margin:9px 0}summary{cursor:pointer;font-
weight:700}
footer{background:#0d1f33;color:#dce7f5;text-align:center;padding:30px
20px}.disclaimer{max-width:900px;margin:10px auto 0;color:#a9bad0;font-
size:12px;line-height:1.6}
.toast{position:fixed;right:20px;bottom:20px;background:#102a43;color:#fff
;padding:12px 16px;border-radius:10px;display:none;z-index:30}
@media(max-width:900px){.hero-inner,.workspace{grid-template-
columns:1fr}.cards,.stats{grid-template-columns:1fr 1fr}.steps{grid-
template-columns:1fr 1fr}h1{font-size:42px}}
@media(max-width:620px){nav a{display:none}.cards,.stats,.steps,.form-
grid{grid-template-columns:1fr}.full{grid-
column:auto}.preview{padding:22px}}

@media
print{header,.hero,section:not(#generator),.toolrow,.notice,footer,.sideba
r-actions{display:none!important}.generator-
wrap{border:0;background:#fff}.workspace{display:block}.preview{box-
shadow:none;border:0;padding:0;min-height:0}}
&lt;/style&gt;
&lt;/head&gt;
&lt;body&gt;
&lt;header&gt;
&lt;nav&gt;
&lt;div class=&quot;logo&quot;&gt;Legal&lt;span&gt;Ease&lt;/span&gt;&lt;/div&gt;
&lt;div&gt;&lt;a href=&quot;#home&quot;&gt;Home&lt;/a&gt;&lt;a href=&quot;#documents&quot;&gt;Documents&lt;/a&gt;&lt;a
href=&quot;#generator&quot;&gt;AI Generator&lt;/a&gt;&lt;a href=&quot;#history&quot;&gt;My Documents&lt;/a&gt;&lt;a
href=&quot;#faq&quot;&gt;FAQ&lt;/a&gt;&lt;/div&gt;
&lt;/nav&gt;
&lt;/header&gt;
&lt;main&gt;
&lt;section class=&quot;hero&quot; id=&quot;home&quot;&gt;
&lt;div class=&quot;hero-inner&quot;&gt;
&lt;div&gt;
&lt;span class=&quot;badge&quot;&gt;Generative AI with Google • Project Prototype&lt;/span&gt;
&lt;h1&gt;Legal Documents, Made Easier.&lt;/h1&gt;
&lt;p&gt;LegalEase is an AI-powered legal document generation platform concept.
Users provide structured information, the system transforms it into a
professional draft, and the result can be reviewed, edited, saved and
exported.&lt;/p&gt;
&lt;a class=&quot;btn primary&quot; href=&quot;#generator&quot;&gt;Start Creating&lt;/a&gt;
&lt;a class=&quot;btn secondary&quot; href=&quot;#documents&quot;&gt;Explore Documents&lt;/a&gt;
&lt;/div&gt;
&lt;div class=&quot;hero-card&quot;&gt;
&lt;h3&gt;LegalEase Workflow&lt;/h3&gt;
&lt;div class=&quot;check&quot;&gt;✓ Choose the right document type&lt;/div&gt;
&lt;div class=&quot;check&quot;&gt;✓ Complete guided information fields&lt;/div&gt;
&lt;div class=&quot;check&quot;&gt;✓ Generate a structured draft&lt;/div&gt;
&lt;div class=&quot;check&quot;&gt;✓ Review &amp; edit before use&lt;/div&gt;
&lt;div class=&quot;check&quot;&gt;✓ Save locally &amp; export to PDF&lt;/div&gt;
&lt;/div&gt;
&lt;/div&gt;
&lt;/section&gt;
&lt;section&gt;
&lt;div class=&quot;stats&quot;&gt;
&lt;div class=&quot;stat&quot;&gt;&lt;strong&gt;06&lt;/strong&gt;&lt;span&gt;Document
categories&lt;/span&gt;&lt;/div&gt;
&lt;div class=&quot;stat&quot;&gt;&lt;strong&gt;AI&lt;/strong&gt;&lt;span&gt;Generation
workflow&lt;/span&gt;&lt;/div&gt;
&lt;div class=&quot;stat&quot;&gt;&lt;strong&gt;100%&lt;/strong&gt;&lt;span&gt;Browser-based
prototype&lt;/span&gt;&lt;/div&gt;
&lt;div class=&quot;stat&quot;&gt;&lt;strong&gt;3 Mo&lt;/strong&gt;&lt;span&gt;Project-ready local
use&lt;/span&gt;&lt;/div&gt;
&lt;/div&gt;
&lt;/section&gt;

&lt;section id=&quot;documents&quot;&gt;
&lt;h2 class=&quot;section-title&quot;&gt;Document Library&lt;/h2&gt;
&lt;p class=&quot;section-sub&quot;&gt;Choose a category and LegalEase will load the
relevant information fields.&lt;/p&gt;
&lt;div class=&quot;cards&quot;&gt;
&lt;div class=&quot;card&quot;&gt;&lt;div class=&quot;icon&quot;&gt;��&lt;/div&gt;&lt;h3&gt;Rental
Agreement&lt;/h3&gt;&lt;p&gt;Property, rent, deposit, tenancy, utilities, maintenance
and permitted-use details.&lt;/p&gt;&lt;button class=&quot;btn ghost&quot;
onclick=&quot;choose(&#39;rental&#39;)&quot;&gt;Use Template&lt;/button&gt;&lt;/div&gt;
&lt;div class=&quot;card&quot;&gt;&lt;div class=&quot;icon&quot;&gt;��&lt;/div&gt;&lt;h3&gt;Employment
Agreement&lt;/h3&gt;&lt;p&gt;Employer, employee, role, salary, work location,
probation, leave and termination terms.&lt;/p&gt;&lt;button class=&quot;btn ghost&quot;
onclick=&quot;choose(&#39;employment&#39;)&quot;&gt;Use Template&lt;/button&gt;&lt;/div&gt;
&lt;div class=&quot;card&quot;&gt;&lt;div class=&quot;icon&quot;&gt;��&lt;/div&gt;&lt;h3&gt;Affidavit&lt;/h3&gt;&lt;p&gt;Deponent
information, purpose, statements and verification details.&lt;/p&gt;&lt;button
class=&quot;btn ghost&quot; onclick=&quot;choose(&#39;affidavit&#39;)&quot;&gt;Use
Template&lt;/button&gt;&lt;/div&gt;
&lt;div class=&quot;card&quot;&gt;&lt;div class=&quot;icon&quot;&gt;⚖️&lt;/div&gt;&lt;h3&gt;Simple Legal
Notice&lt;/h3&gt;&lt;p&gt;Sender, recipient, subject, facts, grievance, requested
action and response period.&lt;/p&gt;&lt;button class=&quot;btn ghost&quot;
onclick=&quot;choose(&#39;notice&#39;)&quot;&gt;Use Template&lt;/button&gt;&lt;/div&gt;
&lt;div class=&quot;card&quot;&gt;&lt;div class=&quot;icon&quot;&gt;��&lt;/div&gt;&lt;h3&gt;Confidentiality
Agreement&lt;/h3&gt;&lt;p&gt;Confidential information, permitted use, protection
duties, exclusions and duration.&lt;/p&gt;&lt;button class=&quot;btn ghost&quot;
onclick=&quot;choose(&#39;confidentiality&#39;)&quot;&gt;Use Template&lt;/button&gt;&lt;/div&gt;
&lt;div class=&quot;card&quot;&gt;&lt;div class=&quot;icon&quot;&gt;��&lt;/div&gt;&lt;h3&gt;Non-Disclosure Agreement
(NDA)&lt;/h3&gt;&lt;p&gt;Business purpose, covered information, access, security,
confidentiality and return obligations.&lt;/p&gt;&lt;button class=&quot;btn ghost&quot;
onclick=&quot;choose(&#39;nda&#39;)&quot;&gt;Use Template&lt;/button&gt;&lt;/div&gt;
&lt;/div&gt;
&lt;/section&gt;
&lt;section&gt;
&lt;h2 class=&quot;section-title&quot;&gt;How LegalEase Works&lt;/h2&gt;
&lt;p class=&quot;section-sub&quot;&gt;A clear five-stage workflow for the AI-powered
project.&lt;/p&gt;
&lt;div class=&quot;steps&quot;&gt;
&lt;div class=&quot;step&quot;&gt;&lt;div class=&quot;num&quot;&gt;1&lt;/div&gt;&lt;h3&gt;Select&lt;/h3&gt;&lt;p&gt;Pick a
document category.&lt;/p&gt;&lt;/div&gt;
&lt;div class=&quot;step&quot;&gt;&lt;div class=&quot;num&quot;&gt;2&lt;/div&gt;&lt;h3&gt;Input&lt;/h3&gt;&lt;p&gt;Enter
structured facts.&lt;/p&gt;&lt;/div&gt;
&lt;div class=&quot;step&quot;&gt;&lt;div class=&quot;num&quot;&gt;3&lt;/div&gt;&lt;h3&gt;Generate&lt;/h3&gt;&lt;p&gt;Build the
draft.&lt;/p&gt;&lt;/div&gt;
&lt;div class=&quot;step&quot;&gt;&lt;div class=&quot;num&quot;&gt;4&lt;/div&gt;&lt;h3&gt;Review&lt;/h3&gt;&lt;p&gt;Edit before
use.&lt;/p&gt;&lt;/div&gt;
&lt;div class=&quot;step&quot;&gt;&lt;div class=&quot;num&quot;&gt;5&lt;/div&gt;&lt;h3&gt;Export&lt;/h3&gt;&lt;p&gt;Save or print
PDF.&lt;/p&gt;&lt;/div&gt;
&lt;/div&gt;
&lt;/section&gt;
&lt;div class=&quot;generator-wrap&quot; id=&quot;generator&quot;&gt;
&lt;section&gt;
&lt;h2 class=&quot;section-title&quot;&gt;AI Legal Document Generator&lt;/h2&gt;

&lt;p class=&quot;section-sub&quot;&gt;Guided generation workspace — designed for your
project demonstration and repeated use.&lt;/p&gt;
&lt;div class=&quot;workspace&quot;&gt;
&lt;div class=&quot;panel&quot;&gt;
&lt;h3&gt;1. Document Details&lt;/h3&gt;
&lt;label&gt;Document Type&lt;/label&gt;
&lt;select id=&quot;type&quot; onchange=&quot;loadFields()&quot;&gt;
&lt;option value=&quot;rental&quot;&gt;Rental Agreement&lt;/option&gt;&lt;option
value=&quot;employment&quot;&gt;Employment Agreement&lt;/option&gt;&lt;option
value=&quot;affidavit&quot;&gt;Affidavit&lt;/option&gt;&lt;option value=&quot;notice&quot;&gt;Simple Legal
Notice&lt;/option&gt;&lt;option value=&quot;confidentiality&quot;&gt;Confidentiality
Agreement&lt;/option&gt;&lt;option value=&quot;nda&quot;&gt;Non-Disclosure Agreement
(NDA)&lt;/option&gt;
&lt;/select&gt;
&lt;div class=&quot;progress&quot;&gt;&lt;div id=&quot;progress&quot;&gt;&lt;/div&gt;&lt;/div&gt;
&lt;p class=&quot;small&quot; id=&quot;fieldCount&quot;&gt;&lt;/p&gt;
&lt;div id=&quot;fields&quot;&gt;&lt;/div&gt;
&lt;div class=&quot;sidebar-actions&quot;&gt;
&lt;button class=&quot;btn primary&quot; onclick=&quot;generate()&quot;&gt;✨ Generate AI
Draft&lt;/button&gt;
&lt;button class=&quot;btn ghost&quot; onclick=&quot;saveDraft()&quot;&gt;�� Save Draft&lt;/button&gt;
&lt;button class=&quot;btn&quot; onclick=&quot;clearForm()&quot;&gt;Clear Form&lt;/button&gt;
&lt;/div&gt;
&lt;div class=&quot;notice&quot;&gt;Project note: this prototype generates structured
drafts from user-provided information. It does not verify facts or
determine legal validity.&lt;/div&gt;
&lt;/div&gt;
&lt;div class=&quot;panel&quot;&gt;
&lt;h3&gt;2. AI-Generated Document Preview&lt;/h3&gt;
&lt;div id=&quot;preview&quot; class=&quot;preview empty&quot;&gt;Your generated legal document will
appear here.&lt;br&gt;&lt;br&gt;Fill the required information and select “Generate AI
Draft”.&lt;/div&gt;
&lt;div class=&quot;toolrow&quot;&gt;
&lt;button class=&quot;btn primary&quot; onclick=&quot;copyDraft()&quot;&gt;Copy&lt;/button&gt;
&lt;button class=&quot;btn ghost&quot; onclick=&quot;window.print()&quot;&gt;Print / Save
PDF&lt;/button&gt;
&lt;button class=&quot;btn ghost&quot; onclick=&quot;downloadTxt()&quot;&gt;Download .TXT&lt;/button&gt;
&lt;/div&gt;
&lt;p class=&quot;small&quot;&gt;Tip: You can edit the generated content directly in the
preview before printing.&lt;/p&gt;
&lt;/div&gt;
&lt;/div&gt;
&lt;/section&gt;
&lt;/div&gt;
&lt;section id=&quot;history&quot;&gt;
&lt;h2 class=&quot;section-title&quot;&gt;My Documents&lt;/h2&gt;
&lt;p class=&quot;section-sub&quot;&gt;Saved drafts are stored in this browser using local
storage, so you can reuse the website during your project period on the
same browser/device.&lt;/p&gt;
&lt;div id=&quot;historyList&quot; class=&quot;history&quot;&gt;&lt;/div&gt;
&lt;/section&gt;

&lt;section id=&quot;faq&quot;&gt;
&lt;h2 class=&quot;section-title&quot;&gt;FAQ&lt;/h2&gt;
&lt;details&gt;&lt;summary&gt;What is LegalEase?&lt;/summary&gt;&lt;p&gt;LegalEase is a Generative
AI project concept for converting structured user inputs into readable
legal-document drafts.&lt;/p&gt;&lt;/details&gt;
&lt;details&gt;&lt;summary&gt;Is this a real legal service?&lt;/summary&gt;&lt;p&gt;No. It is a
project prototype. Generated documents should be reviewed by an
appropriately qualified legal professional before real-world
use.&lt;/p&gt;&lt;/details&gt;
&lt;details&gt;&lt;summary&gt;Will my saved drafts remain?&lt;/summary&gt;&lt;p&gt;Saved drafts
use browser localStorage. They normally remain on the same browser/device
until its site data is cleared. This version does not provide cloud
backup.&lt;/p&gt;&lt;/details&gt;
&lt;details&gt;&lt;summary&gt;Can I use the website for three months?&lt;/summary&gt;&lt;p&gt;Yes.
There is no built-in expiry date. For dependable project use, keep a
backup copy of the HTML file and export important documents as
PDF/TXT.&lt;/p&gt;&lt;/details&gt;
&lt;details&gt;&lt;summary&gt;Is the AI API connected?&lt;/summary&gt;&lt;p&gt;This version
contains the complete AI-style generation workflow and is designed so a
Gemini API/backend can be connected later. The current standalone file
does not expose an API key or require a server.&lt;/p&gt;&lt;/details&gt;
&lt;/section&gt;
&lt;/main&gt;
&lt;footer&gt;
&lt;strong&gt;LegalEase&lt;/strong&gt; — AI-Powered Legal Document Generator
&lt;div class=&quot;disclaimer&quot;&gt;Educational project prototype. This website does
not provide legal advice, verify facts, or guarantee legal validity.
Document requirements may vary by jurisdiction, transaction and purpose.
Review generated content with a qualified legal professional before
signing or relying on it.&lt;/div&gt;
&lt;/footer&gt;
&lt;div class=&quot;toast&quot; id=&quot;toast&quot;&gt;&lt;/div&gt;
&lt;script&gt;
const schemas={
rental:[
[&quot;Agreement Date&quot;,&quot;agreementDate&quot;,&quot;date&quot;],[&quot;Landlord Full
Name&quot;,&quot;landlord&quot;,&quot;text&quot;],[&quot;Landlord
Address&quot;,&quot;landlordAddress&quot;,&quot;textarea&quot;],[&quot;Tenant Full
Name&quot;,&quot;tenant&quot;,&quot;text&quot;],[&quot;Tenant
Address&quot;,&quot;tenantAddress&quot;,&quot;textarea&quot;],[&quot;Property
Address&quot;,&quot;property&quot;,&quot;textarea&quot;],[&quot;Monthly Rent
(₹)&quot;,&quot;rent&quot;,&quot;text&quot;],[&quot;Security Deposit (₹)&quot;,&quot;deposit&quot;,&quot;text&quot;],[&quot;Tenancy
Start Date&quot;,&quot;startDate&quot;,&quot;date&quot;],[&quot;Tenancy End
Date&quot;,&quot;endDate&quot;,&quot;date&quot;],[&quot;Notice
Period&quot;,&quot;noticePeriod&quot;,&quot;text&quot;],[&quot;Utilities /
Bills&quot;,&quot;utilities&quot;,&quot;textarea&quot;],[&quot;Maintenance
Responsibilities&quot;,&quot;maintenance&quot;,&quot;textarea&quot;],[&quot;Permitted
Use&quot;,&quot;use&quot;,&quot;textarea&quot;],[&quot;Additional Terms&quot;,&quot;additional&quot;,&quot;textarea&quot;]],
employment:[
[&quot;Agreement Date&quot;,&quot;agreementDate&quot;,&quot;date&quot;],[&quot;Employer /
Company&quot;,&quot;employer&quot;,&quot;text&quot;],[&quot;Employer
Address&quot;,&quot;employerAddress&quot;,&quot;textarea&quot;],[&quot;Employee Full

Name&quot;,&quot;employee&quot;,&quot;text&quot;],[&quot;Employee
Address&quot;,&quot;employeeAddress&quot;,&quot;textarea&quot;],[&quot;Job Title /
Role&quot;,&quot;role&quot;,&quot;text&quot;],[&quot;Joining Date&quot;,&quot;joiningDate&quot;,&quot;date&quot;],[&quot;Work
Location&quot;,&quot;workLocation&quot;,&quot;text&quot;],[&quot;Salary /
Compensation&quot;,&quot;salary&quot;,&quot;text&quot;],[&quot;Working Hours&quot;,&quot;hours&quot;,&quot;text&quot;],[&quot;Leave /
Benefits&quot;,&quot;benefits&quot;,&quot;textarea&quot;],[&quot;Probation
Period&quot;,&quot;probation&quot;,&quot;text&quot;],[&quot;Notice / Termination
Terms&quot;,&quot;termination&quot;,&quot;textarea&quot;],[&quot;Confidentiality / IP
Terms&quot;,&quot;ip&quot;,&quot;textarea&quot;],[&quot;Other Duties &amp;
Conditions&quot;,&quot;duties&quot;,&quot;textarea&quot;]],
affidavit:[
[&quot;Date&quot;,&quot;date&quot;,&quot;date&quot;],[&quot;Deponent Full
Name&quot;,&quot;deponent&quot;,&quot;text&quot;],[&quot;Age&quot;,&quot;age&quot;,&quot;text&quot;],[&quot;Parent / Spouse
Name&quot;,&quot;relation&quot;,&quot;text&quot;],[&quot;Residential
Address&quot;,&quot;address&quot;,&quot;textarea&quot;],[&quot;Occupation&quot;,&quot;occupation&quot;,&quot;text&quot;],[&quot;Purpos
e of Affidavit&quot;,&quot;purpose&quot;,&quot;textarea&quot;],[&quot;Statement
1&quot;,&quot;statement1&quot;,&quot;textarea&quot;],[&quot;Statement
2&quot;,&quot;statement2&quot;,&quot;textarea&quot;],[&quot;Statement
3&quot;,&quot;statement3&quot;,&quot;textarea&quot;],[&quot;Additional
Statements&quot;,&quot;additional&quot;,&quot;textarea&quot;],[&quot;Place of
Verification&quot;,&quot;place&quot;,&quot;text&quot;]],
notice:[
[&quot;Notice Date&quot;,&quot;noticeDate&quot;,&quot;date&quot;],[&quot;Sender
Name&quot;,&quot;sender&quot;,&quot;text&quot;],[&quot;Sender
Address&quot;,&quot;senderAddress&quot;,&quot;textarea&quot;],[&quot;Recipient
Name&quot;,&quot;recipient&quot;,&quot;text&quot;],[&quot;Recipient
Address&quot;,&quot;recipientAddress&quot;,&quot;textarea&quot;],[&quot;Subject&quot;,&quot;subject&quot;,&quot;text&quot;],[&quot;Rel
ationship / Transaction&quot;,&quot;relationship&quot;,&quot;textarea&quot;],[&quot;Relevant
Date(s)&quot;,&quot;dates&quot;,&quot;text&quot;],[&quot;Facts / Background&quot;,&quot;facts&quot;,&quot;textarea&quot;],[&quot;Issue
/ Breach / Grievance&quot;,&quot;issue&quot;,&quot;textarea&quot;],[&quot;Action
Requested&quot;,&quot;action&quot;,&quot;textarea&quot;],[&quot;Response
Period&quot;,&quot;response&quot;,&quot;text&quot;],[&quot;Consequences / Further Action (if
applicable)&quot;,&quot;consequences&quot;,&quot;textarea&quot;],[&quot;Attachments / Supporting
Documents&quot;,&quot;attachments&quot;,&quot;textarea&quot;],[&quot;Contact for
Response&quot;,&quot;contact&quot;,&quot;text&quot;]],
confidentiality:[
[&quot;Agreement Date&quot;,&quot;agreementDate&quot;,&quot;date&quot;],[&quot;Disclosing
Party&quot;,&quot;disclosing&quot;,&quot;text&quot;],[&quot;Disclosing Party
Address&quot;,&quot;disclosingAddress&quot;,&quot;textarea&quot;],[&quot;Receiving
Party&quot;,&quot;receiving&quot;,&quot;text&quot;],[&quot;Receiving Party
Address&quot;,&quot;receivingAddress&quot;,&quot;textarea&quot;],[&quot;Purpose of
Disclosure&quot;,&quot;purpose&quot;,&quot;textarea&quot;],[&quot;Definition of Confidential
Information&quot;,&quot;confidentialInfo&quot;,&quot;textarea&quot;],[&quot;Permitted
Use&quot;,&quot;permittedUse&quot;,&quot;textarea&quot;],[&quot;Exclusions from Confidential
Information&quot;,&quot;exclusions&quot;,&quot;textarea&quot;],[&quot;Security / Protection
Duties&quot;,&quot;security&quot;,&quot;textarea&quot;],[&quot;Confidentiality
Period&quot;,&quot;period&quot;,&quot;text&quot;],[&quot;Return / Destruction of
Information&quot;,&quot;return&quot;,&quot;textarea&quot;],[&quot;Permitted Disclosure / Legal
Requirement&quot;,&quot;legalDisclosure&quot;,&quot;textarea&quot;],[&quot;Governing Law /
Jurisdiction&quot;,&quot;law&quot;,&quot;text&quot;],[&quot;Additional Terms&quot;,&quot;additional&quot;,&quot;textarea&quot;]],
nda:[
[&quot;Agreement Date&quot;,&quot;agreementDate&quot;,&quot;date&quot;],[&quot;Disclosing Party /
Company&quot;,&quot;disclosing&quot;,&quot;text&quot;],[&quot;Disclosing Party
Address&quot;,&quot;disclosingAddress&quot;,&quot;textarea&quot;],[&quot;Receiving Party /

Company&quot;,&quot;receiving&quot;,&quot;text&quot;],[&quot;Receiving Party
Address&quot;,&quot;receivingAddress&quot;,&quot;textarea&quot;],[&quot;Business / Project
Purpose&quot;,&quot;purpose&quot;,&quot;textarea&quot;],[&quot;Confidential Information
Covered&quot;,&quot;confidentialInfo&quot;,&quot;textarea&quot;],[&quot;Permitted Purpose /
Use&quot;,&quot;permittedUse&quot;,&quot;textarea&quot;],[&quot;Information
Exclusions&quot;,&quot;exclusions&quot;,&quot;textarea&quot;],[&quot;Security
Measures&quot;,&quot;security&quot;,&quot;textarea&quot;],[&quot;Employees / Representatives
Access&quot;,&quot;access&quot;,&quot;textarea&quot;],[&quot;Confidentiality
Period&quot;,&quot;period&quot;,&quot;text&quot;],[&quot;Return /
Destruction&quot;,&quot;return&quot;,&quot;textarea&quot;],[&quot;Breach / Remedies Clause
(draft)&quot;,&quot;remedies&quot;,&quot;textarea&quot;],[&quot;Governing Law /
Jurisdiction&quot;,&quot;law&quot;,&quot;text&quot;],[&quot;Additional
Terms&quot;,&quot;additional&quot;,&quot;textarea&quot;],[&quot;Disclosing Party Signatory
Name&quot;,&quot;signatory1&quot;,&quot;text&quot;],[&quot;Receiving Party Signatory
Name&quot;,&quot;signatory2&quot;,&quot;text&quot;]]
};
let lastDraft=&quot;&quot;, lastTitle=&quot;&quot;;
function
choose(type){document.getElementById(&quot;type&quot;).value=type;loadFields();docum
ent.getElementById(&quot;generator&quot;).scrollIntoView({behavior:&quot;smooth&quot;});}
function loadFields(){
const type=document.getElementById(&quot;type&quot;).value,
box=document.getElementById(&quot;fields&quot;), arr=schemas[type];
box.innerHTML=arr.map((f,i)=&gt;`&lt;div style=&quot;margin:12px
0&quot;&gt;&lt;label&gt;${f[0]}${i&lt;2?&quot; *&quot;:&quot;&quot;}&lt;/label&gt;${f[2]===&quot;textarea&quot;?`&lt;textarea
id=&quot;f_${f[1]}&quot; placeholder=&quot;Enter
${f[0].toLowerCase()}&quot;&gt;&lt;/textarea&gt;`:`&lt;input id=&quot;f_${f[1]}&quot; type=&quot;${f[2]}&quot;
placeholder=&quot;Enter ${f[0].toLowerCase()}&quot;&gt;`}&lt;/div&gt;`).join(&quot;&quot;);
document.getElementById(&quot;fieldCount&quot;).textContent=arr.length+&quot; guided
fields available for this document.&quot;;
document.getElementById(&quot;progress&quot;).style.width=Math.min(92,25+arr.length*
3)+&quot;%&quot;;
}
function val(key){const e=document.getElementById(&quot;f_&quot;+key);return
e&amp;&amp;e.value.trim()?e.value.trim():&quot;[Not provided]&quot;;}
function heading(s){return
&quot;\n\n&quot;+s.toUpperCase()+&quot;\n&quot;+(&quot;=&quot;.repeat(Math.min(58,s.length+2)))+&quot;\n&quot;;}
function generate(){
const type=document.getElementById(&quot;type&quot;).value, arr=schemas[type];
if(!val(arr[0][1])||!val(arr[1][1])){toast(&quot;Please fill the first
required fields.&quot;);return;}
const names={rental:&quot;RENTAL AGREEMENT&quot;,employment:&quot;EMPLOYMENT
AGREEMENT&quot;,affidavit:&quot;AFFIDAVIT&quot;,notice:&quot;LEGAL
NOTICE&quot;,confidentiality:&quot;CONFIDENTIALITY AGREEMENT&quot;,nda:&quot;NON-DISCLOSURE
AGREEMENT (NDA)&quot;};
let out=names[type]+heading(&quot;DOCUMENT DETAILS&quot;);
arr.forEach(f=&gt;{out+=f[0]+&quot;: &quot;+val(f[1])+&quot;\n&quot;;});
out+=heading(&quot;DRAFTING NOTE&quot;)+&quot;This structured draft was generated from
the information entered into LegalEase. Review names, dates, amounts,
obligations, jurisdiction-specific requirements and all clauses before
signing or relying on the document.\n&quot;;
out+=&quot;\nSIGNATURES\n\nDisclosing / First Party:
______________________________\nReceiving / Second Party:
_____________________________\nDate: __________________\n&quot;;

lastDraft=out.trim();lastTitle=names[type];
const
p=document.getElementById(&quot;preview&quot;);p.classList.remove(&quot;empty&quot;);p.content
Editable=&quot;true&quot;;p.textContent=lastDraft;
p.scrollIntoView({behavior:&quot;smooth&quot;,block:&quot;start&quot;});toast(&quot;Draft
generated successfully.&quot;);
}
function copyDraft(){const
text=document.getElementById(&quot;preview&quot;).innerText.trim();if(!text){toast(&quot;
Generate a draft
first.&quot;);return;}navigator.clipboard.writeText(text);toast(&quot;Draft
copied.&quot;);}
function saveDraft(){
const
text=document.getElementById(&quot;preview&quot;).innerText.trim();if(!text){toast(&quot;
Generate a draft first.&quot;);return;}
const
arr=JSON.parse(localStorage.getItem(&quot;legaleaseDocs&quot;)||&quot;[]&quot;);arr.unshift({i
d:Date.now(),title:lastTitle||&quot;Legal Document&quot;,text,date:new
Date().toLocaleString()});localStorage.setItem(&quot;legaleaseDocs&quot;,JSON.string
ify(arr.slice(0,20)));renderHistory();toast(&quot;Draft saved to My
Documents.&quot;);
}
function renderHistory(){
const arr=JSON.parse(localStorage.getItem(&quot;legaleaseDocs&quot;)||&quot;[]&quot;),
box=document.getElementById(&quot;historyList&quot;);
if(!arr.length){box.innerHTML=&#39;&lt;div class=&quot;panel&quot;&gt;No saved drafts yet.
Generate a document and click “Save Draft”.&lt;/div&gt;&#39;;return;}
box.innerHTML=arr.map(x=&gt;`&lt;div class=&quot;history-
item&quot;&gt;&lt;div&gt;&lt;b&gt;${x.title}&lt;/b&gt;&lt;br&gt;&lt;small&gt;${x.date}&lt;/small&gt;&lt;/div&gt;&lt;div
class=&quot;history-actions&quot;&gt;&lt;button
onclick=&quot;openSaved(${x.id})&quot;&gt;Open&lt;/button&gt;&lt;button
onclick=&quot;deleteSaved(${x.id})&quot;&gt;Delete&lt;/button&gt;&lt;/div&gt;&lt;/div&gt;`).join(&quot;&quot;);
}
function openSaved(id){const
x=JSON.parse(localStorage.getItem(&quot;legaleaseDocs&quot;)||&quot;[]&quot;).find(a=&gt;a.id===i
d);if(!x)return;lastDraft=x.text;lastTitle=x.title;const
p=document.getElementById(&quot;preview&quot;);p.classList.remove(&quot;empty&quot;);p.content
Editable=&quot;true&quot;;p.textContent=x.text;document.getElementById(&quot;generator&quot;).
scrollIntoView({behavior:&quot;smooth&quot;});}
function
deleteSaved(id){localStorage.setItem(&quot;legaleaseDocs&quot;,JSON.stringify(JSON.p
arse(localStorage.getItem(&quot;legaleaseDocs&quot;)||&quot;[]&quot;).filter(x=&gt;x.id!==id)));r
enderHistory();toast(&quot;Saved draft deleted.&quot;);}
function clearForm(){document.querySelectorAll(&quot;#fields input,#fields
textarea&quot;).forEach(e=&gt;e.value=&quot;&quot;);const
p=document.getElementById(&quot;preview&quot;);p.classList.add(&quot;empty&quot;);p.contentEdi
table=&quot;false&quot;;p.textContent=&quot;Your generated legal document will appear
here.&quot;;lastDraft=&quot;&quot;;toast(&quot;Form cleared.&quot;);}
function downloadTxt(){const
text=document.getElementById(&quot;preview&quot;).innerText.trim();if(!text){toast(&quot;
Generate a draft first.&quot;);return;}const
a=document.createElement(&quot;a&quot;);a.href=URL.createObjectURL(new
Blob([text],{type:&quot;text/plain&quot;}));a.download=(lastTitle||&quot;LegalEase_Docume

nt&quot;).replace(/[^a-z0-
9]+/gi,&quot;_&quot;)+&quot;.txt&quot;;a.click();URL.revokeObjectURL(a.href);}
function toast(msg){const
t=document.getElementById(&quot;toast&quot;);t.textContent=msg;t.style.display=&quot;bloc
k&quot;;clearTimeout(window._toast);window._toast=setTimeout(()=&gt;t.style.displa
y=&quot;none&quot;,2200);}
loadFields();renderHistory();
&lt;/script&gt;
&lt;/body&gt;
&lt;/html&gt;

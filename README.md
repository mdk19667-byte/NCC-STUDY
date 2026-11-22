<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>NCC-1 (AEC-IV) Sem IV - 5 Hour Study Planner</title>
<style>
:root{--bg:#0d1117;--panel:#161b22;--panel2:#1c2330;--line:#2a3342;--tx:#e6edf3;--mut:#8b98a9;--acc:#3fb950;--acc2:#58a6ff;--warn:#f0b429;--bad:#f85149;--rad:12px}
*{box-sizing:border-box;margin:0;padding:0}
html,body{height:100%}
body{background:var(--bg);color:var(--tx);font-family:Segoe UI,system-ui,-apple-system,Roboto,Arial,sans-serif;line-height:1.6;font-size:16px}
button{font:inherit;cursor:pointer;border:0;color:inherit}
.app{display:flex;min-height:100vh}
aside{width:290px;background:var(--panel);border-right:1px solid var(--line);position:fixed;top:0;bottom:0;left:0;overflow-y:auto;z-index:30;padding:14px;transition:transform .25s}
.brand{font-weight:700;font-size:1.05rem;margin-bottom:2px}
.brand small{display:block;color:var(--mut);font-weight:400;font-size:.78rem}
.nav-btn{display:flex;align-items:center;gap:8px;width:100%;text-align:left;background:transparent;padding:9px 10px;border-radius:9px;color:var(--tx);margin-top:4px;font-size:.93rem}
.nav-btn:hover{background:var(--panel2)}
.nav-btn.on{background:#1f6feb33;color:#fff;outline:1px solid #1f6feb66}
.sec-title{color:var(--mut);font-size:.72rem;text-transform:uppercase;letter-spacing:.08em;margin:16px 4px 4px}
.unit{margin-top:6px;border:1px solid var(--line);border-radius:10px;overflow:hidden}
.unit-h{width:100%;background:var(--panel2);padding:9px 10px;text-align:left}
.unit-h b{display:block;font-size:.9rem}
.unit-h span{font-size:.75rem;color:var(--mut)}
.mini{height:5px;background:#0b0f14;border-radius:9px;margin-top:5px;overflow:hidden}
.mini i{display:block;height:100%;background:var(--acc);width:0;transition:width .3s}
.tlist button{display:block;width:100%;text-align:left;background:transparent;padding:6px 10px 6px 12px;font-size:.82rem;color:var(--mut);border-top:1px solid #20283a}
.tlist button:hover{color:var(--tx);background:#1a2130}
.tlist button.on{color:#fff;background:#1f6feb2a}
.tlist button.ok::before{content:"\2713 ";color:var(--acc)}
main{margin-left:290px;flex:1;min-width:0}
.top{position:sticky;top:0;z-index:20;background:#0d1117ee;backdrop-filter:blur(6px);border-bottom:1px solid var(--line);display:flex;align-items:center;gap:10px;padding:10px 16px;flex-wrap:wrap}
.burger{display:none;background:var(--panel2);padding:7px 11px;border-radius:8px;font-size:1.1rem}
.timer{display:flex;align-items:center;gap:10px;background:var(--panel);border:1px solid var(--line);border-radius:10px;padding:6px 12px}
.timer .t{font-variant-numeric:tabular-nums;font-size:1.25rem;font-weight:700;color:var(--warn)}
.timer small{color:var(--mut);display:block;font-size:.68rem;line-height:1}
.grow{flex:1}
.btn{padding:8px 14px;border-radius:9px;background:var(--panel2);border:1px solid var(--line);font-size:.9rem}
.btn:hover{border-color:#3d4a60}
.btn.pri{background:var(--acc);color:#04120a;font-weight:700;border-color:var(--acc)}
.btn.blue{background:#1f6feb;border-color:#1f6feb;color:#fff}
.btn.danger{color:var(--bad)}
.btn:disabled{opacity:.4;cursor:not-allowed}
.gbar{height:8px;background:#0b0f14;border-radius:9px;overflow:hidden;border:1px solid var(--line)}
.gbar i{display:block;height:100%;background:linear-gradient(90deg,var(--acc),var(--acc2));width:0;transition:width .3s}
.wrap{padding:18px 18px 70px;max-width:980px;margin:0 auto}
h1{font-size:1.5rem;margin-bottom:4px}
h2{font-size:1.2rem;margin:18px 0 8px}
h3{font-size:1.02rem;margin:0 0 6px}
h4{font-size:.95rem;margin:12px 0 4px;color:var(--acc2)}
.sub{color:var(--mut);font-size:.92rem}
.card{background:var(--panel);border:1px solid var(--line);border-radius:var(--rad);padding:16px;margin-top:14px}
.grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(210px,1fr));gap:12px;margin-top:12px}
.stat{background:var(--panel);border:1px solid var(--line);border-radius:var(--rad);padding:14px}
.stat b{font-size:1.5rem;display:block}
table{width:100%;border-collapse:collapse;font-size:.9rem}
th,td{padding:8px 6px;border-bottom:1px solid var(--line);text-align:left}
th{color:var(--mut);font-weight:600;font-size:.78rem;text-transform:uppercase}
.row{display:flex;gap:8px;flex-wrap:wrap;align-items:center}
.chip{display:inline-block;background:#1f6feb22;border:1px solid #1f6feb66;color:#a5c8ff;border-radius:99px;padding:2px 10px;font-size:.8rem;margin:3px 4px 3px 0}
.hing{border-left:4px solid var(--warn)}
.exm{border-left:4px solid var(--acc)}
.mem{border-left:4px solid #bc8cff}
.exa{border-left:4px solid var(--acc2)}
.lbl{font-size:.72rem;text-transform:uppercase;letter-spacing:.08em;color:var(--mut);margin-bottom:4px;font-weight:700}
ol,ul{margin:4px 0 4px 22px}
li{margin:3px 0}
.opt{display:block;width:100%;text-align:left;background:var(--panel2);border:1px solid var(--line);border-radius:9px;padding:9px 12px;margin-top:6px}
.opt:hover:not(.lock){border-color:var(--acc2)}
.opt.right{background:#1b3a25;border-color:var(--acc)}
.opt.wrong{background:#3d1a1d;border-color:var(--bad)}
.expl{margin-top:8px;padding:9px 12px;border-radius:9px;background:#0b0f14;border:1px dashed var(--line);font-size:.9rem}
details{background:var(--panel2);border:1px solid var(--line);border-radius:10px;padding:9px 12px;margin-top:8px}
summary{cursor:pointer;font-weight:600}
textarea{width:100%;min-height:150px;background:#0b0f14;color:var(--tx);border:1px solid var(--line);border-radius:10px;padding:10px;font:inherit;resize:vertical}
.nav2{display:flex;justify-content:space-between;gap:8px;margin-top:18px;flex-wrap:wrap}
.done-btn.isdone{background:#1b3a25;border-color:var(--acc);color:#7ee2a0}
.big{font-size:2rem;font-weight:800}
.ok{color:var(--acc)}.bad{color:var(--bad)}
select{background:var(--panel2);color:var(--tx);border:1px solid var(--line);border-radius:9px;padding:8px}
.overlay{display:none;position:fixed;inset:0;background:#0009;z-index:25}
@media(max-width:860px){
aside{transform:translateX(-100%);width:84%;max-width:320px}
body.menu aside{transform:none}
body.menu .overlay{display:block}
main{margin-left:0}
.burger{display:block}
.wrap{padding:14px 12px 70px}
.timer .t{font-size:1.05rem}
}
</style>
</head>
<body>
<div class="overlay" id="ov"></div>
<div class="app">
<aside id="side"></aside>
<main>
<div class="top">
<button class="burger" id="burger" aria-label="Menu">&#9776;</button>
<div class="timer"><div><small>STUDY TIME LEFT (5h)</small><span class="t" id="tm">05:00:00</span></div></div>
<button class="btn pri" id="startBtn">Start Study</button>
<div class="grow" style="min-width:120px"><div class="gbar"><i id="gp"></i></div><div class="sub" style="font-size:.75rem" id="gt"></div></div>
<button class="btn danger" id="resetBtn">Reset</button>
</div>
<div class="wrap" id="view"></div>
</main>
</div>

<script>
/* ================= HELPERS ================= */
const T=(title,h,ex,intro,pts,concl,kw,mt,mcq,sq,sa)=>({title,d:intro.split(". ")[0].replace(/\.$/,"")+".",h,ex,intro,pts,concl,kw,mt,mcq,sq,sa});
const M=(q,o,a,e)=>({q,o,a,e});

/* ================= CONTENT ================= */
const UNITS=[
{n:"Unit I",name:"NCC",min:60,topics:[
T("Importance of NCC in promoting national integration",
"National integration means 'hum sab Indian hain' ka feeling. Bhai, India mein alag alag bhasha, dharm aur jaati ke log rehte hain. NCC mein sab cadets ek hi uniform pehente hain, ek saath rehte, khaate aur parade karte hain. Isse bhed-bhav khatam hota hai aur oneness aati hai.",
"In a camp, a cadet from Punjab, one from Kerala and one from Assam share one tent and eat together. After 10 days they become close friends and forget regional differences.",
"National integration means unity of all citizens of the country, in spite of differences of religion, language, caste and region. NCC plays a big role in this by bringing youth of every part of India together under its motto 'Unity and Discipline'.",
["Common uniform and identity: all cadets look the same, so rich-poor and caste differences disappear.","Mixed living in camps: cadets of different states live, eat and train together.","National Integration Camps (NIC): special camps where cadets from all states meet and share culture.","Youth Exchange Programme: cadets visit other states and countries and learn about other cultures.","Secular outlook: all religions are respected; every festival is celebrated together.","Joint activities: Republic Day parade, disaster relief and social service build team spirit.","National pride: flag hoisting, pledge and parades create love for the nation."],
"In short, NCC acts like a mini India where every cadet is treated equally. It builds unity, secular thinking and patriotism, which makes the nation strong.",
["Unity and Discipline","Common uniform","National Integration Camp","Secular outlook","Oneness","Youth Exchange","Unity in diversity"],
"Remember 'CUMS': Camps, Uniform, Mixing, Secularism.",
[M("What is the motto of NCC?",["Duty and Honour","Unity and Discipline","Service Before Self","Truth and Courage"],1,"The NCC motto is 'Unity and Discipline' (Ekta aur Anushasan)."),
M("Which camp brings cadets of all states together to build oneness?",["Thal Sainik Camp","Army Attachment Camp","National Integration Camp","Trekking Camp"],2,"The National Integration Camp (NIC) is meant to promote unity among cadets of different states.")],
"How does NCC promote national integration? (5 marks)",
"NCC brings cadets of all religions, regions and languages together in camps, parades and social service under one uniform and one motto. This creates oneness, secular outlook and national pride."),

T("NCC and leadership / personality development",
"Leader banne ke liye decision lena, team ko guide karna aur zimmedari uthana aana chahiye. NCC mein cadets ko squad ya platoon command karne ko milta hai, speech dene ko milta hai. Isse confidence aur personality dono badhte hain.",
"A senior cadet is made squad leader for a parade. He plans, gives commands and corrects mistakes. After a few months he can speak confidently in front of 100 people.",
"Leadership is the ability to guide and motivate others towards a goal. Personality development means improving a person's overall behaviour, confidence and skills. NCC gives cadets many chances to grow in both.",
["Command opportunities: cadets lead squads, sections and parades.","Drill and parade: improves voice, posture and bearing.","Public speaking: group discussions and lectures improve communication.","Teamwork: working with others teaches cooperation and trust.","Decision making: camps and training give real situations to decide quickly.","Responsibility: duties like guard, orderly and camp work build a sense of duty.","Self-confidence: awards, certificates and recognition raise confidence."],
"Thus NCC turns shy and average students into confident, disciplined and responsible leaders who are useful to society.",
["Leadership","Command","Confidence","Teamwork","Responsibility","Communication","Self-discipline"],
"LEAD = Learn, Execute, Advise, Decide.",
[M("Which quality grows when a cadet commands a squad?",["Laziness","Leadership","Shyness","Carelessness"],1,"Commanding others develops leadership."),
M("Which one is NOT a leadership quality?",["Courage","Honesty","Indecision","Responsibility"],2,"Indecision (not being able to decide) is a weakness, not a leadership quality.")],
"Explain how NCC develops leadership and personality. (5 marks)",
"By giving command chances, drill, public speaking, teamwork and responsibility, NCC builds confidence, communication and decision-making in cadets."),

T("Activities promoting physical fitness and discipline",
"Fit body aur disciplined mind NCC ki pehchaan hai. Roz PT, drill, running, route march, trekking aur sports hote hain. Time par aana, order maanna aur uniform theek rakhna discipline sikhata hai.",
"A cadet wakes up at 5 AM for PT every day in camp. In two weeks his stamina improves and he is never late for anything.",
"Physical fitness and discipline are the base of NCC training. A healthy and disciplined youth is useful for the nation and for the armed forces.",
["Physical Training (PT): exercises, running and stretching improve strength and stamina.","Drill and parade: improves coordination, alertness and obedience.","Route march and trekking: build endurance and love for nature.","Games and sports: develop team spirit and fair play.","Yoga and meditation: improve focus and calm the mind.","Obstacle training and adventure activities: rock climbing, para-sailing, cycling and sailing build courage.","Rules of camp: wake-up call, dress code and punctuality teach self-discipline."],
"Through these activities NCC makes cadets physically strong, mentally alert and self-disciplined citizens.",
["PT","Drill","Route march","Trekking","Yoga","Adventure","Punctuality"],
"PADS = Parade, Adventure, Drill, Sports.",
[M("Which activity mainly teaches obedience and coordination?",["Drill","Painting","Singing","Reading"],0,"Drill and parade teach obedience, coordination and alertness."),
M("Rock climbing is an example of a/an ___ activity.",["Cultural","Adventure","Academic","Clerical"],1,"Rock climbing, trekking and sailing are adventure activities of NCC.")],
"Name five NCC activities that promote physical fitness and discipline. (3 marks)",
"PT, drill and parade, route march and trekking, games and sports, yoga, and adventure activities like rock climbing."),

T("NCC contribution to social service",
"NCC sirf parade nahi hai, samaj ki seva bhi hai. Cadets blood donation camp lagate hain, ped lagate hain, safai abhiyan chalate hain aur baadh ya bhukamp mein madad karte hain.",
"During floods, NCC cadets help villagers move to safe places and distribute food and water packets.",
"Social service means helping society without expecting anything in return. NCC trains cadets to serve the community with a spirit of selfless service, which is also one of its aims.",
["Blood donation and health camps: cadets donate blood and help in check-ups.","Tree plantation and environment: planting trees, cleaning rivers and beaches.","Swachh Bharat activities: cleanliness drives in villages and cities.","Literacy and awareness: teaching poor children and rallies on drugs, road safety and health.","Disaster relief: help during floods, earthquakes, fires and pandemics.","Village adoption and community work: building toilets, repairing roads and wells.","Support to elderly and needy: visits to old-age homes and orphanages."],
"NCC cadets thus become responsible citizens who work for the welfare of society and the nation.",
["Selfless service","Blood donation","Tree plantation","Swachh Bharat","Disaster relief","Awareness rally","Community"],
"BEST = Blood, Environment, Swachhata, Teaching.",
[M("Which is a social service activity of NCC?",["Blood donation camp","Betting","Politics","Shopping"],0,"Blood donation camps are a common NCC social service."),
M("NCC cadets help mostly during ___.",["Natural disasters","Film shooting","Cricket matches only","Exams"],0,"They assist authorities in floods, earthquakes and other disasters.")],
"Describe the contribution of NCC to social service. (5 marks)",
"NCC cadets do blood donation, tree plantation, cleanliness drives, literacy and awareness work, and disaster relief, showing selfless service to society."),

T("Challenges faced by NCC cadets",
"Har cadet ke saamne kuch problems aati hain: padhai aur NCC ka time clash, kam funds, kam equipment, kam seats aur trainers ki kami. Ghar se support na milna bhi ek problem hai.",
"A cadet has exams but also has a camp in the same week. He finds it hard to manage both.",
"Although NCC is very useful, cadets face many practical challenges in their training and daily life.",
["Time management: balancing studies, classes and NCC training is difficult.","Lack of infrastructure and equipment: shortage of grounds, uniforms and training material in some places.","Shortage of trainers: fewer instructors and officers than required.","Limited seats: demand is high but vacancies are limited.","Low awareness of benefits: many students and parents do not know the incentives.","Safety and health risks: adventure activities and hard training can cause injury.","Rural and girl cadets: distance, transport and social restrictions reduce participation.","Dropouts: loss of interest or career pressure makes some cadets leave."],
"These challenges can be reduced by more funds, better facilities, trained staff, awareness programmes and strong support from families and institutions.",
["Time management","Funds","Infrastructure","Trainers","Limited seats","Awareness","Dropouts"],
"TIFS-AD: Time, Infrastructure, Funds, Staff, Awareness, Dropouts.",
[M("A common challenge for a cadet is ___.",["Balancing studies and training","Too many holidays","Free time","No uniform ever"],0,"Time clash between studies and NCC is the most common challenge."),
M("Which step can reduce dropouts?",["Ignoring cadets","Better motivation and incentives","Removing camps","Stopping parades"],1,"Motivation, awareness and incentives keep cadets interested.")],
"List the main challenges faced by NCC cadets. (5 marks)",
"Time management, lack of infrastructure and equipment, shortage of trainers, limited seats, low awareness, safety risks and dropouts."),

T("Aims and objectives of NCC",
"NCC ke aim simple hain: youth mein character, discipline aur seva ki bhavna lana, trained youth ki ek force banana, aur armed forces mein jaane ke liye motivate karna. NCC ki sthapna 1948 mein hui thi aur ye Ministry of Defence ke under aati hai.",
"A school student joins NCC, learns discipline and later decides to join the Army. This fulfils the aims of NCC.",
"The National Cadet Corps was formed in 1948 under the NCC Act. It is the youth wing of the Indian Armed Forces. Its motto is 'Unity and Discipline'.",
["Develop character: build character, comradeship, discipline, secular outlook, spirit of adventure and ideals of selfless service among youth.","Create human resource: build a pool of organised, trained and motivated youth who can lead in all walks of life, including the armed forces.","Armed forces motivation: provide a suitable environment to motivate youth to take up a career in the armed forces.","Objective - Discipline: make cadets disciplined citizens.","Objective - Leadership: develop leadership and team spirit.","Objective - Service: promote social service and national integration."],
"Thus NCC prepares young people to become good citizens, leaders and, if they wish, officers of the armed forces.",
["1948","Ministry of Defence","Unity and Discipline","Character","Comradeship","Secular outlook","Selfless service","Armed forces career"],
"CCS-A: Character, Comradeship, Secularism, Adventure/Service.",
[M("NCC was established in the year ___.",["1942","1948","1950","1962"],1,"NCC came into existence in 1948 under the NCC Act."),
M("NCC works under which ministry?",["Ministry of Education","Ministry of Home Affairs","Ministry of Defence","Ministry of Sports"],2,"NCC is a tri-service organisation under the Ministry of Defence.")],
"Write the aims of NCC. (5 marks)",
"To develop character, comradeship, discipline, secular outlook, adventure and selfless service; to create organised, trained, motivated youth for leadership; and to motivate youth to join armed forces."),

T("Organization and structure of NCC",
"NCC ka structure upar se neeche aisa chalta hai: Headquarters (Delhi) mein Director General, phir State Directorates, phir Groups, phir Units. Teen wings hote hain: Army, Navy, Air Force. Aur do divisions: Senior (college) aur Junior (school).",
"Think of a school: Principal at top, then department heads, then class teachers. NCC works the same way - DG at top and Unit Commanding Officers close to cadets.",
"NCC is a tri-service organisation with Army, Navy and Air Force wings. It is organised in a hierarchy from national level to unit level.",
["National level: NCC Headquarters at New Delhi, headed by the Director General (a Lieutenant General or equivalent).","State level: State Directorates headed by an Additional Director General (Major General or equivalent), who look after one or more states/UTs.","Group level: Groups headed by Group Commanders (Brigadier or equivalent) control many units.","Unit level: Units/Battalions headed by a Commanding Officer (Colonel or equivalent); they train cadets directly.","Associate NCC Officers (ANO): teachers/lecturers who train cadets in schools and colleges.","Wings: Army Wing, Naval Wing and Air Wing.","Divisions: Senior Division/Wing (boys/girls in colleges) and Junior Division/Wing (boys/girls in schools)."],
"This strong chain of command helps in smooth planning, training and administration of lakhs of cadets across India.",
["HQ New Delhi","Director General","Directorate","Group","Unit","ANO","Army-Navy-Air wings","SD/SW and JD/JW"],
"Order: HQ - Directorate - Group - Unit = 'Hum Do Group Unit' (HQ, Directorate, Group, Unit).",
[M("Head of NCC at the national level is the ___.",["Group Commander","Director General","Commanding Officer","ANO"],1,"The Director General heads NCC at NCC HQ, New Delhi."),
M("NCC wings are:",["Army, Navy, Air Force","Army, Police, Navy","Navy, Coast, Police","Army, Air, Railways"],0,"NCC has three wings: Army, Navy and Air Force.")],
"Explain the organisation of NCC at national, state and unit level. (5 marks)",
"At national level DG at HQ Delhi; at state level Directorates under an ADG; then Groups under Group Commanders; and Units under Commanding Officers, with ANOs training cadets."),

T("Incentives offered to NCC cadets",
"NCC join karne ke fayde bahut hain. Certificate milta hai (A, B, C), armed forces mein selection mein advantage milta hai, kuch jagah naukri aur college admission mein preference ya bonus marks milte hain. Camps mein free uniform, khana aur adventure ke chances bhi milte hain.",
"A cadet with a C certificate gets direct SSB interview chance in some entries of the armed forces without a written exam, so his path becomes easier.",
"The government and institutions give many benefits to NCC cadets to encourage youth to join. Some benefits may differ from state to state and university to university.",
["NCC Certificates (A, B, C): proof of training, valuable for jobs and admissions.","Armed forces benefits: special entry and relaxation for C certificate holders (like direct SSB interview and reserved vacancies in officer academies).","Preference in jobs: weightage in police, paramilitary and some government recruitments (varies by state).","Education benefits: bonus marks, extra credits or preference in admission in some institutions.","Camps and training: free uniform, food, boarding and allowances in camps.","Adventure and exposure: trekking, sailing, Republic Day Camp and Youth Exchange Programme.","Awards and scholarships: medals, best cadet awards and recognition."],
"These incentives encourage cadets to take NCC seriously and help them in building a bright career.",
["Certificates A B C","SSB advantage","Reserved vacancies","Bonus marks","Camp allowances","Youth exchange","Awards"],
"'ABC-SBA': ABC certificates, SSB, Bonus marks, Awards.",
[M("Which certificate gives the best advantage for armed forces entry?",["A","B","C","None"],2,"The C certificate gives special benefits like direct SSB entry in some schemes."),
M("In camps, cadets generally receive ___.",["Free uniform and food","Nothing","Only homework","Fees to pay"],0,"Cadets receive uniform, boarding and food, and may get allowances.")],
"Write any five incentives offered to NCC cadets. (3 marks)",
"Certificates, preference in armed forces entry, preference in jobs, bonus marks in education, free camps with allowances, and adventure and exchange programmes."),

T("Duties and responsibilities of NCC cadets",
"Cadet ki kuch duties hoti hain: regular parade aur training attend karna, discipline maanna, uniform sahi pehenna, camp mein hissa lena, seniors ki respect karna aur samaj ki seva karna. NCC ka cadet sabke liye role model hota hai.",
"A cadet picks up litter near the college gate in uniform. Others see him and also start keeping the place clean.",
"A cadet is a disciplined youth representing NCC. Therefore he or she must follow certain duties towards NCC, society and the nation.",
["Attend parades and classes regularly: be punctual and sincere.","Obey orders and rules: follow commands of officers and instructors.","Wear proper uniform: keep dress and equipment clean.","Take part in camps and activities: join training, sports and cultural programmes.","Social service: help the community and protect the environment.","Respect and courtesy: respect seniors, flag, national anthem and fellow cadets.","Good character and honesty: avoid bad habits and set an example.","Protect property: take care of NCC equipment and public property."],
"A cadet who follows these duties makes NCC proud and becomes a responsible citizen of India.",
["Punctuality","Obedience","Uniform","Camp participation","Social service","Respect","Role model"],
"DUTY = Discipline, Uniform, Training, You as role model.",
[M("A cadet should always ___.",["Obey lawful orders","Skip parades","Break rules","Ignore uniform"],0,"Obeying orders and rules is the first duty of a cadet."),
M("Which of these is a duty of a cadet?",["Regular attendance in training","Bullying juniors","Missing camps","Wearing any dress"],0,"Regular and sincere attendance is a basic duty.")],
"State the duties of NCC cadets. (3-5 marks)",
"Attend parades regularly, obey orders, wear proper uniform, join camps, serve society, respect seniors and flag, keep good character and protect equipment."),

T("Types of NCC camps and their conduct",
"NCC mein alag alag camps hote hain: Annual Training Camp (ATC), Combined Annual Training Camp (CATC), National Integration Camp (NIC), Thal Sainik Camp, Vayu Sainik Camp, Nau Sainik Camp, Republic Day Camp (RDC), Army Attachment, Adventure camps. Camp mein subah PT, din mein drill aur classes, shaam ko games aur raat ko lights-out hota hai.",
"Cadets in an Annual Training Camp wake up early, do PT, attend drill and weapon training classes, play games, perform a cultural evening and sleep on time.",
"NCC conducts different camps every year to give practical training, adventure and exposure to cadets. These camps are the heart of NCC training.",
["Annual Training Camp (ATC): yearly camp for units, usually about 10 days, for basic training.","Combined Annual Training Camp (CATC): several units/groups train together at a bigger level.","National Integration Camp (NIC): cadets from different states meet to promote unity.","Thal Sainik Camp (Army), Vayu Sainik Camp (Air) and Nau Sainik Camp (Navy): national level competition camps for the best cadets.","Republic Day Camp (RDC): selected cadets from all India camp in Delhi in January and march in the Republic Day parade.","Attachment and adventure camps: Army Attachment, trekking, rock climbing, sailing and para-sailing.","Conduct of a camp: reveille and PT, drill and classes, games, cultural programmes, medical care, strict discipline, a Camp Commandant, and lights-out.","Evaluation: cadets are assessed and best performers get awards."],
"Camps give hands-on training, improve discipline and teamwork, and bring cadets of all backgrounds together.",
["ATC","CATC","NIC","Thal Sainik","Vayu Sainik","Nau Sainik","Republic Day Camp","Camp Commandant"],
"'ACN-TVN-R': ATC, CATC, NIC - Thal, Vayu, Nau - Republic Day.",
[M("Which camp is held in Delhi in January for the Republic Day parade?",["ATC","Republic Day Camp","Trekking Camp","CATC"],1,"Selected cadets attend the RDC in Delhi to take part in the Republic Day celebrations."),
M("Vayu Sainik Camp is related to which wing?",["Army","Navy","Air","Police"],2,"Vayu means air; it is for the Air Wing. (Thal = Army, Nau = Navy).")],
"Name and explain different types of NCC camps. (5 marks)",
"ATC, CATC, NIC, Thal/Vayu/Nau Sainik Camps, Republic Day Camp and adventure/attachment camps; each gives training, discipline and national-level exposure.")
]},

{n:"Unit II",name:"National Integration",min:75,topics:[
T("Social, religious and regional divisions and their solutions",
"India mein jaati, dharm, bhasha aur region ke naam par kabhi kabhi jhagde hote hain. Isse desh kamzor hota hai. Solution: acchi education, barabar kanoon, sabka vikas aur ek dusre ki respect.",
"Two villages fight over language. A teacher organises a joint cultural fair where both perform. Friendship starts.",
"India is a land of many castes, religions, languages and regions. When these differences turn into conflict, they become divisions that threaten unity.",
["Social divisions: caste discrimination, untouchability and gender inequality.","Religious divisions: communal tension, mistrust and hate speech.","Regional divisions: demands for separate states, river and border disputes, and regional imbalance.","Solution - Education: teaches tolerance and equality.","Solution - Secularism and law: equal rights for all as per the Constitution.","Solution - Balanced development: develop backward regions.","Solution - Dialogue and cultural exchange: festivals, sports and youth programmes."],
"Respect for diversity, equal opportunity and strict action against hate can end divisions and strengthen India.",
["Caste","Communalism","Regionalism","Tolerance","Secularism","Equality","Dialogue"],
"SEED = Secularism, Education, Equality, Dialogue.",
[M("A main solution to communal divisions is ___.",["Tolerance and dialogue","Hate speech","Violence","Isolation"],0,"Tolerance and dialogue reduce mistrust between communities."),
M("Regional imbalance means ___.",["Equal growth in all areas","Unequal development between regions","No states","One language"],1,"Some regions develop faster than others, causing unrest.")],
"What are social, religious and regional divisions? Suggest solutions. (5 marks)",
"Divisions are differences turning into conflict on caste, religion or region. Solutions are education, secularism, equal laws, balanced development and dialogue."),

T("Threats to national security",
"National security ka matlab desh ko andar aur bahar ke khatron se bachana. Khatre hain: terrorism, border dispute, insurgency, cyber attack, drugs, fake news aur communal hinsa.",
"A hacker group attacks a bank's computers. This is a cyber threat to national security.",
"National security means protecting the country's sovereignty, people, economy and values from threats, both external and internal.",
["Terrorism: violent attacks to spread fear.","Insurgency and Naxalism: armed groups fighting the state.","Border disputes and wars: threats from neighbours.","Cyber attacks: hacking of defence, banks and power grids.","Communalism and extremism: break social harmony.","Drug and arms trafficking: weaken youth and fund crime.","Illegal migration and organised crime.","Fake news and propaganda: create panic and hatred.","Economic threats: counterfeit currency, economic sabotage."],
"A strong military, alert citizens and unity of people are needed to face these threats.",
["Terrorism","Insurgency","Cyber attack","Border dispute","Communalism","Trafficking","Fake news"],
"'TIC-CBD': Terrorism, Insurgency, Cyber, Communalism, Border, Drugs.",
[M("Which is a cyber threat?",["Hacking of government websites","Heavy rain","Festival","Sports day"],0,"Hacking is a cyber threat to national security."),
M("Naxalism is a type of ___.",["Internal security threat","Sports event","Weather problem","Trade policy"],0,"Naxalism is an internal armed movement.")],
"Explain the major threats to India's national security. (5 marks)",
"Terrorism, insurgency, border disputes, cyber attacks, communalism, trafficking and fake news threaten India's security."),

T("Leadership and national integration",
"Achha leader logon ko jodta hai. Sardar Patel ne 500 se zyada princely states ko India mein milaya. Aaj bhi leaders ko hate nahi, unity ki baat karni chahiye.",
"A class monitor keeps students of all religions together by planning common events. This is leadership for integration.",
"Leadership plays a key role in uniting people. Good leaders inspire trust, and bad leadership can divide society.",
["Setting an example: leaders who respect all communities guide the people.","Historical leaders: Sardar Patel integrated princely states; Gandhi united people in the freedom struggle.","Political leadership: fair policies for all groups.","Social and religious leaders: promote peace and harmony.","Youth leaders: students and cadets can spread unity.","Avoiding hate speech: leaders should not use religion or caste for votes.","Crisis leadership: calm leadership during riots and disasters protects unity."],
"Honest, inclusive and visionary leadership is the key to strong national integration.",
["Sardar Patel","Inclusive leader","Trust","Role model","Harmony","Youth leaders","No hate speech"],
"'PEACE' leaders: Patel, Example, All-inclusive, Calm, Equality.",
[M("Who integrated the princely states of India?",["Sardar Vallabhbhai Patel","Subhas Chandra Bose","Bhagat Singh","Lala Lajpat Rai"],0,"Sardar Patel, as Deputy PM and Home Minister, integrated over 500 princely states."),
M("A good leader for integration should be ___.",["Inclusive","Selfish","Hateful","Divisive"],0,"An inclusive leader treats all groups equally.")],
"Discuss the role of leadership in national integration. (5 marks)",
"Leaders unite people by setting examples, making fair policies and avoiding hate. Patel's integration of states is a strong example."),

T("Media and communication in promoting integration",
"Media matlab newspaper, TV, radio aur social media. Ye logon tak news, culture aur unity ke message pahunchate hain. Lekin fake news se nuksan bhi ho sakta hai, isliye media ko responsible hona chahiye.",
"A TV show shows festivals of all states. A child in Gujarat learns about Pongal and feels connected.",
"Media and communication are powerful tools that shape public opinion. Used well, they bring people closer.",
["Spreading awareness: news on national issues and rights.","Cultural exchange: programmes on festivals, food and languages of all states.","Promoting unity messages: campaigns like 'Mile Sur Mera Tumhara' type songs and national programmes.","Regional language content: connects people in their own language.","Social media: quick sharing of positive stories and youth campaigns.","Role in crisis: spreads correct information during disasters and riots.","Negative role: fake news and hate speech can increase tension, so ethical media and fact-checking are needed."],
"Responsible and honest media can strengthen unity, while irresponsible media can weaken it.",
["Mass media","Cultural exchange","Awareness","Regional language","Social media","Fake news","Fact-checking"],
"'MAC-FRS': Media, Awareness, Culture, Fact-check, Responsible, Social.",
[M("Which is a negative role of media?",["Fake news","Awareness","Education","Culture"],0,"Fake news can spread panic and hatred."),
M("Regional language programmes help to ___.",["Connect people of different regions","Increase hatred","Reduce education","Close channels"],0,"They help people understand each other's culture.")],
"How can media and communication help in national integration? (5 marks)",
"Through awareness, cultural exchange, regional content, social media campaigns and truthful reporting, media can promote unity."),

T("Steps to prevent terrorism, insurgency and communalism",
"Terrorism, insurgency aur communalism rokne ke liye sarkar aur janta dono ko kaam karna padta hai. Strong intelligence, border security, development, education aur community ka bharosa zaroori hai.",
"Villagers inform police about a suspicious bag. A big attack is prevented.",
"Terrorism, insurgency and communalism harm peace and development. They can be controlled by firm action and social efforts.",
["Strong intelligence and policing: early information and quick action.","Border security: fencing, patrolling and technology.","Strict laws: fast trials for terror and hate crimes.","Development of affected areas: roads, jobs and schools reduce anger.","Education and awareness: teach tolerance and fight false propaganda.","Community policing and citizen vigilance: people report suspicious activity.","De-radicalisation and rehabilitation: bring misled youth back to normal life.","Control of hate content online and promoting inter-faith dialogue."],
"A joint effort of government, security forces, media and citizens is needed to defeat these evils.",
["Intelligence","Border security","Strict laws","Development","Awareness","Community policing","Rehabilitation"],
"'I-BLADE-CR': Intelligence, Border, Law, Awareness, Development, Education, Community, Rehabilitation.",
[M("Which step helps prevent insurgency in backward areas?",["Development and jobs","Ignoring them","More hate","Closing schools"],0,"Development reduces anger and support for insurgents."),
M("Citizen vigilance means ___.",["Reporting suspicious activity","Spreading rumours","Ignoring danger","Hiding facts"],0,"Alert citizens help police stop crimes.")],
"What steps can be taken to prevent terrorism, insurgency and communalism? (5 marks)",
"Strong intelligence, border security, strict laws, development, education, community policing and rehabilitation."),

T("India's national security challenges",
"India ki borders badi hain aur padosi desh kabhi kabhi problem karte hain. Andar bhi terrorism, Naxalism aur North-East mein insurgency hai. Cyber, maritime aur climate ke challenges bhi hain.",
"A ship is stopped in the Indian Ocean for suspected smuggling. This shows the maritime security challenge.",
"India faces both traditional (military) and non-traditional challenges to its national security.",
["Border disputes: tensions with Pakistan and China.","Terrorism: cross-border and homegrown.","Internal conflicts: Naxal areas, insurgency in the North-East and Jammu and Kashmir.","Maritime security: long coastline and Indian Ocean safety.","Cyber security: attacks on defence and critical systems.","Energy and economic security: dependence on imported fuel.","Climate and disasters: floods and cyclones affect security.","Nuclear and space security."],
"India handles these challenges through a strong armed force, diplomacy, technology and people's unity.",
["Border disputes","Cross-border terrorism","Naxalism","Maritime security","Cyber security","Energy security","Disasters"],
"'BTN-MCE': Border, Terrorism, Naxal, Maritime, Cyber, Energy.",
[M("Which is a non-traditional security challenge?",["Cyber attack","Tank war","Border war","Fort siege"],0,"Cyber attacks come under non-traditional threats."),
M("Long coastline creates which challenge?",["Maritime security","Desert storms","Less trade","No threat"],0,"A long coast needs strong maritime security.")],
"Discuss India's national security challenges. (5 marks)",
"Border disputes, terrorism, internal insurgency, maritime and cyber threats, and energy and climate issues challenge India's security."),

T("Meaning, importance and necessity of national integration",
"National integration ka matlab hai desh ke sabhi logon mein ekta ki bhavna. Iske bina desh toot sakta hai. Isliye har citizen ke liye ye zaroori hai.",
"In a cricket match everyone supports India, forgetting caste and religion. That feeling is integration.",
"National integration is the feeling of oneness among people of different groups, so that they think of themselves first as Indians.",
["Meaning: unity in spite of differences of caste, religion, language and region.","Peace and harmony: reduces riots and conflict.","National strength: a united nation resists enemies.","Economic growth: stability attracts investment and development.","Democracy: helps democracy work smoothly.","Cultural richness: preserves and shares all cultures.","Necessity: India has great diversity; without integration there is risk of division."],
"National integration is the base of India's progress, peace and security.",
["Oneness","Unity","Harmony","Peace","Strength","Democracy","Necessity"],
"'UPS-DEN': Unity, Peace, Strength, Democracy, Economy, National pride.",
[M("National integration means ___.",["Feeling of oneness","Racial separation","Language war","Regional hatred"],0,"It means feeling united as one nation."),
M("Why is it necessary for India?",["Because of great diversity","Because of no differences","To increase conflicts","To close borders"],0,"India is diverse, so unity is essential.")],
"Define national integration and explain its importance. (5 marks)",
"National integration is the feeling of unity among all citizens. It is important for peace, strength, economic growth and the success of democracy."),

T("National integration and economic stability",
"Jab desh mein ekta hoti hai to shanti rehti hai, investors aate hain, naukri badhti hai aur economy majboot hoti hai. Aur strong economy se bhi ekta badhti hai. Dono ek dusre ki madad karte hain.",
"A company opens a factory in a peaceful state and gives jobs to people from many regions. They work together and grow together.",
"National integration and economic stability are linked. Unity brings stability, and a stable economy keeps people united.",
["Peaceful environment: attracts industries and investors.","Single national market: free movement of goods and people; GST helps one market.","Less cost of conflict: money is not wasted on riots and security.","Balanced regional development: reduces anger of backward areas.","Employment and mobility: people can work across India.","Strong economy gives resources for education, health and defence.","Two-way relation: economic equality reduces social tension."],
"So integration and economic stability support each other and lead to a developed India.",
["Peace","Investment","Single market","GST","Employment","Balanced development","Stability"],
"'PIE-GBE': Peace, Investment, Employment, GST, Balanced growth.",
[M("Which helps a single national market?",["GST","Riots","Strikes","Curfew"],0,"GST created one common tax system across states."),
M("Unity in a country leads to ___.",["More investment","Less jobs","More conflicts","Weak economy"],0,"Unity gives stability that attracts investors.")],
"How are national integration and economic stability related? (5 marks)",
"Unity creates peace and investment, while balanced economic growth reduces inequality and strengthens unity."),

T("Political, social, economic and cultural factors affecting integration",
"Integration ko kuch cheezein badhati hain aur kuch cheezein rokti hain. Political: vote bank politics. Social: jaati-dharm bhed. Economic: gareebi aur asamanta. Cultural: bhasha ya riti-riwaj ko lekar takraav.",
"A leader asks for votes in the name of caste. Society gets divided - a political factor harming integration.",
"Many factors affect national integration, either by strengthening or weakening it.",
["Political factors: vote-bank politics, regionalism and corruption hurt; fair democracy and federalism help.","Social factors: caste and communal divisions hurt; social equality helps.","Economic factors: poverty, unemployment and regional imbalance create unrest; inclusive growth helps.","Cultural factors: language and religious clashes hurt; respect for all cultures helps.","Role of history: shared freedom struggle unites Indians.","Role of media and education: can either spread hatred or unity.","Solution: balanced policies and awareness in all four areas."],
"Positive factors should be encouraged and negative ones controlled to protect national unity.",
["Vote-bank politics","Social inequality","Poverty","Regionalism","Language conflict","Federalism","Inclusive growth"],
"'PSEC': Political, Social, Economic, Cultural.",
[M("Vote-bank politics is a ___ factor.",["Political","Cultural","Geographical","Biological"],0,"It is a political factor that can divide society."),
M("Poverty and unemployment are ___ factors.",["Economic","Cultural","Religious","Political"],0,"They are economic factors affecting integration.")],
"Explain political, social, economic and cultural factors affecting national integration. (5 marks)",
"Political (vote banks), social (caste), economic (poverty, imbalance) and cultural (language clashes) factors can weaken integration; fairness and inclusion strengthen it."),

T("Role of education and educational policies",
"Education se soch badalti hai. School mein sab bachche saath padhte hain to unity aati hai. Sarkar ki policies jaise NEP 2020 mein multilingualism, Indian culture aur values par zor diya gaya hai.",
"A school teaches all festivals and languages in assemblies. Children become friendly and respectful.",
"Education shapes attitudes and values. It is a strong tool for building national integration.",
["Values and tolerance: moral education teaches equality and respect.","Common schooling: students of all backgrounds study together.","Three-language formula: promotes understanding between languages (recommended by Kothari Commission and National Policy of Education).","National Education Policy (NEP) 2020: promotes multilingualism, Indian knowledge, and holistic education.","Right to Education (RTE) 2009: free and compulsory education for children aged 6-14, includes all groups.","Programmes like NCC, NSS and Ek Bharat Shreshtha Bharat: connect students of different states.","History and civics: teach the freedom struggle and the Constitution."],
"Thus education and good policies create responsible and united citizens.",
["Moral education","Three-language formula","NEP 2020","RTE 2009","Multilingualism","NCC/NSS","Ek Bharat Shreshtha Bharat"],
"'MRN-TE': Moral values, RTE, NEP, Three-language, Exchange programmes.",
[M("RTE Act 2009 gives free and compulsory education to children of age ___.",["3-5","6-14","15-18","18-21"],1,"RTE guarantees free and compulsory education for ages 6-14."),
M("Which policy promotes multilingualism in India?",["NEP 2020","Vote policy","GST","Arms policy"],0,"NEP 2020 supports multilingual education.")],
"Describe the role of education and educational policies in promoting national integration. (5 marks)",
"Education teaches tolerance and equality; policies like three-language formula, RTE and NEP 2020 and programmes like NCC and NSS bring students together."),

T("Unity in diversity in India's language, religion, culture and geography",
"India ek aisa desh hai jahan alag alag bhasha, dharm, khaan-paan aur geography hai, phir bhi sab ek hain. Isi ko 'Unity in Diversity' kehte hain.",
"On Republic Day, floats of all states with different dresses and dances move together in one parade.",
"Unity in diversity means that in spite of many differences, Indians are bound together as one nation.",
["Language: 22 scheduled languages and hundreds of dialects; Hindi and English are used for official work.","Religion: Hinduism, Islam, Christianity, Sikhism, Buddhism, Jainism and others live together; India is a secular country.","Culture: different food, dress, music, dance and festivals, with many common celebrations like Diwali, Eid, Christmas.","Geography: Himalayas, plains, deserts, coasts, islands, with varied climate.","Common bonds: one Constitution, one citizenship, one flag and one national anthem.","Shared history: freedom struggle and common heritage.","Unity: cricket, army, Republic Day and festivals unite all."],
"India's diversity is its strength and beauty, and it must be protected through tolerance and unity.",
["22 languages","Secular","Festivals","Geography","One Constitution","Common citizenship","Unity in diversity"],
"'LRCG': Language, Religion, Culture, Geography.",
[M("How many languages are in the Eighth Schedule of the Constitution?",["14","18","22","30"],2,"There are 22 scheduled languages."),
M("India is described as a land of ___.",["Unity in diversity","One language only","One religion only","No culture"],0,"It has many differences but remains united.")],
"Explain 'Unity in Diversity' with reference to India. (5 marks)",
"India has many languages, religions, cultures and geographies, but one Constitution, flag and citizenship bind all Indians together.")
]},

{n:"Unit III",name:"Personality Development",min:75,topics:[
T("Decision-making and problem-solving",
"Decision lena matlab kai options mein se sabse sahi option chunna. Problem solve karne ke liye steps follow karo: problem samjho, options likho, faayde-nuksan dekho, decide karo aur result check karo.",
"You must choose between studying at night or in the morning. You test both for a week and pick the one in which you remember more.",
"Decision-making is the process of choosing the best option from many choices. Problem-solving is finding a solution to a difficulty. Both are important life skills.",
["Define the problem clearly.","Collect information and facts.","List possible options.","Evaluate pros and cons of each.","Choose the best option.","Implement the decision with a plan.","Review the result and learn from it.","Tips: stay calm, take advice, and avoid decisions in anger."],
"Good decisions and problem-solving give success in studies, career and life, and are very important for a leader and cadet.",
["Define problem","Collect facts","Options","Pros and cons","Choose","Implement","Review"],
"'DECIDE': Define, Explore, Choose, Implement, Do review, Evaluate.",
[M("What is the first step of problem-solving?",["Define the problem","Take decision","Blame others","Ignore it"],0,"First understand the problem."),
M("After taking a decision we should ___.",["Review the result","Forget it","Hide it","Blame others"],0,"Review and learn from the result.")],
"Explain the steps of decision-making. (5 marks)",
"Define the problem, collect information, list options, evaluate, choose, implement and review the result."),

T("Self-confidence and personality development",
"Self-confidence ka matlab apne aap par bharosa. Personality ka matlab aapke habits, soch aur behaviour ka total. Positive soch, practice aur chhoti jeet se confidence badhta hai.",
"A shy student prepares well and gives a speech. People clap. Next time he feels more confident.",
"Personality is the sum of a person's thoughts, feelings, habits and behaviour. Self-confidence is belief in one's own abilities. Both help in success.",
["Meaning of personality: the unique pattern of a person's behaviour and character.","Meaning of confidence: trust in one's own ability.","Positive thinking and self-talk: encourage yourself.","Preparation and practice: skill removes fear.","Set small goals and celebrate small wins.","Good communication and body language: eye contact, posture and voice.","Learning from failures: failure is a lesson, not the end.","Healthy lifestyle and neat appearance."],
"A confident and balanced personality helps a person face challenges and succeed in life.",
["Personality","Self-confidence","Positive thinking","Practice","Small goals","Body language","Learning from failure"],
"'CAPS': Confidence, Attitude, Practice, Skills.",
[M("Self-confidence means ___.",["Trust in own ability","Fear of others","Laziness","Anger"],0,"It is belief in oneself."),
M("Which habit builds confidence?",["Regular practice","Avoiding everything","Negative talk","Comparing always"],0,"Practice and preparation reduce fear.")],
"How can self-confidence be developed? (5 marks)",
"By positive thinking, preparation, small goals, good communication, learning from failures and a healthy lifestyle."),

T("Emotional Intelligence (EQ) and its components",
"EQ ka matlab apni aur dusron ki emotions ko samajhna aur sambhalna. Daniel Goleman ke hisaab se EQ ke 5 parts hain: self-awareness, self-regulation, motivation, empathy aur social skills.",
"A cadet gets scolded but stays calm, listens and improves. This shows high EQ.",
"Emotional Intelligence is the ability to understand, control and use emotions positively, and to understand others' emotions. It was popularised by Daniel Goleman.",
["Self-awareness: knowing your own feelings and strengths.","Self-regulation: controlling anger and impulses.","Motivation: inner drive to achieve goals.","Empathy: understanding others' feelings.","Social skills: good communication, teamwork and conflict handling.","Importance: better relationships, leadership and less stress.","Development: reflection, listening and managing stress."],
"High EQ helps in success in studies, jobs and relationships, sometimes even more than IQ.",
["EQ","Daniel Goleman","Self-awareness","Self-regulation","Motivation","Empathy","Social skills"],
"'ARMES': Awareness, Regulation, Motivation, Empathy, Social skills.",
[M("How many components of EQ are given by Goleman?",["3","4","5","7"],2,"Goleman gave five components."),
M("Controlling anger is part of ___.",["Self-regulation","Empathy","Motivation","Intelligence quotient"],0,"Self-regulation means controlling emotions and impulses.")],
"What is Emotional Intelligence? Explain its components. (5 marks)",
"EQ is the ability to understand and manage emotions; its components are self-awareness, self-regulation, motivation, empathy and social skills."),

T("Goal setting and achievement",
"Goal ka matlab aapka lakshya. Goal clear ho to mehnat sahi direction mein hoti hai. SMART goal banao: Specific, Measurable, Achievable, Relevant, Time-bound.",
"Instead of 'I will study more', say 'I will study 2 hours daily for 30 days to finish my syllabus'. This is SMART.",
"Goal setting means deciding what you want to achieve and planning how to reach it. It gives direction, motivation and success.",
["Specific: clear and exact.","Measurable: you can track progress.","Achievable: realistic.","Relevant: matches your life aim.","Time-bound: has a deadline.","Short-term and long-term goals: small steps lead to big goals.","Action plan and review: write steps and check progress regularly.","Overcome obstacles: stay disciplined and flexible."],
"A person with clear goals and consistent effort is more likely to achieve success.",
["Goal","SMART","Short-term","Long-term","Action plan","Deadline","Review"],
"SMART = Specific, Measurable, Achievable, Relevant, Time-bound.",
[M("What does 'M' in SMART stand for?",["Measurable","Mental","Moral","Major"],0,"M stands for Measurable."),
M("A good goal must have ___.",["A deadline","No plan","No clarity","No steps"],0,"Time-bound means it has a deadline.")],
"Explain SMART goals with an example. (5 marks)",
"SMART goals are Specific, Measurable, Achievable, Relevant and Time-bound; e.g. 'I will study 2 hours daily for 30 days'."),

T("Resilience and coping with setbacks",
"Resilience matlab girkar phir uthna. Zindagi mein fail hona, reject hona ya problem aana normal hai. Jo log seekhkar aage badhte hain, wo resilient hote hain.",
"A student fails a test, studies the mistakes and scores well next time. This is resilience.",
"Resilience is the ability to recover quickly from difficulties. Coping means ways to handle stress and setbacks.",
["Positive thinking: see failure as a lesson.","Problem-focused coping: make a plan to solve the problem.","Emotion-focused coping: talk, relax, exercise or pray to manage feelings.","Social support: share with family, friends or mentors.","Healthy habits: sleep, food and exercise.","Flexibility: change plans when needed.","Seek help: talk to a counsellor if stress is too heavy.","NCC helps through hard training and teamwork."],
"Resilience helps a person stay strong, learn from mistakes and keep moving ahead.",
["Resilience","Setback","Coping","Positive thinking","Support system","Flexibility","Stress management"],
"'BOUNCE': Believe, Organise, Understand, Network, Care, Exercise.",
[M("Resilience means ___.",["Recovering from difficulty","Giving up","Blaming others","Avoiding work"],0,"It is bouncing back after failure."),
M("Which is a healthy coping method?",["Exercise and talking","Anger","Drugs","Isolation"],0,"Exercise and sharing feelings are healthy.")],
"What is resilience? How can one cope with setbacks? (5 marks)",
"Resilience is bouncing back from difficulties; coping includes positive thinking, planning, social support, healthy habits and seeking help."),

T("Hereditary, environmental and social factors in personality",
"Personality teen cheezon se banti hai: heredity (genes jo parents se aate hain), environment (ghar, school, khana-paani) aur society (dost, culture, media).",
"Two brothers have similar height (heredity) but different habits because of different friends (social factor).",
"Personality is shaped by many factors. Mainly, heredity, environment and social factors play a role.",
["Hereditary factors: genes decide physical features, basic temperament and potential like intelligence.","Family environment: parents' behaviour, love and discipline shape habits.","School environment: teachers and peers influence thinking.","Physical environment: climate, nutrition and health.","Social factors: friends, culture, religion and traditions.","Media and technology: influence values and behaviour.","Result: personality is a mix of nature (heredity) and nurture (environment)."],
"Though heredity gives the base, environment and social surroundings help us to develop and change our personality.",
["Heredity","Genes","Environment","Family","School","Society","Nature and nurture"],
"'HES': Heredity, Environment, Society.",
[M("Genes are part of ___.",["Heredity","Environment","Society","Media"],0,"Genes come from parents and form heredity."),
M("Friends and culture are ___ factors.",["Social","Hereditary","Chemical","Physical"],0,"They are social factors.")],
"Explain hereditary, environmental and social factors affecting personality. (5 marks)",
"Heredity gives genes and basic traits, environment (family, school, health) shapes habits, and social factors like peers and culture influence behaviour."),

T("Self-awareness and how to develop it",
"Self-awareness matlab apne aap ko jaanna: meri strengths, weaknesses, values aur emotions kya hain. Jab hum khud ko jaante hain to sahi decision aur improvement aasan hota hai.",
"A student notices he gets nervous in speeches. He practises daily and improves. He became aware and worked on it.",
"Self-awareness is the ability to know and understand your own feelings, thoughts, strengths, weaknesses and values.",
["Know strengths and weaknesses: make a SWOT list of yourself.","Reflect daily: write a diary or journal.","Ask for feedback: from teachers, friends and seniors.","Observe your emotions and reactions.","Practise mindfulness or meditation.","Understand your values and goals.","Take personality or interest tests.","Accept and improve: work on weak areas."],
"Self-awareness is the first step to personal growth and success.",
["Self-awareness","Strengths","Weaknesses","SWOT","Journal","Feedback","Mindfulness"],
"'SAFE-JM': SWOT, Ask feedback, Journal, Meditate.",
[M("Self-awareness means ___.",["Knowing oneself","Knowing others only","Ignoring feelings","Copying others"],0,"It is understanding your own traits and feelings."),
M("Which helps develop self-awareness?",["Journal writing","Ignoring feedback","Blaming others","Avoiding thinking"],0,"Writing a journal helps reflection.")],
"What is self-awareness? How can it be developed? (5 marks)",
"It is knowing one's strengths, weaknesses and emotions; develop it through reflection, feedback, journal, meditation and SWOT."),

T("Empathy and relationships",
"Empathy matlab doosre ke jagah par khud ko rakhkar unki feelings samajhna. Isse dosti, family aur team ke rishte achhe hote hain.",
"A friend is sad about his results. You listen, do not judge and say 'I understand'. He feels better.",
"Empathy is the ability to understand and share the feelings of others. It is the base of healthy relationships.",
["Active listening: listen fully without interrupting.","No judgement: accept others as they are.","Respect and kindness: treat everyone equally.","Clear communication: express feelings politely.","Trust and honesty: key for strong bonds.","Conflict handling: understand the other side before reacting.","Types: cognitive (understanding), emotional (feeling) and compassionate (acting to help).","Benefits: better teamwork, friendship and leadership."],
"Empathy builds trust, reduces conflict and makes relationships strong and meaningful.",
["Empathy","Active listening","Respect","Trust","Communication","Compassion","Teamwork"],
"'LRC': Listen, Respect, Care.",
[M("Empathy means ___.",["Understanding others' feelings","Ignoring others","Mocking others","Being selfish"],0,"Empathy is putting yourself in someone else's shoes."),
M("Which skill is most important for empathy?",["Active listening","Interrupting","Shouting","Judging"],0,"Listening carefully shows care.")],
"Explain empathy and its role in relationships. (5 marks)",
"Empathy is understanding others' feelings; with listening, respect and trust it improves relationships and teamwork."),

T("Critical thinking and problem-solving",
"Critical thinking matlab kisi baat ko aankh band karke na maanna, balki sawal puchna, proof dekhna aur soch samajh kar nirnay lena. Isse fake news aur galat decisions se bachte hain.",
"You get a WhatsApp message about a free offer. You check the source and find it fake. That is critical thinking.",
"Critical thinking is the ability to analyse information logically, question assumptions and make reasoned judgements. It is a key part of problem-solving.",
["Ask questions: who, what, why, how?","Check the source and evidence before believing.","Analyse facts and separate them from opinions.","Avoid bias: keep an open mind.","Use logical reasoning to compare options.","Consider different viewpoints.","Draw conclusions and test them.","Benefits: smart decisions and protection from fake news."],
"Critical thinkers solve problems better and become wise and independent citizens.",
["Analysis","Evidence","Logic","Bias","Source checking","Questioning","Judgement"],
"'QUEST': Question, Understand, Evidence, Sort facts, Test.",
[M("Critical thinking involves ___.",["Questioning and analysing","Blind belief","Copying","Fear"],0,"It means questioning and analysing information."),
M("What should you check before believing news?",["The source","Only the headline","Number of shares","Colour of page"],0,"Always check the source and evidence.")],
"What is critical thinking? Why is it important? (5 marks)",
"Critical thinking is logical analysis of information; it helps in good decisions, solving problems and avoiding fake news."),

T("Creative thinking and how to foster creativity",
"Creative thinking matlab naye idea sochna. Har problem ke multiple solutions ho sakte hain. Curiosity, practice, brainstorming aur galtiyan karne ka dar na rakhne se creativity badhti hai.",
"In a college camp, cadets use waste bottles to make dustbins. This new idea is creativity.",
"Creative thinking is the ability to think of new, original and useful ideas. It is important for solving problems in new ways.",
["Be curious: ask 'what if' questions.","Brainstorming: write many ideas without judging.","Mind maps: connect ideas visually.","Open mind: accept different views.","Allow mistakes: failure leads to learning.","Try new hobbies: art, music, reading, travel.","Teamwork: different people give different ideas.","Rest and relaxation: fresh mind gives fresh ideas."],
"Creativity can be developed by anyone through practice and a supportive environment.",
["Creative thinking","Curiosity","Brainstorming","Mind map","Original idea","Open mind","Hobbies"],
"'CURIOUS': Curiosity, Unique ideas, Risk-taking, Imagination, Open mind, Unlimited tries, Share.",
[M("Brainstorming means ___.",["Generating many ideas freely","Judging ideas","Copying","Sleeping"],0,"Brainstorming is free flow of many ideas."),
M("Which supports creativity?",["Curiosity","Fear of mistakes","Strict copying","Closed mind"],0,"Curiosity encourages new thinking.")],
"What is creative thinking? How can creativity be fostered? (5 marks)",
"Creative thinking is generating new useful ideas; foster it by curiosity, brainstorming, open mind, hobbies and accepting mistakes.")
]},

{n:"Unit IV",name:"Social Service and Community Development",min:75,topics:[
T("Public-private partnerships involving NGOs, government and private entities",
"PPP matlab sarkar, private companies aur NGOs milkar kaam karte hain. Sarkar policy aur paisa deti hai, company paisa aur technology, NGO ground par kaam karta hai. Companies ka CSR bhi isi mein aata hai.",
"A company funds a school building (CSR), the government gives land and teachers, and an NGO runs the extra classes.",
"A partnership is when government, NGOs and private companies work together for public welfare, sharing resources and responsibility.",
["Government: makes policy, gives land, funds and legal support.","Private sector: gives money (CSR), technology and management skills.","NGOs: know local needs, reach people and run programmes.","CSR: under the Companies Act, 2013, big companies must spend part of profit (2%) on social work.","Examples: sanitation, health camps, school meals, skill training.","Benefits: more resources, better efficiency and wider reach.","Challenges: lack of coordination, accountability and profit motives."],
"If properly managed, such partnerships can speed up community development and reach more people.",
["PPP","NGO","CSR","Companies Act 2013","2% of profit","Coordination","Resources"],
"'GPN': Government, Private, NGO - all three together.",
[M("CSR stands for ___.",["Corporate Social Responsibility","Central Social Rule","Community Service Report","Corporate Sales Rule"],0,"CSR is Corporate Social Responsibility."),
M("Who knows local needs best?",["NGOs","Foreign banks","Stock markets","Film industry"],0,"NGOs work on the ground and know local problems.")],
"Explain public-private partnership in social development. (5 marks)",
"Government, private companies and NGOs share resources and roles; CSR funds help projects, and NGOs execute them locally."),

T("Role of youth in social service and community development",
"Youth ke paas energy, naye idea aur technology ki knowledge hoti hai. India mein youth bahut zyada hain, to wo samaj badalne mein badi bhoomika nibha sakte hain.",
"College students teach poor children in the evening for free. Many children improve in studies.",
"Youth are the future builders of the nation. Their energy and ideas can solve social problems.",
["Volunteering: NCC, NSS and clubs offer chances for service.","Awareness campaigns: cleanliness, health, voting and road safety.","Education support: teach underprivileged children.","Technology use: digital literacy and social media campaigns.","Environmental protection: plantation and waste management.","Entrepreneurship: start-ups that solve social problems.","Leadership: lead community groups.","Disaster response: first aid and relief."],
"When youth work with honesty and dedication, communities progress and the nation develops.",
["Youth power","Volunteering","NCC/NSS","Awareness","Digital literacy","Social entrepreneurship","Leadership"],
"'YOUTH': Energy, Ideas, Technology, Service, Leadership (Y-O-U-T-H = You Offer Useful Time and Help).",
[M("Which organisations promote youth volunteering?",["NCC and NSS","Stock exchanges","Film studios","Banks"],0,"NCC and NSS promote volunteering."),
M("Youth can contribute by ___.",["Teaching poor children","Wasting time","Spreading rumours","Ignoring society"],0,"Teaching and awareness are valuable services.")],
"Discuss the role of youth in community development. (5 marks)",
"Youth volunteer, spread awareness, teach, use technology, protect the environment and lead community projects."),

T("Youth-led initiatives in mental health, environmental protection and education",
"Aaj youth khud bhi kaam kar rahe hain: mental health par baat karna, ped lagana, plastic kam karna aur gareeb bachchon ko padhana.",
"A group of students starts a peer-support club in college so that stressed students can talk freely.",
"Many young people lead initiatives to solve problems in their communities, especially in mental health, environment and education.",
["Mental health: peer support groups, awareness talks, stress-free campus drives, and helping students reach counsellors.","Environmental protection: tree plantation, beach and river clean-up, plastic-free campaigns, recycling and saving water and energy.","Education: free tuition, digital literacy classes, community libraries and 'each one teach one' drives.","Use of social media: spread messages quickly.","Partnership: work with NGOs, schools and local government.","Impact: awareness, reduced stigma, cleaner surroundings and more literacy.","Challenges: funds, time and need for training."],
"Such youth-led initiatives show that small efforts can create big social change.",
["Peer support","Reduce stigma","Tree plantation","Plastic-free","Clean-up drive","Free tuition","Digital literacy"],
"'MEE': Mind, Earth, Education.",
[M("A youth-led mental health initiative is ___.",["Peer support group","Cutting trees","Burning waste","Ignoring stress"],0,"Peer support groups help students share problems."),
M("Plastic-free drive belongs to ___.",["Environmental protection","Cooking","Sports","Banking"],0,"It reduces plastic pollution.")],
"Give examples of youth-led initiatives in mental health, environment and education. (5 marks)",
"Peer support groups for mental health, tree plantation and plastic-free drives for the environment, and free tuition and digital literacy classes for education."),

T("Design a rural community social service project",
"Ek project design karne ke liye steps follow karo: pehle gaon ki zarurat pata karo, goal banao, plan likho, team aur budget tay karo, kaam karo, monitor karo aur result dekho. Maan lo project hai 'Clean and Literate Village'.",
"Project: 'Swachh and Saakshar Gaon' - cleanliness drive plus adult literacy classes in a village for 3 months.",
"A social service project is a planned set of activities to solve a community problem. A good project has clear steps.",
["1. Need assessment: survey with villagers and Panchayat (e.g., poor sanitation and low literacy).","2. Aim and objectives: clean village, 100 adults literate in 3 months.","3. Team: cadets, teachers, villagers, volunteers.","4. Partners: Gram Panchayat, NGO, school, local health centre.","5. Activities: cleanliness drives, dustbins, awareness rallies, evening literacy classes.","6. Resources and budget: books, brooms, bins, posters, small funds.","7. Timeline: week-wise plan.","8. Monitoring: weekly attendance and cleanliness check.","9. Evaluation: before-and-after comparison and feedback.","10. Sustainability: village committee continues after the project."],
"A project that listens to villagers, has a clear plan and involves local people will be successful and lasting.",
["Need assessment","Objectives","Team","Gram Panchayat","Budget","Monitoring","Sustainability"],
"Need - Goal - Plan - Act - Monitor - Evaluate - Sustain = 'NGPAMES'.",
[M("The first step in designing a project is ___.",["Need assessment","Evaluation","Closing","Celebration"],0,"First find out the real needs of the community."),
M("Sustainability means ___.",["Project continues after the team leaves","Project stops soon","Wasting money","Ignoring villagers"],0,"Locals should continue the work after volunteers leave.")],
"Design a social service project for a rural community. (8 marks)",
"Choose a need (e.g., sanitation and literacy), set aims, form team and partners, plan activities, budget and timeline, monitor, evaluate and ensure sustainability."),

T("Ethics, cultural sensitivity and inclusiveness in social service",
"Social service karte waqt ethics ka dhyan rakho: sabki izzat, honesty aur privacy. Local culture aur bhasha ki respect karo. Kisi ke saath bhed-bhav na karo - sabko include karo, women, disabled aur gareeb ko bhi.",
"A volunteer asks permission before taking photos in a village and avoids sharing private details. This is ethical behaviour.",
"Ethics are moral rules of right and wrong. In social service, ethics, cultural sensitivity and inclusiveness ensure respect and fairness for all.",
["Respect and dignity: treat everyone equally.","Honesty and transparency: no cheating in funds or reports.","Consent and privacy: ask permission and keep personal details safe.","Do no harm: avoid actions that may hurt people.","Cultural sensitivity: respect local customs, dress, language and beliefs.","Inclusiveness: include women, elderly, disabled, minorities and poor.","No imposing of own views: listen to the community.","Accountability: be responsible for actions and funds."],
"Ethical, sensitive and inclusive service earns trust and makes the work more effective.",
["Ethics","Dignity","Transparency","Consent","Cultural sensitivity","Inclusiveness","Accountability"],
"'RECIPE': Respect, Ethics, Consent, Inclusion, Privacy, Equality.",
[M("Cultural sensitivity means ___.",["Respecting local customs","Mocking customs","Ignoring culture","Imposing own culture"],0,"Respect local beliefs and customs."),
M("Inclusiveness means ___.",["Including everyone","Excluding minorities","Serving only rich","Ignoring disabled"],0,"Everyone should benefit and participate.")],
"Why are ethics, cultural sensitivity and inclusiveness important in social service? (5 marks)",
"They ensure respect, trust and fairness; work should be honest, respect local culture and include all groups."),

T("Importance of social service and national development",
"Social service se gareebi, bimari aur ashiksha kam hoti hai, jisse desh aage badhta hai. Sarkar akele sab nahi kar sakti, isliye logon ka seva mein hissa lena zaroori hai.",
"Volunteers run a free health camp in a village. Sick people are treated early and can go back to work.",
"Social service means helping people and society voluntarily. It is closely linked to national development because it improves the quality of life of people.",
["Reduces poverty and inequality: helps weaker sections.","Improves health and education: camps, literacy drives.","Supports the government: fills gaps in schemes.","Builds social harmony: people of different groups work together.","Develops character: kindness, discipline and responsibility.","Promotes sustainable development: environment protection.","Creates better human resources: healthier and educated citizens.","Strengthens democracy: active and aware citizens."],
"Thus social service is a powerful tool for building a strong, equal and developed India.",
["Voluntary service","Poverty reduction","Health and education","Social harmony","Sustainable development","Human resource","Nation building"],
"'SERVE': Society, Equality, Responsibility, Values, Education.",
[M("Social service helps national development by ___.",["Improving quality of life","Increasing crime","Dividing people","Stopping education"],0,"It improves people's health, education and income."),
M("Social service is generally ___.",["Voluntary","Forced","Paid only","Illegal"],0,"It is done willingly to help others.")],
"Explain the importance of social service in national development. (5 marks)",
"Social service reduces poverty, improves health and education, supports government work, builds harmony and develops responsible citizens."),

T("Challenges in poverty, inequality and education in India",
"India mein abhi bhi gareebi, asamanta aur education ki kami badi problems hain. Gareebi se bachche school nahi ja pate, aur bina education ke gareebi ghoomti rehti hai.",
"A poor family sends its child to work instead of school. The child grows up with low income - a poverty-education cycle.",
"India has made progress, but poverty, inequality and weak access to quality education remain major challenges.",
["Poverty: low income, unemployment, hunger and poor housing.","Inequality: gaps between rich-poor, rural-urban, men-women and castes.","Education: dropouts, poor quality, lack of teachers and buildings, and digital divide.","Link between all three: poor families cannot afford education, and lack of education keeps them poor.","Other issues: child labour, malnutrition and lack of health care.","Government schemes: free education, mid-day meals, skill development and job schemes.","Role of citizens and NGOs: awareness, volunteering and support.","Solutions: inclusive growth, skill training, quality education and equal opportunities."],
"To remove these challenges, government, society and youth must work together.",
["Poverty","Unemployment","Inequality","Dropouts","Digital divide","Child labour","Skill development"],
"'PIE': Poverty, Inequality, Education.",
[M("Which is an education challenge in India?",["School dropouts","Too many teachers","Free uniform for all","No problem"],0,"Dropouts and poor quality are key problems."),
M("Poverty and education are ___.",["Linked","Unrelated","Opposite","Same"],0,"Poverty reduces education and low education causes poverty.")],
"Discuss the challenges of poverty, inequality and education in India. (5 marks)",
"Poverty, inequality and weak education form a cycle; solutions include inclusive growth, schemes, skill training and quality education."),

T("MGNREGA and Pradhan Mantri Awas Yojana (PMAY)",
"MGNREGA mein gaon ke ghar ko saal mein 100 din ka kaam (rozgar) ki guarantee milti hai. PMAY mein gareeb logon ko pakka ghar milta hai. Dono schemes gareebi kam karne ke liye hain.",
"A villager gets 100 days of work digging a pond under MGNREGA. A poor family builds a pucca house under PMAY.",
"MGNREGA and PMAY are important government schemes for rural employment and housing. (Note: the government has been reforming the rural employment law recently; write MGNREGA as taught in your syllabus and check your class notes for updates.)",
["MGNREGA - meaning: Mahatma Gandhi National Rural Employment Guarantee Act, 2005.","Aim: guarantee of 100 days of wage employment per year to rural households whose adult members agree to do unskilled manual work.","Features: demand-driven work, wages through bank accounts, at least one-third participation of women, work near home.","Types of work: ponds, roads, water conservation, afforestation.","Role of Gram Panchayat and social audit.","PMAY - meaning: Pradhan Mantri Awas Yojana, started in 2015 with the goal of 'Housing for All'.","Two parts: PMAY-Gramin (rural) and PMAY-Urban.","Benefits: pucca house with toilet, electricity, water and women's ownership/priority.","Challenges: delays, corruption, wage delays and quality of houses."],
"These schemes reduce poverty, create assets, improve living standards and support rural development.",
["MGNREGA 2005","100 days","Wage employment","Unskilled work","Gram Panchayat","PMAY 2015","Housing for All","Pucca house"],
"MGNREGA = 100 days Work; PMAY = Pucca house (2015).",
[M("MGNREGA guarantees how many days of work?",["50","75","100","200"],2,"Original MGNREGA guarantees 100 days of wage employment per rural household."),
M("PMAY mainly aims to provide ___.",["Pucca houses","Free cars","Free phones","Free land everywhere"],0,"PMAY targets 'Housing for All' with pucca houses.")],
"Write short notes on MGNREGA and PMAY. (5-8 marks)",
"MGNREGA gives 100 days of guaranteed rural wage work; PMAY provides pucca houses under the 'Housing for All' mission."),

T("Technology and digital initiatives in rural development",
"Ab gaon mein bhi mobile, internet aur apps pahunch rahe hain. Digital India, UPI, e-health aur online padhai se gaon ke logon ko suvidha aur paise ka fayda mil raha hai.",
"A farmer checks crop prices on his phone and sells at the right market instead of depending on a middleman.",
"Technology helps connect villages to services, markets and knowledge, and improves quality of life.",
["Digital India (2015): to make India digitally empowered.","Common Service Centres (CSC): give government services in villages.","BharatNet: broadband to Gram Panchayats.","UPI and Direct Benefit Transfer: easy and safe money transfer and subsidy.","e-Health and telemedicine (e.g., eSanjeevani): doctors online.","e-Learning platforms: DIKSHA and SWAYAM.","Agri-tech: weather apps, e-NAM market, drone and soil testing.","Challenges: poor connectivity and electricity, low digital literacy and cost of devices."],
"With better access and training, technology can speed up rural development and reduce the gap between villages and cities.",
["Digital India","CSC","BharatNet","UPI","DBT","Telemedicine","e-learning"],
"'DUB-CAT': Digital India, UPI, BharatNet, CSC, Agri-tech, Telemedicine.",
[M("BharatNet provides ___ to Gram Panchayats.",["Broadband internet","Free tractors","Free houses","Ration"],0,"BharatNet aims to give broadband connectivity."),
M("UPI helps in ___.",["Digital payments","Weather forecast only","Building roads","Voting"],0,"UPI enables easy digital payments.")],
"Explain the role of technology and digital initiatives in rural development. (5 marks)",
"Digital India, CSCs, BharatNet, UPI/DBT, telemedicine, e-learning and agri-tech bring services, markets and education to villages."),

T("Role and challenges of NGOs in India",
"NGO matlab Non-Governmental Organisation. Ye sarkar se alag hote hain aur samaj ki bhalai ke liye kaam karte hain - jaise health, education, environment. Par inko funds, trained staff aur rules ki problems hoti hain.",
"An NGO runs night schools for working children and trains them in skills.",
"NGOs are voluntary, non-profit organisations that work independently of the government for social welfare.",
["Role - Service delivery: education, health, food and shelter.","Role - Awareness and advocacy: rights, environment and gender issues.","Role - Disaster relief and rehabilitation.","Role - Skill training and livelihood support.","Role - Bridge between people and government.","Challenge - Funding: dependency on donations and grants.","Challenge - Rules and compliance: such as the Foreign Contribution (Regulation) Act (FCRA) for foreign funds.","Challenge - Lack of trained staff and volunteers.","Challenge - Accountability, trust and sometimes corruption, and coordination with government."],
"Strong, transparent and well-funded NGOs can greatly help India's development.",
["NGO","Non-profit","Voluntary","Advocacy","Funding","FCRA","Accountability"],
"'NGO' = Not for profit, Grassroots, Outreach.",
[M("NGO stands for ___.",["Non-Governmental Organisation","National Group Office","New Government Order","Non-General Operation"],0,"NGO is Non-Governmental Organisation."),
M("A common challenge for NGOs is ___.",["Funding","Too much money","No work","Too many staff"],0,"Funding and compliance are common challenges.")],
"Discuss the role and challenges of NGOs in India. (5-8 marks)",
"NGOs deliver services, create awareness and help in disasters; challenges include funding, compliance, staff shortage and accountability.")
]}
];

/* Unit I short-answer topics */
const U1SHORT=[
["Aims and objectives of NCC","To develop character, comradeship, discipline, secular outlook, adventure and selfless service; to build trained, motivated youth for leadership; and to motivate youth for armed forces. NCC was formed in 1948 under the Ministry of Defence."],
["National, state and unit-level structure","National: NCC HQ Delhi under DG. State: Directorates under ADG. Group: Group Commander. Unit: Commanding Officer, with ANOs training cadets. Wings: Army, Navy, Air."],
["Different types of NCC camps","Annual Training Camp, Combined Annual Training Camp, National Integration Camp, Thal Sainik, Vayu Sainik and Nau Sainik Camps, Republic Day Camp, attachment and adventure camps."],
["Incentives offered to cadets","Certificates, armed forces entry benefits, preference in jobs and admission, bonus marks, free camps with allowances, adventure and exchange programmes, awards."],
["Duties of cadets","Attend training regularly, obey orders, wear proper uniform, participate in camps, serve society, respect seniors, keep good character and protect property."],
["Character building","Developing honesty, discipline, courage, integrity and selfless service. NCC does it through drill, camps, pledge, social service and leadership training."],
["National integration","Feeling of oneness among all Indians despite differences. NCC promotes it through mixed camps, common uniform, NIC and Youth Exchange."],
["NCC certificate categories and their importance","Usually A (Junior Division/Wing), B (after second year of Senior Division) and C (after third year of Senior Division). The C certificate gives the maximum benefits like armed forces entry preference. Check exact rules with your unit."]
];

/* ================= STATE ================= */
const TOTAL=5*3600;
const LS="ncc4_study_v1";
let ALL=[];
UNITS.forEach((u,ui)=>u.topics.forEach((t,ti)=>{t.id="u"+(ui+1)+"t"+(ti+1);t.ui=ui;t.ti=ti;ALL.push(t)}));
let S=load();
function dflt(){return{done:{},studied:0,notes:"",best:{},ans:{}}}
function load(){try{return Object.assign(dflt(),JSON.parse(localStorage.getItem(LS)||"{}"))}catch(e){return dflt()}}
function save(){try{localStorage.setItem(LS,JSON.stringify(S))}catch(e){}}
let V={view:"dash",idx:0,openUnit:0};
let running=false,last=0;
let Q=null;
let rev={left:900,run:false,iv:null};

const $=s=>document.querySelector(s);
const esc=s=>String(s);
function pct(done,total){return total?Math.round(done*100/total):0}
function unitProg(ui){const ts=UNITS[ui].topics;const d=ts.filter(t=>S.done[t.id]).length;return{d,n:ts.length,p:pct(d,ts.length)}}
function overall(){const d=ALL.filter(t=>S.done[t.id]).length;return{d,n:ALL.length,p:pct(d,ALL.length)}}
function fmt(sec){sec=Math.max(0,Math.floor(sec));const h=Math.floor(sec/3600),m=Math.floor(sec%3600/60),s=sec%60;return[h,m,s].map(x=>String(x).padStart(2,"0")).join(":")}
function shuffle(a){a=a.slice();for(let i=a.length-1;i>0;i--){const j=Math.floor(Math.random()*(i+1));[a[i],a[j]]=[a[j],a[i]]}return a}

/* ================= TIMER ================= */
function updateTimer(){
 $("#tm").textContent=fmt(TOTAL-S.studied);
 $("#startBtn").textContent=running?"Pause":(S.studied>0?"Resume Study":"Start Study");
 $("#startBtn").classList.toggle("pri",!running);
 const o=overall();
 $("#gp").style.width=o.p+"%";
 $("#gt").textContent=o.d+"/"+o.n+" topics done ("+o.p+"%)";
}
setInterval(()=>{
 if(running){const now=Date.now();S.studied+=(now-last)/1000;last=now;if(S.studied>=TOTAL){S.studied=TOTAL;running=false}
  if(Math.floor(S.studied)%5===0)save();updateTimer()}
},1000);
function toggleStudy(){
 if(running){running=false;save()}
 else{running=true;last=Date.now();if(V.view==="dash"){const n=ALL.findIndex(t=>!S.done[t.id]);V={view:"topic",idx:n<0?0:n,openUnit:n<0?0:ALL[n].ui};}}
 render();
}
document.addEventListener("visibilitychange",()=>{if(document.hidden)save()});
window.addEventListener("beforeunload",save);

/* ================= SIDEBAR ================= */
function renderSide(){
 let h='<div class="brand">NCC-1 (AEC-IV)<small>Semester IV - 5 Hour Exam Planner</small></div>';
 const nb=(v,l)=>'<button class="nav-btn '+(V.view===v?"on":"")+'" data-nav="'+v+'">'+l+'</button>';
 h+=nb("dash","&#127968; Dashboard");
 h+='<div class="sec-title">Units</div>';
 UNITS.forEach((u,ui)=>{
  const p=unitProg(ui);
  h+='<div class="unit"><button class="unit-h" data-unit="'+ui+'"><b>'+u.n+': '+u.name+'</b><span>'+u.min+' min &bull; '+p.d+'/'+p.n+' done ('+p.p+'%)</span><div class="mini"><i style="width:'+p.p+'%"></i></div></button>';
  if(V.openUnit===ui){h+='<div class="tlist">';u.topics.forEach((t,ti)=>{const gi=ALL.indexOf(t);h+='<button class="'+(S.done[t.id]?"ok ":"")+(V.view==="topic"&&V.idx===gi?"on":"")+'" data-topic="'+gi+'">'+(ti+1)+'. '+t.title+'</button>'});h+='</div>'}
  h+='</div>';
 });
 h+='<div class="sec-title">Exam Tools</div>';
 h+=nb("notes","&#128221; Quick Notes")+nb("imp","&#11088; Important Questions")+nb("quiz","&#9989; MCQ Test")+nb("rand","&#127922; Random Quiz")+nb("rev","&#9889; 15-Min Revision");
 $("#side").innerHTML=h;
}

/* ================= VIEWS ================= */
function render(){
 renderSide();
 const v=V.view;
 if(v==="dash")dash();else if(v==="topic")topicView();else if(v==="notes")notesView();else if(v==="imp")impView();else if(v==="quiz")quizSetup();else if(v==="rand")randomQuiz();else if(v==="rev")revView();
 updateTimer();
 document.body.classList.remove("menu");
}
function setView(html){$("#view").innerHTML=html;window.scrollTo(0,0)}

function dash(){
 const o=overall();
 const plan=UNITS.map((u,ui)=>{const p=unitProg(ui);return'<tr><td><b>'+u.n+'</b> '+u.name+'</td><td>'+u.min+' min</td><td>'+u.topics.length+'</td><td>~'+Math.round(u.min/u.topics.length)+' min</td><td>'+p.p+'%</td></tr>'}).join("");
 setView('<h1>Your 5-Hour Study Plan</h1><p class="sub">NCC-1 (AEC-IV), Semester IV. Study topic by topic, mark them done, then test yourself.</p>'+
 '<div class="grid"><div class="stat"><span class="sub">Time left</span><b style="color:var(--warn)">'+fmt(TOTAL-S.studied)+'</b></div><div class="stat"><span class="sub">Topics completed</span><b>'+o.d+' / '+o.n+'</b></div><div class="stat"><span class="sub">Overall progress</span><b class="ok">'+o.p+'%</b></div></div>'+
 '<div class="card"><h3>Time table</h3><table><tr><th>Part</th><th>Time</th><th>Topics</th><th>Per topic</th><th>Done</th></tr>'+plan+'<tr><td><b>Final</b> Revision</td><td>15 min</td><td>All</td><td>-</td><td>-</td></tr><tr><td><b>Total</b></td><td><b>5 hours</b></td><td>'+ALL.length+'</td><td></td><td></td></tr></table></div>'+
 '<div class="card"><h3>How to use</h3><ol><li>Press <b>Start Study</b> - the timer begins and you jump to your next topic.</li><li>Read the easy Hinglish explanation, then the exam answer, then memorise keywords.</li><li>Solve 2 MCQs and the short question, then press <b>Mark completed</b>.</li><li>After each unit, take the <b>MCQ Test</b>. In the last 15 minutes use <b>Revision mode</b>.</li></ol><div class="row" style="margin-top:10px"><button class="btn pri" id="goStart">'+(running?"Continue Studying":"Start Study")+'</button><button class="btn" data-nav="imp">Important Questions</button><button class="btn" data-nav="rev">Revision Mode</button><button class="btn" data-nav="rand">Random Quiz</button></div></div>');
}

function mcqHTML(m,key,i){
 const a=S.ans[key];let h='<div class="card" style="margin-top:10px"><b>Q'+(i+1)+'. '+m.q+'</b>';
 m.o.forEach((o,k)=>{let c="opt";if(a!==undefined){c+=" lock";if(k===m.a)c+=" right";else if(k===a)c+=" wrong"}h+='<button class="'+c+'" data-mcq="'+key+'" data-k="'+k+'">'+String.fromCharCode(65+k)+'. '+o+'</button>'});
 if(a!==undefined)h+='<div class="expl">'+(a===m.a?'<b class="ok">Correct!</b> ':'<b class="bad">Wrong.</b> ')+'Answer: '+String.fromCharCode(65+m.a)+'. '+m.e+'</div>';
 return h+'</div>';
}

function topicView(){
 const t=ALL[V.idx],u=UNITS[t.ui];
 const pts=t.pts.map(p=>{const k=p.indexOf(": ");return k>0?'<li><b>'+p.slice(0,k)+':</b> '+p.slice(k+2)+'</li>':'<li>'+p+'</li>'}).join("");
 const isd=!!S.done[t.id];
 setView('<div class="sub">'+u.n+' &bull; '+u.name+' &bull; Topic '+(t.ti+1)+' of '+u.topics.length+' &bull; suggested time ~'+Math.round(u.min/u.topics.length)+' min</div><h1>'+t.title+'</h1>'+
 '<div class="card hing"><div class="lbl">1. Samjho (Easy Hinglish)</div><p>'+t.h+'</p></div>'+
 '<div class="card exm"><div class="lbl">2. Example</div><p>'+t.ex+'</p></div>'+
 '<div class="card exa"><div class="lbl">3. Exam Answer (5-8 marks, simple English)</div><h4>Introduction</h4><p>'+t.intro+'</p><h4>Main Points</h4><ol>'+pts+'</ol><h4>Conclusion</h4><p>'+t.concl+'</p></div>'+
 '<div class="card"><div class="lbl">4. Keywords to memorise</div><div>'+t.kw.map(k=>'<span class="chip">'+k+'</span>').join("")+'</div></div>'+
 '<div class="card mem"><div class="lbl">5. Memory trick</div><p>'+t.mt+'</p></div>'+
 '<h2>Practice</h2>'+t.mcq.map((m,i)=>mcqHTML(m,t.id+":"+i,i)).join("")+
 '<div class="card"><b>Short question:</b> '+t.sq+'<details><summary>Show model answer</summary><p style="margin-top:6px">'+t.sa+'</p></details></div>'+
 '<div class="nav2"><button class="btn" id="prevT" '+(V.idx===0?"disabled":"")+'>&larr; Previous Topic</button><button class="btn done-btn '+(isd?"isdone":"blue")+'" id="doneT">'+(isd?"&#10003; Completed (click to undo)":"Mark as completed")+'</button><button class="btn pri" id="nextT" '+(V.idx===ALL.length-1?"disabled":"")+'>Next Topic &rarr;</button></div>');
}

function notesView(){
 let h='<h1>Quick Notes</h1><p class="sub">All keywords and memory tricks in one place. Your own notes are saved automatically.</p>';
 UNITS.forEach(u=>{h+='<div class="card"><h3>'+u.n+': '+u.name+'</h3>';u.topics.forEach(t=>{h+='<p style="margin-top:8px"><b>'+t.title+'</b><br>'+t.kw.map(k=>'<span class="chip">'+k+'</span>').join("")+'<br><span class="sub">&#128161; '+t.mt+'</span></p>'});h+='</div>'});
 h+='<div class="card"><h3>My Notes</h3><textarea id="myNotes" placeholder="Write your own notes here...">'+S.notes.replace(/&/g,"&amp;").replace(/</g,"&lt;")+'</textarea></div>';
 setView(h);
 $("#myNotes").addEventListener("input",e=>{S.notes=e.target.value;save()});
}

function impView(){
 let h='<h1>Important Questions</h1><p class="sub">Tap a question to see the short model answer. For full answers open the topic.</p>';
 h+='<div class="card"><h3>Unit I - Short Answer Topics</h3>'+U1SHORT.map(q=>'<details><summary>'+q[0]+'</summary><p style="margin-top:6px">'+q[1]+'</p></details>').join("")+'</div>';
 UNITS.forEach((u,ui)=>{h+='<div class="card"><h3>'+u.n+': '+u.name+' - Long Questions</h3>'+u.topics.map(t=>'<details><summary>'+t.sq+'</summary><p style="margin-top:6px">'+t.sa+'</p><button class="btn" style="margin-top:6px" data-topic="'+ALL.indexOf(t)+'">Open full topic</button></details>').join("")+'</div>'});
 setView(h);
}

/* ---------- Quiz engine ---------- */
function allMCQ(units){const out=[];ALL.forEach(t=>{if(units==="all"||units.includes(t.ui))t.mcq.forEach(m=>out.push(Object.assign({},m,{src:t.title})))});return out}
function prep(list){return list.map(m=>{const idx=shuffle(m.o.map((_,i)=>i));return{q:m.q,o:idx.map(i=>m.o[i]),a:idx.indexOf(m.a),e:m.e,src:m.src}})}
function quizSetup(){
 const bests=Object.keys(S.best).map(k=>'<span class="chip">'+k+': best '+S.best[k]+'</span>').join("")||'<span class="sub">No attempts yet.</span>';
 setView('<h1>MCQ Test</h1><p class="sub">Choose a unit. Explanations appear after every answer.</p><div class="card"><div class="row"><select id="qUnit"><option value="all">All Units (full test)</option>'+UNITS.map((u,i)=>'<option value="'+i+'">'+u.n+': '+u.name+'</option>').join("")+'</select><button class="btn pri" id="qStart">Start Test</button></div><div style="margin-top:10px">'+bests+'</div></div>');
}
function startQuiz(list,label){Q={list:prep(list),i:0,score:0,done:false,sel:null,label};quizRender()}
function quizRender(){
 if(Q.done||Q.i>=Q.list.length){Q.done=true;const p=pct(Q.score,Q.list.length);const key=Q.label;if(S.best[key]===undefined||p>parseInt(S.best[key]))S.best[key]=p+"%";save();
  setView('<h1>Test Finished</h1><div class="card" style="text-align:center"><div class="big '+(p>=60?"ok":"bad")+'">'+Q.score+' / '+Q.list.length+'</div><p>'+p+'% &bull; '+(p>=80?"Excellent! You are exam ready.":p>=60?"Good. Revise weak topics once more.":"Revise the topics again and retry.")+'</p><div class="row" style="justify-content:center;margin-top:10px"><button class="btn pri" id="qAgain">Try again</button><button class="btn" data-nav="quiz">Change test</button><button class="btn" data-nav="rev">Revision</button></div></div>');return}
 const m=Q.list[Q.i];
 let h='<div class="sub">'+Q.label+' &bull; Question '+(Q.i+1)+' of '+Q.list.length+' &bull; Score '+Q.score+'</div><div class="gbar" style="margin:6px 0"><i style="width:'+pct(Q.i,Q.list.length)+'%"></i></div><div class="card"><b>'+m.q+'</b>';
 m.o.forEach((o,k)=>{let c="opt";if(Q.sel!==null){c+=" lock";if(k===m.a)c+=" right";else if(k===Q.sel)c+=" wrong"}h+='<button class="'+c+'" data-q="'+k+'">'+String.fromCharCode(65+k)+'. '+o+'</button>'});
 if(Q.sel!==null)h+='<div class="expl">'+(Q.sel===m.a?'<b class="ok">Correct!</b> ':'<b class="bad">Wrong.</b> ')+'Answer: '+String.fromCharCode(65+m.a)+'. '+m.e+'<br><span class="sub">Topic: '+m.src+'</span></div><div class="row" style="margin-top:10px"><button class="btn pri" id="qNext">'+(Q.i===Q.list.length-1?"Finish":"Next")+' &rarr;</button></div>';
 h+='</div>';setView(h);
}
function randomQuiz(){startQuiz(shuffle(allMCQ("all")).slice(0,10),"Random Quiz")}

/* ---------- Revision ---------- */
function revView(){
 let h='<h1>Final 15-Minute Revision</h1><p class="sub">Only definitions, keywords and main points. Read fast, do not stop.</p><div class="card row"><span class="big" style="color:var(--warn)" id="revT">'+fmt(rev.left)+'</span><button class="btn pri" id="revBtn">'+(rev.run?"Pause":"Start 15-min timer")+'</button><button class="btn" id="revReset">Reset</button></div>';
 UNITS.forEach(u=>{h+='<h2>'+u.n+': '+u.name+'</h2>';u.topics.forEach(t=>{h+='<div class="card"><b>'+t.title+'</b><p style="margin:4px 0"><i>Definition:</i> '+t.d+'</p><div>'+t.kw.map(k=>'<span class="chip">'+k+'</span>').join("")+'</div><p class="sub" style="margin-top:4px"><b>Main points:</b> '+t.pts.map(p=>{const k=p.indexOf(":");return k>0?p.slice(0,k):p}).join(" &bull; ")+'</p><p class="sub">&#128161; '+t.mt+'</p></div>'})});
 setView(h);
}
function revTick(){if(rev.run){rev.left=Math.max(0,rev.left-1);const e=$("#revT");if(e)e.textContent=fmt(rev.left);if(rev.left===0){rev.run=false;if(V.view==="rev")render()}}}
setInterval(revTick,1000);

/* ================= EVENTS ================= */
document.addEventListener("click",e=>{
 const t=e.target.closest("button");
 if(e.target.id==="ov"){document.body.classList.remove("menu");return}
 if(!t)return;
 if(t.id==="burger"){document.body.classList.toggle("menu");return}
 if(t.id==="startBtn"){toggleStudy();return}
 if(t.id==="goStart"){toggleStudy();return}
 if(t.id==="resetBtn"){if(confirm("Reset ALL progress, timer, notes and scores? This cannot be undone.")){localStorage.removeItem(LS);S=dflt();running=false;Q=null;rev.left=900;rev.run=false;V={view:"dash",idx:0,openUnit:0};render()}return}
 if(t.dataset.nav){V.view=t.dataset.nav;render();return}
 if(t.dataset.unit!==undefined){const ui=+t.dataset.unit;V.openUnit=V.openUnit===ui?-1:ui;if(V.openUnit===ui){const first=ALL.findIndex(x=>x.ui===ui&&!S.done[x.id]);V.view="topic";V.idx=first<0?ALL.findIndex(x=>x.ui===ui):first}render();return}
 if(t.dataset.topic!==undefined){V.view="topic";V.idx=+t.dataset.topic;V.openUnit=ALL[V.idx].ui;render();return}
 if(t.dataset.mcq){const k=t.dataset.mcq;if(S.ans[k]===undefined){S.ans[k]=+t.dataset.k;save();const y=window.scrollY;render();window.scrollTo(0,y)}return}
 if(t.id==="prevT"&&V.idx>0){V.idx--;V.openUnit=ALL[V.idx].ui;render();return}
 if(t.id==="nextT"&&V.idx<ALL.length-1){V.idx++;V.openUnit=ALL[V.idx].ui;render();return}
 if(t.id==="doneT"){const id=ALL[V.idx].id;if(S.done[id])delete S.done[id];else S.done[id]=true;save();const y=window.scrollY;render();window.scrollTo(0,y);return}
 if(t.id==="qStart"){const v=$("#qUnit").value;const label=v==="all"?"All Units":UNITS[+v].n;startQuiz(shuffle(allMCQ(v==="all"?"all":[+v])),label);return}
 if(t.dataset.q!==undefined&&Q&&Q.sel===null){Q.sel=+t.dataset.q;if(Q.sel===Q.list[Q.i].a)Q.score++;quizRender();return}
 if(t.id==="qNext"){Q.i++;Q.sel=null;quizRender();return}
 if(t.id==="qAgain"){if(Q.label==="Random Quiz")randomQuiz();else startQuiz(allMCQ(Q.label==="All Units"?"all":[UNITS.findIndex(u=>u.n===Q.label)]),Q.label);return}
 if(t.id==="revBtn"){rev.run=!rev.run;t.textContent=rev.run?"Pause":"Start 15-min timer";return}
 if(t.id==="revReset"){rev.left=900;rev.run=false;revView();return}
});
document.addEventListener("keydown",e=>{if(V.view==="topic"&&!/INPUT|TEXTAREA|SELECT/.test(e.target.tagName)){if(e.key==="ArrowRight"&&V.idx<ALL.length-1){V.idx++;V.openUnit=ALL[V.idx].ui;render()}if(e.key==="ArrowLeft"&&V.idx>0){V.idx--;V.openUnit=ALL[V.idx].ui;render()}}});
render();
</script>
</body>
</html>

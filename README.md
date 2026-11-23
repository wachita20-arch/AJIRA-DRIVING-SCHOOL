<AJIRA DRIVING SCHOOL>
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no, viewport-fit=cover">
<meta name="theme-color" content="#0b2c4a">
<title>AJIRA Driving School - ADMISSION • LESSONS • PAYMENTS • BALANCES • CLASSES</title>
<link rel="manifest" href="manifest.json">
<style>
*{box-sizing:border-box;font-family:Arial,sans-serif;-webkit-tap-highlight-color:transparent}
body{margin:0;background:#0b2c4a;display:flex;justify-content:center}
.phone{width:100%;max-width:460px;min-height:100vh;background:#fff;display:flex;flex-direction:column}
header{background:#0b2c4a;color:#fff;padding:14px;text-align:center;position:sticky;top:0;z-index:10}
header h1{margin:0;font-size:18px} header p{margin:4px 0 0;font-size:12px;opacity:.9}
header .badge{background:#ffc107;color:#000;padding:3px 8px;border-radius:10px;font-size:11px;font-weight:700}
.lang{display:flex;gap:6px;margin-top:10px}.lang button{flex:1;padding:9px;background:#fff;color:#0b2c4a;font-weight:900;min-height:38px}.lang button.active{background:#ffc107}
main{padding:14px 14px 90px;flex:1}
.card{background:#f6f6f6;border-radius:12px;padding:12px;margin-bottom:10px}
button{width:100%;padding:13px;border:0;border-radius:10px;background:#0b2c4a;color:#fff;font-weight:700;font-size:15px;cursor:pointer;margin-top:8px;min-height:48px}
button.secondary{background:#eee;color:#222} button.green{background:#1a7a3a} button.orange{background:#ef6c00} button.red{background:#b71c1c}
input,select,textarea{width:100%;padding:12px;border:1px solid #ddd;border-radius:10px;margin:5px 0;font-size:16px}
.small{font-size:12px;color:#555}
.badge{display:inline-block;background:#ffe082;padding:4px 10px;border-radius:20px;font-size:11px;font-weight:700}
.top{display:flex;justify-content:space-between;align-items:center}
.hidden{display:none}
footer{padding:12px;text-align:center;font-size:12px;color:#555;border-top:1px solid #eee}
.tabs{display:flex;gap:6px;margin-bottom:10px;flex-wrap:wrap;position:sticky;top:0;background:#fff;padding:6px 0;z-index:5}
.tabs button{flex:1;background:#eee;color:#222;padding:10px;min-width:70px;font-size:13px}
.tabs button.active{background:#0b2c4a;color:#fff}
.bottom-nav{position:fixed;bottom:0;left:50%;transform:translateX(-50%);width:100%;max-width:460px;background:#0b2c4a;display:flex;padding:8px 4px;z-index:20}
.bottom-nav button{background:transparent;color:#aaa;font-size:11px;padding:6px 2px;margin:0;min-height:auto}
.bottom-nav button.active{color:#ffc107} .bottom-nav span{font-size:18px;display:block}
.alert-green{background:#e8f5e9;border:1px solid #1a7a3a;padding:10px;border-radius:10px;margin-bottom:10px}
.alert-orange{background:#fff3e0;border:2px solid #ef6c00;padding:12px;border-radius:10px;margin-bottom:10px;font-weight:700;color:#e65100}
.alert-red{background:#ffebee;border:2px solid #b71c1c;padding:12px;border-radius:10px;margin-bottom:10px;font-weight:700;color:#b71c1c}
.bar{height:14px;background:#eee;border-radius:7px;overflow:hidden;margin:6px 0}.fill{height:100%;background:#1a7a3a}
.avatar{width:52px;height:52px;border-radius:50%;background:#0b2c4a;color:#fff;display:flex;align-items:center;justify-content:center;font-size:20px;font-weight:900;overflow:hidden}
.pay-box{background:#e8f5e9;border:2px solid #1a7a3a;border-radius:12px;padding:12px}.pay-box.red{background:#ffebee;border-color:#b71c1c}
.progress-ring{width:90px;height:90px;border-radius:50%;background:conic-gradient(#1a7a3a 0deg,#eee 0deg);display:flex;align-items:center;justify-content:center;margin:auto}
.progress-ring div{width:68px;height:68px;background:#fff;border-radius:50%;display:flex;align-items:center;justify-content:center;font-weight:900;font-size:18px}
.receipt{background:#fff;border:2px dashed #0b2c4a;border-radius:10px;padding:14px;text-align:center}
.class-slot{border-left:5px solid #0b2c4a}
.class-slot.full{border-left-color:#b71c1c;background:#ffebee}
.class-slot.mine{border-left-color:#1a7a3a;background:#e8f5e9}
.kpi{display:grid;grid-template-columns:1fr 1fr;gap:8px}
.kpi div{background:#fff;border-radius:10px;padding:10px;text-align:center}
</style>
</head>
<body>
<div class="phone">
<header><div>🇰🇪 NPS AJIRA DRIVING SCHOOL</div><h1>ADMISSION • LESSONS • FEES • BALANCES • CLASSES</h1><p>One App - Everything</p><span class="badge">NTSA APPROVED • EN / SW • ULTIMATE v4</span>
<div class="lang"><button id="btnEN" class="active" onclick="setLang('en')">🇬🇧 ENGLISH</button><button id="btnSW" onclick="setLang('sw')">🇰🇪 KISWAHILI</button></div>
<a href="https://wa.me/c/254777725770" target="_blank" style="text-decoration:none"><button style="background:#25D366">💬 JOIN WHATSAPP CHANNEL - 0777 725 770</button></a>
</header>
<main>
<div id="loginView">
  <h2 data-i18n="welcome">Welcome - Ajira Driving School</h2>
  <select id="userType" onchange="toggleLogin()"><option value="student" data-i18n="iAmStudent">I am a Student - Admission / Lessons / Payments</option><option value="instructor" data-i18n="iAmInstructor">I am an Instructor / Admin</option></select>
  <div id="studentLogin"><input id="stuName" data-ph="fullName" placeholder="Full Name *"><input id="stuPhone" data-ph="phone" placeholder="Phone e.g. 0712345678" inputmode="tel"><input id="stuId" data-ph="idNo" placeholder="ID No." inputmode="numeric"></div>
  <div id="instructorLogin" class="hidden"><input id="offName" data-ph="instructorName" placeholder="Instructor / Admin Name"><input id="offNo" data-ph="staffNo" placeholder="Staff No." inputmode="numeric"><select id="offRole"><option data-i18n="roleInstructor">Instructor</option><option data-i18n="roleAdmin">Admin</option><option data-i18n="roleOCS">OCS / MT Officer</option></select></div>
  <button onclick="login()" data-i18n="login">Login</button>
  <p class="small" data-i18n="loginHint">Student: Name + Phone only. Instructor Demo: Any name + number.</p>
</div>

<div id="appView" class="hidden">
  <div class="top"><b><span data-i18n="hello">Hello</span>, <span id="userName"></span></b><button class="secondary" style="width:auto" onclick="logout()" data-i18n="logout">Logout</button></div>
  <p class="small"><span id="stationLabel"></span> • <span id="dateLabel"></span></p>
  <div id="alertBox"></div>

  <!-- DASHBOARD -->
  <div class="kpi">
    <div><b id="kStudents" style="font-size:22px;color:#0b2c4a">0</b><br><span class="small" data-i18n="students">Students</span></div>
    <div><b id="kClasses" style="font-size:22px;color:#0b2c4a">0</b><br><span class="small" data-i18n="classesBooked">Classes Booked</span></div>
    <div><b id="kPaid" style="font-size:18px;color:#1a7a3a">Ksh 0</b><br><span class="small" data-i18n="collected">Collected</span></div>
    <div><b id="kOwing" style="font-size:18px;color:#b71c1c">Ksh 0</b><br><span class="small" data-i18n="owing">Still Owing</span></div>
    <div><b id="kLessonsDone" style="font-size:22px">0</b><br><span class="small" data-i18n="lessonsDone">Lessons Completed</span></div>
    <div><b id="kPassed" style="font-size:22px;color:#1a7a3a">0</b><br><span class="small" data-i18n="passed">Passed</span></div>
  </div>

  <!-- MY ADMISSION + PAYMENT CARD -->
  <div class="card" id="myCard" style="margin-top:10px">
    <div class="top"><b>🪪 <span data-i18n="myAdmission">My Admission</span></b><span class="badge" id="myStatusBadge">-</span></div>
    <div id="myAdmissionInfo" class="small"></div>
    <div style="margin-top:8px"><div class="top"><span class="small">💰 <span data-i18n="paid">Paid</span> <b id="myPaid2">Ksh 0</b> / <b id="myFee2">Ksh 0</b> (<b id="myPct">0%</b>)</span><span class="small"><span data-i18n="balance">Balance</span>: <b id="myBal2" style="color:#b71c1c">Ksh 0</b></span></div><div class="bar"><div class="fill" id="myPayBar" style="width:0%"></div></div></div>
    <div style="margin-top:8px"><div class="top"><span class="small">📚 <span data-i18n="lessons">Lessons</span> <b id="myLessonCount">0/20</b></span><span class="small">📅 <span data-i18n="nextClass">Next Class</span>: <b id="myNextClass">-</b></span></div></div>
    <div id="myCardActions"></div>
  </div>

  <div class="tabs">
    <button id="tabAdmission" class="active" onclick="showTab('admission')">📝 <span data-i18n="admission">Admission</span></button>
    <button id="tabStudents" onclick="showTab('students')">🧑‍🎓 <span data-i18n="students">Students</span></button>
    <button id="tabClasses" onclick="showTab('classes')">📅 <span data-i18n="classes">Classes</span></button>
    <button id="tabLessons" onclick="showTab('lessons')">📚 <span data-i18n="lessons">Lessons</span></button>
    <button id="tabPayments" onclick="showTab('payments')">💰 <span data-i18n="payments">Payments</span></button>
    <button id="tabBalances" onclick="showTab('balances')">⚖️ <span data-i18n="balances">Balances</span></button>
    <button id="tabReport" onclick="showTab('report')">📄 <span data-i18n="report">Report</span></button>
  </div>

  <!-- 1. ADMISSION -->
  <div id="admissionTab">
    <div class="card"><h3 style="margin:0">📝 <span data-i18n="admissionForm">Admission Form - New Student</span></h3><p class="small" data-i18n="admissionHint">Fill once. Student gets Admission No, ID, Course, Payment Plan, Class Schedule automatically.</p>
      <label class="small" data-i18n="selectCourse">Select Course *</label><select id="aCourse" onchange="updateAdmissionInfo()"></select><div id="aCourseInfo" class="small"></div>
      <input id="aName" data-ph="fullName" placeholder="Full Name *"><input id="aPhone" data-ph="phone" placeholder="Phone *" inputmode="tel"><input id="aId" data-ph="idNo" placeholder="ID No. *" inputmode="numeric">
      <input id="aAge" data-ph="age" placeholder="Age" type="number" inputmode="numeric">
      <select id="aGender"><option data-i18n="male">Male</option><option data-i18n="female">Female</option></select>
      <input id="aCounty" data-ph="county" placeholder="County e.g. Trans Nzoia"><input id="aEducation" data-ph="education" placeholder="Education e.g. KCSE C-">
      <input id="aNextKin" data-ph="nextKin" placeholder="Next of Kin Name + Phone e.g. Mary - 0712345678">
      <input id="aAddress" data-ph="address" placeholder="Home / Estate e.g. Eldoret - Kapsoya">
      <select id="aHasLicence"><option data-i18n="noLicence">No Licence - Beginner</option><option data-i18n="haveLicence">Have Licence - Add Class</option><option data-i18n="expiredLicence">Licence Expired - Refresher</option></select>
      <input id="aLicenceNo" data-ph="licenceNo" placeholder="Licence No. (If any)">
      <select id="aSchedule"><option data-i18n="morning">Morning - 8am - 11am</option><option data-i18n="midday">Midday - 11am - 2pm</option><option data-i18n="afternoon">Afternoon - 2pm - 5pm</option><option data-i18n="weekend">Weekend Only - Sat / Sun</option></select>
      <label class="small" data-i18n="paymentPlan">Payment Plan *</label><select id="aPlan" onchange="updateAdmissionInfo()"><option value="full" data-i18n="planFull">Pay in Full - 0% Discount? No, Pay Once</option><option value="2" data-i18n="plan2">2 Installments - 50% Now + 50% Later</option><option value="3" data-i18n="plan3">3 Installments - Deposit + 2 Payments</option><option value="4" data-i18n="plan4">4 Installments - Deposit + 3 Payments</option></select><div id="aPlanInfo" class="small"></div>
      <div style="background:#e8f5e9;border:2px solid #1a7a3a;border-radius:10px;padding:10px"><b>💚 <span data-i18n="payDeposit">Pay Deposit Now - M-Pesa STK Push</span></b>
        <input id="aMpesaPhone" data-ph="mpesaPhone" placeholder="M-Pesa Phone" inputmode="tel"><input id="aDeposit" data-ph="deposit" placeholder="Deposit Ksh e.g. 5000" type="number" inputmode="numeric">
        <button class="green" onclick="stkAdmission()">💚 <span data-i18n="sendStk">Send STK Push</span></button>
        <input id="aMpesaCode" data-ph="mpesaCode" placeholder="M-Pesa Code e.g. QK123ABC">
      </div>
      <button class="green" onclick="admitStudent()">✅ <span data-i18n="admitBtn">Admit Student → Create Admission No.</span></button>
    </div>
    <div id="admissionSuccess"></div>
  </div>

  <!-- 2. STUDENTS -->
  <div id="studentsTab" class="hidden">
    <select id="stuFilter" onchange="renderAll()"><option value="all" data-i18n="all">All</option><option value="Enrolled" data-i18n="enrolled">Enrolled</option><option value="In Training" data-i18n="inTraining">In Training</option><option value="Ready for Test" data-i18n="readyTest">Ready for Test</option><option value="Passed" data-i18n="passed">Passed</option><option value="Failed" data-i18n="failed">Failed</option><option value="Dropped" data-i18n="dropped">Dropped</option></select>
    <input id="stuSearch" data-ph="searchStudent" placeholder="Search name, phone, admission no..." oninput="renderAll()">
    <div id="studentList"></div>
  </div>

  <!-- 3. CLASSES BOOKED -->
  <div id="classesTab" class="hidden">
    <div class="card"><h3 style="margin:0">📅 <span data-i18n="bookClass">Book a Class</span></h3>
      <label class="small" data-i18n="student">Student</label><select id="cStudent" onchange="updateClassPayInfo()"></select><div id="cStudentInfo" class="small"></div>
      <label class="small" data-i18n="selectLesson">Select Lesson / Class *</label><select id="cLesson" onchange="updateClassInfo()"></select><div id="cLessonInfo" class="small"></div>
      <input id="cDate" type="date"><input id="cTime" type="time">
      <select id="cInstructor"><option>Instr. David Otieno - Class B / B+C</option><option>Instr. Peter Kamau - Class C / Defensive</option><option>Instr. Jane Wanjiru - Class D / PSV</option><option>Instr. Mary Achieng - Class A / Motorcycle</option></select>
      <select id="cVehicle"><option>KDJ 123A - Probox (Class B) - Seats: 4</option><option>KDJ 456B - Lorry (Class C) - Seats: 2</option><option>KDJ 789C - Bus (Class D) - Seats: 10</option><option>KMDA 101 - Honda (Class A) - Seats: 1</option></select>
      <select id="cLocation"><option>Eldoret - Yard</option><option>Eldoret - Town Driving</option><option>Kitale - Yard</option><option>Kitale - Town</option></select>
      <select id="cSlot"><option data-i18n="morning">Morning - 8am - 11am</option><option data-i18n="midday">Midday - 11am - 2pm</option><option data-i18n="afternoon">Afternoon - 2pm - 5pm</option><option data-i18n="weekend">Weekend Only - Sat / Sun</option></select>
      <button class="green" onclick="bookClass()">📅 <span data-i18n="bookClassBtn">Book Class</span></button>
    </div>
    <div class="card"><h3 style="margin:0" data-i18n="classesToday">Classes Today</h3><div id="todayClasses"></div></div>
    <select id="classFilter" onchange="renderAll()"><option value="all" data-i18n="all">All</option><option value="Scheduled" data-i18n="scheduled">Scheduled</option><option value="Completed" data-i18n="completed">Completed</option><option value="Absent" data-i18n="absent">Absent</option><option value="Cancelled" data-i18n="cancelled">Cancelled</option></select>
    <div id="classList"></div>
  </div>

  <!-- 4. LESSONS SYLLABUS -->
  <div id="lessonsTab" class="hidden">
    <select id="catFilter" onchange="renderCatalog()"><option value="all" data-i18n="allLessons">All Lessons</option><option value="Theory" data-i18n="theory">Theory Only</option><option value="Practical" data-i18n="practical">Practical Only</option><option value="Mock" data-i18n="mock">Mock Test Only</option></select>
    <div id="catalogList"></div>
  </div>

  <!-- 5. PAYMENTS -->
  <div id="paymentsTab" class="hidden">
    <div class="card" style="background:#e8f5e9;border:2px solid #1a7a3a"><h3 style="margin:0">💚 <span data-i18n="payNowTitle">Pay Fee - M-Pesa STK Push</span></h3>
      <label class="small" data-i18n="student">Student</label><select id="pStudent" onchange="updatePayFormInfo()"></select><div id="pStudentInfo" class="small"></div>
      <input id="pMpesaPhone" data-ph="mpesaPhone" placeholder="M-Pesa Phone" inputmode="tel">
      <input id="pAmount" data-ph="amount" placeholder="Amount Ksh" type="number" inputmode="numeric">
      <select id="pFor"><option data-i18n="payDeposit">Deposit / Admission Fee</option><option data-i18n="payInstallment">Installment - Paying Balance</option><option data-i18n="payFull">Full Payment - Clear Balance</option><option data-i18n="payTest">NTSA Test Fee</option></select>
      <button class="green" onclick="stkPushPayment()">💚 <span data-i18n="sendStk">Send STK Push</span></button>
      <input id="pCode" data-ph="receipt" placeholder="M-Pesa Code e.g. QK123ABC">
      <select id="pMethod"><option>M-Pesa</option><option>Cash</option><option>Bank</option></select>
      <button class="green" onclick="savePayment()">✅ <span data-i18n="recordPayment">Record Payment</span></button>
    </div>
    <select id="payFilter" onchange="renderAll()"><option value="all" data-i18n="allPayments">All Payments</option><option value="M-Pesa">M-Pesa Only</option><option value="Cash">Cash Only</option><option value="Bank">Bank Only</option></select>
    <div id="paymentList"></div>
    <div id="receiptArea"></div>
  </div>

  <!-- 6. BALANCES -->
  <div id="balancesTab" class="hidden">
    <div class="card" style="background:#e3f2fd"><h3 style="margin:0">⚖️ <span data-i18n="balancesTitle">Balances - Who Owes What?</span></h3><p class="small" data-i18n="balancesHint">Green = Paid ✅ | Orange = Has Balance | Red = Big Balance - Cannot Book Until Paid</p></div>
    <select id="balFilter" onchange="renderAll()"><option value="all" data-i18n="allStudents">All Students</option><option value="paid" data-i18n="paidFull">Paid in Full ✅</option><option value="owing" data-i18n="hasBalance">Has Balance ⚠️</option><option value="big" data-i18n="bigBalance">Big Balance > Ksh 10,000 🔴</option></select>
    <input id="balSearch" data-ph="searchStudent" placeholder="Search..." oninput="renderAll()">
    <div id="balanceList"></div>
  </div>

  <!-- 7. REPORT -->
  <div id="reportTab" class="hidden">
    <div class="card"><h3 style="margin:0">📄 <span data-i18n="schoolReport">School Report</span></h3><input type="month" id="reportMonth"><button class="green" onclick="generateReport()" data-i18n="genReport">Generate Report PDF</button><button class="secondary" onclick="shareReport()" data-i18n="shareWA">Share via WhatsApp</button></div>
    <div id="reportPreview"></div>
  </div>

  <div id="certTab" class="hidden"><div id="certArea"></div></div>
</div>
</main>
<footer>NPS AJIRA DRIVING SCHOOL • NTSA Approved<br><span data-i18n="footer">Learn • Pass • Get Job</span> • 💬 <a href="https://wa.me/c/254777725770" target="_blank">WhatsApp Channel</a></footer>
</div>
<div class="bottom-nav" id="bottomNav" style="display:none">
  <button onclick="showTab('admission')" id="navAdmission"><span>📝</span><span data-i18n="admission">Admission</span></button>
  <button onclick="showTab('students')" id="navStudents"><span>🧑‍🎓</span><span data-i18n="students">Students</span></button>
  <button onclick="showTab('classes')" id="navClasses"><span>📅</span><span data-i18n="classes">Classes</span></button>
  <button onclick="showTab('payments')" id="navPayments"><span>💰</span><span data-i18n="payments">Payments</span></button>
  <button onclick="showTab('balances')" id="navBalances"><span>⚖️</span><span data-i18n="balances">Balances</span></button>
  <button onclick="showTab('report')" id="navReport"><span>📄</span><span data-i18n="report">Report</span></button>
</div>
<script>
let LANG = localStorage.getItem("ajira_lang") || "en";
const I18N={
en:{welcome:"Welcome - Ajira Driving School",iAmStudent:"I am a Student - Admission / Lessons / Payments",iAmInstructor:"I am an Instructor / Admin",roleInstructor:"Instructor",roleAdmin:"Admin",roleOCS:"OCS / MT Officer",login:"Login",loginHint:"Student: Name + Phone only. Instructor Demo: Any name + number.",hello:"Hello",logout:"Logout",students:"Students",classesBooked:"Classes Booked",collected:"Collected",owing:"Still Owing",lessonsDone:"Lessons Completed",passed:"Passed",myAdmission:"My Admission",paid:"Paid",balance:"Balance",lessons:"Lessons",nextClass:"Next Class",admission:"Admission",classes:"Classes",payments:"Payments",balances:"Balances",report:"Report",admissionForm:"Admission Form - New Student",admissionHint:"Fill once. Student gets Admission No, ID, Course, Payment Plan, Class Schedule automatically.",selectCourse:"Select Course *",male:"Male",female:"Female",noLicence:"No Licence - Beginner",haveLicence:"Have Licence - Add Class",expiredLicence:"Licence Expired - Refresher",morning:"Morning - 8am - 11am",midday:"Midday - 11am - 2pm",afternoon:"Afternoon - 2pm - 5pm",weekend:"Weekend Only - Sat / Sun",paymentPlan:"Payment Plan *",planFull:"Pay in Full - Pay Once",plan2:"2 Installments - 50% Now + 50% Later",plan3:"3 Installments - Deposit + 2 Payments",plan4:"4 Installments - Deposit + 3 Payments",payDeposit:"Pay Deposit Now - M-Pesa STK Push",sendStk:"Send STK Push",admitBtn:"Admit Student → Create Admission No.",enrolled:"Enrolled",inTraining:"In Training",readyTest:"Ready for Test",failed:"Failed",dropped:"Dropped",bookClass:"Book a Class",student:"Student",selectLesson:"Select Lesson / Class *",bookClassBtn:"Book Class",classesToday:"Classes Today",all:"All",scheduled:"Scheduled",completed:"Completed",absent:"Absent",cancelled:"Cancelled",allLessons:"All Lessons",theory:"Theory Only",practical:"Practical Only",mock:"Mock Test Only",payNowTitle:"Pay Fee - M-Pesa STK Push",recordPayment:"Record Payment",allPayments:"All Payments",balancesTitle:"Balances - Who Owes What?",balancesHint:"Green = Paid ✅ | Orange = Has Balance | Red = Big Balance - Cannot Book Until Paid",allStudents:"All Students",paidFull:"Paid in Full ✅",hasBalance:"Has Balance ⚠️",bigBalance:"Big Balance > Ksh 10,000 🔴",schoolReport:"School Report",genReport:"Generate Report PDF",shareWA:"Share via WhatsApp",footer:"Learn • Pass • Get Job",payDeposit:"Deposit / Admission Fee",payInstallment:"Installment - Paying Balance",payFull:"Full Payment - Clear Balance",payTest:"NTSA Test Fee",
ph:{fullName:"Full Name *",phone:"Phone e.g. 0712345678",idNo:"ID No.",instructorName:"Instructor / Admin Name",staffNo:"Staff No.",age:"Age",county:"County e.g. Trans Nzoia",education:"Education e.g. KCSE C-",nextKin:"Next of Kin Name + Phone e.g. Mary - 0712345678",address:"Home / Estate e.g. Eldoret - Kapsoya",licenceNo:"Licence No. (If any)",mpesaPhone:"M-Pesa Phone e.g. 0712345678",deposit:"Deposit Ksh e.g. 5000",mpesaCode:"M-Pesa Code e.g. QK123ABC",amount:"Amount Ksh e.g. 5000",receipt:"M-Pesa Code e.g. QK123ABC",searchStudent:"Search name, phone, admission no..."}},
sw:{welcome:"Karibu - Ajira Driving School",iAmStudent:"Mimi ni Mwanafunzi - Admission / Masomo / Malipo",iAmInstructor:"Mimi ni Mwalimu / Admin",roleInstructor:"Mwalimu",roleAdmin:"Admin",roleOCS:"OCS / Afisa MT",login:"Ingia",loginHint:"Mwanafunzi: Jina + Simu tu. Mwalimu Demo: Jina lolote + namba.",hello:"Habari",logout:"Toka",students:"Wanafunzi",classesBooked:"Madarsa Yaliyowekwa",collected:"Zimekusanywa",owing:"Bado Zinadaiwa",lessonsDone:"Masomo Yaliyokwisha",passed:"Wamefaulu",myAdmission:"Admission Yangu",paid:"Amelipa",balance:"Deni",lessons:"Masomo",nextClass:"Darasa Linalofuata",admission:"Admission",classes:"Madarsa",payments:"Malipo",balances:"Madeni",report:"Ripoti",admissionForm:"Fomu ya Admission - Mwanafunzi Mpya",admissionHint:"Jaza mara moja. Mwanafunzi anapata Admission No, ID, Kozi, Mpango wa Malipo, Ratiba ya Darasa yenyewe.",selectCourse:"Chagua Kozi *",male:"Kiume",female:"Kike",noLicence:"Sina Leseni - Mgeni",haveLicence:"Nina Leseni - Ongeza Class",expiredLicence:"Leseni Ime-expire - Refresher",morning:"Asubuhi - 8am - 11am",midday:"Mchana - 11am - 2pm",afternoon:"Jioni - 2pm - 5pm",weekend:"Weekend Tu - Sat / Sun",paymentPlan:"Mpango wa Malipo *",planFull:"Lipa Yote Mara Moja",plan2:"Awamu 2 - 50% Sasa + 50% Baadaye",plan3:"Awamu 3 - Deposit + Malipo 2",plan4:"Awamu 4 - Deposit + Malipo 3",payDeposit:"Lipa Deposit Sasa - M-Pesa STK Push",sendStk:"Tuma STK Push",admitBtn:"Mwandikishe → Tengeneza Admission No.",enrolled:"Amejiandikisha",inTraining:"Mafunzoni",readyTest:"Tayari kwa Mtihani",failed:"Amefail",dropped:"Ameacha",bookClass:"Weka Nafasi ya Darasa",student:"Mwanafunzi",selectLesson:"Chagua Somo / Darasa *",bookClassBtn:"Weka Nafasi ya Darasa",classesToday:"Madarsa ya Leo",all:"Yote",scheduled:"Yamepangwa",completed:"Yamekwisha",absent:"Hayupo",cancelled:"Yameghairiwa",allLessons:"Masomo Yote",theory:"Theory Tu",practical:"Practical Tu",mock:"Mock Test Tu",payNowTitle:"Lipa Ada - M-Pesa STK Push",recordPayment:"Rekodi Malipo",allPayments:"Malipo Yote",balancesTitle:"Madeni - Nani Anadaiwa Nini?",balancesHint:"Kijani = Amelipa ✅ | Machungwa = Ana Deni | Nyekundu = Deni Kubwa - Hawezi Kuweka Darasa Mpaka Alipe",allStudents:"Wanafunzi Wote",paidFull:"Amelipa Yote ✅",hasBalance:"Ana Deni ⚠️",bigBalance:"Deni Kubwa > Ksh 10,000 🔴",schoolReport:"Ripoti ya Shule",genReport:"Tengeneza Ripoti PDF",shareWA:"Share kupitia WhatsApp",footer:"Jifunze • Faulu • Pata Kazi",payDeposit:"Deposit / Ada ya Admission",payInstallment:"Installment - Kulipa Deni",payFull:"Malipo Kamili - Maliza Deni",payTest:"Ada ya Mtihani wa NTSA",
ph:{fullName:"Jina Kamili *",phone:"Simu e.g. 0712345678",idNo:"Namba ya ID",instructorName:"Jina la Mwalimu / Admin",staffNo:"Namba ya Staff",age:"Umri",county:"County e.g. Trans Nzoia",education:"Elimu e.g. KCSE C-",nextKin:"Ndugu wa Karibu Jina + Simu e.g. Mary - 0712345678",address:"Nyumbani / Estate e.g. Eldoret - Kapsoya",licenceNo:"Namba ya Leseni (Kama unayo)",mpesaPhone:"Simu ya M-Pesa e.g. 0712345678",deposit:"Deposit Ksh e.g. 5000",mpesaCode:"M-Pesa Code e.g. QK123ABC",amount:"Kiasi Ksh e.g. 5000",receipt:"M-Pesa Code e.g. QK123ABC",searchStudent:"Tafuta jina, simu, admission no..."}}
};
function setLang(l){ LANG=l; localStorage.setItem("ajira_lang",l); document.getElementById("btnEN").classList.toggle("active",l==="en"); document.getElementById("btnSW").classList.toggle("active",l==="sw"); applyLang(); renderAll(); }
function applyLang(){ let d=I18N[LANG]; document.querySelectorAll("[data-i18n]").forEach(el=>{let k=el.getAttribute("data-i18n"); if(d[k]) el.innerHTML=d[k];}); document.querySelectorAll("[data-ph]").forEach(el=>{let k=el.getAttribute("data-ph"); if(d.ph[k]) el.placeholder=d.ph[k];}); }
function t(en,sw){ return LANG==="sw"?sw:en; }
let courses = JSON.parse(localStorage.getItem("ajira_ds_courses")||"[]");
let students = JSON.parse(localStorage.getItem("ajira_ds_students")||"[]");
let classes = JSON.parse(localStorage.getItem("ajira_ds_classes")||"[]");
let payments = JSON.parse(localStorage.getItem("ajira_ds_payments")||"[]");
let currentUser=null, isAdmin=false;
function getToday(){ return new Date().toISOString().slice(0,10); }
function getCurrentMonth(){ return new Date().toISOString().slice(0,7); }
function getBal(s){ return Math.max(0, s.coursePrice - (s.totalPaid||0)); }
function getPct(s){ return s.coursePrice?Math.round((s.totalPaid||0)/s.coursePrice*100):0; }
function genAdmissionNo(){ let n=students.length+1; return "ADS-"+String(n).padStart(4,"0")+"-"+new Date().getFullYear(); }
const SYLLABUS=[
{id:1,no:"L1",type:"Theory",titleEN:"Intro to Driving & Road Safety",titleSW:"Utangulizi wa Udereva & Usalama",descEN:"Car parts, dashboard, seatbelt, mirrors.",descSW:"Sehemu za gari, dashboard, seatbelt, vioo.",duration:"1 hr"},
{id:2,no:"L2",type:"Theory",titleEN:"Traffic Rules & Highway Code",titleSW:"Sheria za Barabara & Highway Code",descEN:"Speed limits, right of way.",descSW:"Kikomo cha kasi, kipaumbele.",duration:"1.5 hrs"},
{id:3,no:"L3",type:"Theory",titleEN:"Road Signs - All Signs",titleSW:"Alama za Barabara - Zote",descEN:"100+ signs, NTSA focus.",descSW:"Alama 100+, NTSA.",duration:"1.5 hrs"},
{id:4,no:"L4",type:"Theory",titleEN:"Defensive Driving & Hazard",titleSW:"Defensive & Hatari",descEN:"Anticipating others.",descSW:"Kutarajia wengine.",duration:"1 hr"},
{id:5,no:"L5",type:"Practical",titleEN:"Car Controls - Start, Stop, Clutch",titleSW:"Kudhibiti Gari - Kuanza, Kusimama",descEN:"Yard only, clutch + brake.",descSW:"Yard tu, clutch + breki.",duration:"1 hr"},
{id:6,no:"L6",type:"Practical",titleEN:"Moving Off, Gear 1-2-3",titleSW:"Kuanza Safari, Gear 1-2-3",descEN:"Smooth start.",descSW:"Kuanza laini.",duration:"1 hr"},
{id:7,no:"L7",type:"Practical",titleEN:"Steering, Turning Left & Right",titleSW:"Usukani, Kugeuka",descEN:"Mirror - Signal - Blind Spot.",descSW:"Kioo - Ishara - Blind Spot.",duration:"1 hr"},
{id:8,no:"L8",type:"Practical",titleEN:"Parking - Bay & Parallel",titleSW:"Parking - Bay & Parallel",descEN:"Hardest NTSA part.",descSW:"Ngumu zaidi ya NTSA.",duration:"1.5 hrs"},
{id:9,no:"L9",type:"Practical",titleEN:"Reverse Parking",titleSW:"Reverse Parking",descEN:"Reverse, observation.",descSW:"Kurudi nyuma.",duration:"1 hr"},
{id:10,no:"L10",type:"Practical",titleEN:"Roundabout & Town Driving",titleSW:"Roundabout & Mjini",descEN:"Eldoret town.",descSW:"Mji wa Eldoret.",duration:"1.5 hrs"},
{id:11,no:"L11",type:"Practical",titleEN:"Highway - Speed, Overtaking",titleSW:"Highway - Kasi, Kupita",descEN:"Highway to Kitale.",descSW:"Highway Kitale.",duration:"2 hrs"},
{id:12,no:"L12",type:"Practical",titleEN:"Hill Start",titleSW:"Kuanza Mlimani",descEN:"Handbrake start.",descSW:"Handbrake.",duration:"1 hr"},
{id:13,no:"L13",type:"Practical",titleEN:"Night Driving & Bad Weather",titleSW:"Usiku & Hali Mbaya",descEN:"Lights, rain, fog.",descSW:"Taa, mvua.",duration:"1 hr"},
{id:14,no:"L14",type:"Practical",titleEN:"Emergency Stop & Hazard",titleSW:"Dharura & Hazard",descEN:"Emergency brake.",descSW:"Breki ya dharura.",duration:"1 hr"},
{id:15,no:"L15",type:"Theory",titleEN:"Vehicle Maintenance",titleSW:"Matunzo ya Gari",descEN:"Tyres, oil, water.",descSW:"Matairi, mafuta.",duration:"1 hr"},
{id:16,no:"L16",type:"Theory",titleEN:"NTSA Test - What Examiners Look For",titleSW:"NTSA - Wanaangalia Nini",descEN:"Mistakes that fail.",descSW:"Makosa yanayofelisha.",duration:"1 hr"},
{id:17,no:"L17",type:"Mock",titleEN:"Mock Test 1 - Full NTSA Simulation",titleSW:"Mock 1 - Kama NTSA",descEN:"Full test.",descSW:"Mtihani kamili.",duration:"2 hrs"},
{id:18,no:"L18",type:"Mock",titleEN:"Mock Test 2 - Fix Weak Areas",titleSW:"Mock 2 - Rekebisha Dhaifu",descEN:"Focus on Mock 1.",descSW:"Mock 1.",duration:"2 hrs"},
{id:19,no:"L19",type:"Practical",titleEN:"Final Polish",titleSW:"Kumalizia",descEN:"Last practice.",descSW:"Mazoezi ya mwisho.",duration:"2 hrs"},
{id:20,no:"L20",type:"Mock",titleEN:"Final Assessment - Ready for NTSA?",titleSW:"Tathmini ya Mwisho",descEN:"Ready or more practice.",descSW:"Tayari au mazoezi.",duration:"1 hr"},
];
function toggleLogin(){ let tt=document.getElementById("userType").value; document.getElementById("studentLogin").classList.toggle("hidden", tt!=="student"); document.getElementById("instructorLogin").classList.toggle("hidden", tt!=="student"); }
function login(){
  let type=document.getElementById("userType").value;
  if(type==="student"){ let name=document.getElementById("stuName").value.trim(); let phone=document.getElementById("stuPhone").value.trim(); let id=document.getElementById("stuId").value.trim(); if(!name||!phone) return alert(t("Enter Name and Phone","Jaza Jina na Simu")); currentUser={name,phone,id,role:t("Student","Mwanafunzi")}; isAdmin=false; }
  else { let name=document.getElementById("offName").value.trim(); let no=document.getElementById("offNo").value.trim(); let role=document.getElementById("offRole").value; if(!name||!no) return alert(t("Enter Name and Staff No.","Jaza Jina na Staff No.")); currentUser={name,no,role,station:"Ajira Driving School - Eldoret"}; isAdmin=true; }
  document.getElementById("loginView").classList.add("hidden"); document.getElementById("appView").classList.remove("hidden"); document.getElementById("bottomNav").style.display="flex";
  document.getElementById("userName").innerText=currentUser.name+" ("+currentUser.role+")"; document.getElementById("stationLabel").innerText=currentUser.station||t("Student","Mwanafunzi"); document.getElementById("dateLabel").innerText=new Date().toLocaleDateString();
  if(courses.length===0){
    courses=[{id:1,title:t("Class B - Small Car / Probox","Class B - Gari Ndogo / Probox"),price:18000,duration:t("4 Weeks / 20 Lessons","Wiki 4 / Masomo 20"),instructor:"Instr. David Otieno",vehicle:"KDJ 123A - Probox",desc:t("Theory + Practical, Parking, Town, NTSA.","Theory + Practical, Parking, Town, NTSA."),createdAt:new Date().toISOString()},{id:2,title:t("Class C - Lorry","Class C - Lorry"),price:25000,duration:t("5 Weeks / 25 Lessons","Wiki 5 / Masomo 25"),instructor:"Instr. Peter Kamau",vehicle:"KDJ 456B - Lorry",desc:"Lorry, Reversing, Highway.",createdAt:new Date().toISOString()},{id:3,title:t("Class D - Bus / PSV","Class D - Bus / PSV"),price:28000,duration:t("6 Weeks / 30 Lessons","Wiki 6 / Masomo 30"),instructor:"Instr. Jane Wanjiru",vehicle:"KDJ 789C - Bus",desc:"Bus + PSV.",createdAt:new Date().toISOString()},{id:4,title:t("Class A - Motorcycle","Class A - Pikipiki"),price:12000,duration:t("3 Weeks / 15 Lessons","Wiki 3 / Masomo 15"),instructor:"Instr. Mary Achieng",vehicle:"KMDA 101 - Honda",desc:"Motorcycle.",createdAt:new Date().toISOString()},{id:5,title:t("Class B+C - Car + Lorry","Class B+C - Gari + Lorry"),price:35000,duration:t("8 Weeks / 40 Lessons","Wiki 8 / Masomo 40"),instructor:"Instr. David Otieno",vehicle:"KDJ 123A + KDJ 456B",desc:t("Best for NPS Jobs!","Best kwa Ajira NPS!"),createdAt:new Date().toISOString()},{id:6,title:t("Defensive Driving","Defensive Driving"),price:15000,duration:t("2 Weeks / 10 Lessons","Wiki 2 / Masomo 10"),instructor:"Instr. Peter Kamau",vehicle:"KDJ 123A",desc:"Defensive.",createdAt:new Date().toISOString()}];
    localStorage.setItem("ajira_ds_courses",JSON.stringify(courses));
    students=[
      {id:1,admissionNo:"ADS-0001-2026",name:"John Kiprop",phone:"0711111111",idNo:"40111111",age:24,gender:t("Male","Kiume"),county:"Trans Nzoia",education:"KCSE C-",nextKin:"Mary Kiprop - 0710000000",address:"Eldoret - Kapsoya",courseId:1,courseTitle:courses[0].title,coursePrice:18000,hasLicence:t("No Licence - Beginner","Sina Leseni - Mgeni"),licenceNo:"",schedule:t("Morning - 8am - 11am","Asubuhi - 8am - 11am"),plan:"3 Installments",status:"In Training",lessonsDone:8,totalPaid:12000,officer:"Admin",createdAt:new Date().toISOString(),day:getToday()},
      {id:2,admissionNo:"ADS-0002-2026",name:"Faith Chebet",phone:"0722222222",idNo:"40222222",age:22,gender:t("Female","Kike"),county:"Uasin Gishu",education:"KCSE C",nextKin:"Peter Chebet - 0720000000",address:"Eldoret - Pioneer",courseId:5,courseTitle:courses[4].title,coursePrice:35000,hasLicence:t("No Licence - Beginner","Sina Leseni - Mgeni"),licenceNo:"",schedule:t("Midday - 11am - 2pm","Mchana - 11am - 2pm"),plan:"2 Installments",status:"Ready for Test",lessonsDone:18,totalPaid:35000,officer:"Admin",createdAt:new Date().toISOString(),day:getToday()},
      {id:3,admissionNo:"ADS-0003-2026",name:"Kevin Barasa",phone:"0733333333",idNo:"40333333",age:28,gender:t("Male","Kiume"),county:"Bungoma",education:"KCSE C-",nextKin:"Jane Barasa - 0730000000",address:"Kitale - Town",courseId:2,courseTitle:courses[1].title,coursePrice:25000,hasLicence:t("Have Licence - Add Class","Nina Leseni - Ongeza Class"),licenceNo:"DL999111",schedule:t("Afternoon - 2pm - 5pm","Jioni - 2pm - 5pm"),plan:"Pay in Full",status:"Passed",lessonsDone:20,totalPaid:25000,officer:"Admin",createdAt:new Date().toISOString(),day:getToday()},
      {id:4,admissionNo:"ADS-0004-2026",name:"Grace Wanjiku",phone:"0744444444",idNo:"40444444",age:21,gender:t("Female","Kike"),county:"Uasin Gishu",education:"KCSE C+",nextKin:"John Wanjiku - 0740000000",address:"Eldoret - Langas",courseId:1,courseTitle:courses[0].title,coursePrice:18000,hasLicence:t("No Licence - Beginner","Sina Leseni - Mgeni"),licenceNo:"",schedule:t("Morning - 8am - 11am","Asubuhi - 8am - 11am"),plan:"4 Installments",status:"Enrolled",lessonsDone:2,totalPaid:5000,officer:"Admin",createdAt:new Date().toISOString(),day:getToday()},
    ]; localStorage.setItem("ajira_ds_students",JSON.stringify(students));
    payments=[
      {id:1,studentId:1,admissionNo:"ADS-0001-2026",name:"John Kiprop",amount:5000,method:"M-Pesa",code:"QK111AAA",for:t("Deposit / Admission Fee","Deposit / Ada ya Admission"),date:getToday(),officer:"Admin"},
      {id:2,studentId:1,admissionNo:"ADS-0001-2026",name:"John Kiprop",amount:7000,method:"M-Pesa",code:"QK222BBB",for:t("Installment - Paying Balance","Installment - Kulipa Deni"),date:getToday(),officer:"Admin"},
      {id:3,studentId:2,admissionNo:"ADS-0002-2026",name:"Faith Chebet",amount:17500,method:"M-Pesa",code:"QK333CCC",for:t("Deposit / Admission Fee","Deposit / Ada ya Admission"),date:getToday(),officer:"Admin"},
      {id:4,studentId:2,admissionNo:"ADS-0002-2026",name:"Faith Chebet",amount:17500,method:"Cash",code:"REC002",for:t("Full Payment - Clear Balance","Malipo Kamili - Maliza Deni"),date:getToday(),officer:"Admin"},
      {id:5,studentId:3,admissionNo:"ADS-0003-2026",name:"Kevin Barasa",amount:25000,method:"Cash",code:"REC001",for:t("Full Payment - Clear Balance","Malipo Kamili - Maliza Deni"),date:getToday(),officer:"Admin"},
      {id:6,studentId:4,admissionNo:"ADS-0004-2026",name:"Grace Wanjiku",amount:5000,method:"M-Pesa",code:"QK444DDD",for:t("Deposit / Admission Fee","Deposit / Ada ya Admission"),date:getToday(),officer:"Admin"},
    ]; localStorage.setItem("ajira_ds_payments",JSON.stringify(payments));
    classes=[
      {id:101,studentId:1,admissionNo:"ADS-0001-2026",name:"John Kiprop",phone:"0711111111",syllabusId:9,title:t("Parking - Bay & Parallel","Parking - Bay & Parallel"),type:"Practical",date:getToday(),time:"09:00",instructor:"Instr. David Otieno",vehicle:"KDJ 123A - Probox",location:"Eldoret - Yard",slot:t("Morning - 8am - 11am","Asubuhi - 8am - 11am"),status:"Scheduled",officer:"Admin",createdAt:new Date().toISOString()},
      {id:102,studentId:2,admissionNo:"ADS-0002-2026",name:"Faith Chebet",phone:"0722222222",syllabusId:17,title:t("Mock Test 1 - Full NTSA Simulation","Mock 1 - Kama NTSA"),type:"Mock",date:getToday(),time:"11:30",instructor:"Instr. David Otieno",vehicle:"KDJ 123A + KDJ 456B",location:"Eldoret - Town",slot:t("Midday - 11am - 2pm","Mchana - 11am - 2pm"),status:"Scheduled",officer:"Admin",createdAt:new Date().toISOString()},
      {id:103,studentId:4,admissionNo:"ADS-0004-2026",name:"Grace Wanjiku",phone:"0744444444",syllabusId:5,title:t("Car Controls - Start, Stop, Clutch","Kudhibiti Gari - Kuanza, Kusimama"),type:"Practical",date:getToday(),time:"08:00",instructor:"Instr. David Otieno",vehicle:"KDJ 123A - Probox",location:"Eldoret - Yard",slot:t("Morning - 8am - 11am","Asubuhi - 8am - 11am"),status:"Scheduled",officer:"Admin",createdAt:new Date().toISOString()},
      {id:104,studentId:1,admissionNo:"ADS-0001-2026",name:"John Kiprop",phone:"0711111111",syllabusId:8,title:t("Parking - Bay & Parallel","Parking - Bay & Parallel"),type:"Practical",date:"2026-11-22",time:"09:00",instructor:"Instr. David Otieno",vehicle:"KDJ 123A - Probox",location:"Eldoret - Yard",slot:"Morning",status:"Completed",officer:"Admin",createdAt:new Date().toISOString()},
    ]; localStorage.setItem("ajira_ds_classes",JSON.stringify(classes));
  }
  if(!isAdmin){ document.getElementById("aName").value=currentUser.name; document.getElementById("aPhone").value=currentUser.phone; document.getElementById("aId").value=currentUser.id||""; document.getElementById("aMpesaPhone").value=currentUser.phone; }
  if(document.getElementById("reportMonth")) document.getElementById("reportMonth").value=getCurrentMonth();
  applyLang(); renderAll(); renderCatalog();
}
function logout(){ location.reload(); }
function showTab(tt){
  ["admission","students","classes","lessons","payments","balances","report","cert"].forEach(k=>{let el=document.getElementById(k+"Tab"); if(el) el.classList.toggle("hidden",k!==tt);});
  ["Admission","Students","Classes","Lessons","Payments","Balances","Report"].forEach(k=>{let el=document.getElementById("tab"+k); if(el) el.classList.toggle("active",k.toLowerCase()===tt);});
  ["Admission","Students","Classes","Payments","Balances","Report"].forEach(k=>{let el=document.getElementById("nav"+k); if(el) el.classList.toggle("active",k.toLowerCase()===tt);});
  renderAll(); window.scrollTo({top:0,behavior:"smooth"});
}
// ADMISSION
function updateAdmissionInfo(){ let id=document.getElementById("aCourse").value; let c=courses.find(x=>x.id==id); if(!c) return; document.getElementById("aCourseInfo").innerHTML=`<b>${c.title}</b><br>${t("Fee:","Ada:")} <b>Ksh ${c.price.toLocaleString()}</b> • ${c.duration}<br>${t("Instructor:","Mwalimu:")} ${c.instructor} • ${t("Vehicle:","Gari:")} ${c.vehicle}`; let plan=document.getElementById("aPlan").value; let deposit=plan==="full"?c.price:plan==="2"?Math.round(c.price/2):plan==="3"?Math.round(c.price/3):5000; document.getElementById("aPlanInfo").innerHTML=`${t("Plan:","Mpango:")} ${document.getElementById("aPlan").options[document.getElementById("aPlan").selectedIndex].text}<br>${t("Suggested Deposit:","Deposit Inayopendekezwa:")} <b>Ksh ${deposit.toLocaleString()}</b> • ${t("Admission No will be:","Admission No itakuwa:")} <b>${genAdmissionNo()}</b>`; if(!document.getElementById("aDeposit").value) document.getElementById("aDeposit").value=deposit; }
function stkAdmission(){ let phone=document.getElementById("aMpesaPhone").value.trim(); let amount=parseInt(document.getElementById("aDeposit").value||0); if(!phone||!amount) return alert(t("Enter M-Pesa Phone and Deposit","Weka Simu ya M-Pesa na Deposit")); let btn=event.target; btn.innerText=t("⏳ Sending STK Push...","⏳ Tumatuma STK Push..."); btn.disabled=true; setTimeout(()=>{ btn.innerText="💚 "+t("Send STK Push","Tuma STK Push"); btn.disabled=false; let code="QK"+Math.random().toString(36).substring(2,8).toUpperCase(); document.getElementById("aMpesaCode").value=code; alert(t(`💚 STK PUSH SENT!\nPhone: ${phone}\nDeposit: Ksh ${amount.toLocaleString()}\nCode: ${code}\n\nEnter PIN, then tap Admit Student.`,`💚 STK PUSH IMETUMWA!\nSimu: ${phone}\nDeposit: Ksh ${amount.toLocaleString()}\nCode: ${code}\n\nWeka PIN, kisha bonyeza Mwandikishe.`)); },1200); }
function admitStudent(){
  let courseId=document.getElementById("aCourse").value; let name=document.getElementById("aName").value.trim(); let phone=document.getElementById("aPhone").value.trim(); let idNo=document.getElementById("aId").value.trim(); let age=document.getElementById("aAge").value; let gender=document.getElementById("aGender").value; let county=document.getElementById("aCounty").value.trim(); let edu=document.getElementById("aEducation").value.trim(); let nextKin=document.getElementById("aNextKin").value.trim(); let address=document.getElementById("aAddress").value.trim(); let hasLic=document.getElementById("aHasLicence").value; let licNo=document.getElementById("aLicenceNo").value.trim(); let schedule=document.getElementById("aSchedule").value; let plan=document.getElementById("aPlan").options[document.getElementById("aPlan").selectedIndex].text; let deposit=parseInt(document.getElementById("aDeposit").value||0); let mpesa=document.getElementById("aMpesaCode").value.trim();
  if(!courseId||!name||!phone||!idNo) return alert(t("Enter Course, Name, Phone, ID","Jaza Kozi, Jina, Simu, ID"));
  let course=courses.find(x=>x.id==courseId);
  if(students.find(s=>s.phone===phone && s.courseId==courseId)) return alert(t("Already admitted in this course!","Ameshaandikishwa kwenye kozi hii!"));
  let admissionNo=genAdmissionNo();
  let stu={id:Date.now(),admissionNo,name,phone,idNo,age,gender,county,education:edu,nextKin,address,courseId:parseInt(courseId),courseTitle:course.title,coursePrice:course.price,hasLicence:hasLic,licenceNo:licNo,schedule,plan,status:"Enrolled",lessonsDone:0,totalPaid:deposit,officer:currentUser.name,createdAt:new Date().toISOString(),day:getToday()};
  students.unshift(stu); localStorage.setItem("ajira_ds_students",JSON.stringify(students));
  if(deposit>0){ payments.unshift({id:Date.now()+1,studentId:stu.id,admissionNo,name,amount:deposit,method:"M-Pesa",code:mpesa||"DEPOSIT",for:t("Deposit / Admission Fee","Deposit / Ada ya Admission"),date:getToday(),officer:currentUser.name}); localStorage.setItem("ajira_ds_payments",JSON.stringify(payments)); }
  let bal=course.price-deposit;
  document.getElementById("admissionSuccess").innerHTML=`<div class="card" style="background:#e8f5e9;border:2px solid #1a7a3a"><h3>🎉 ${t("ADMITTED!","AMEANDIKISHWA!")}</h3><p><b>${name}</b><br>${t("Admission No:","Admission No:")} <b>${admissionNo}</b><br>${t("Course:","Kozi:")} ${course.title}<br>${t("Fee:","Ada:")} Ksh ${course.price.toLocaleString()} • ${t("Paid:","Amelipa:")} Ksh ${deposit.toLocaleString()} • ${t("Balance:","Deni:")} Ksh ${bal.toLocaleString()}<br>${t("Plan:","Mpango:")} ${plan}<br>${t("Schedule:","Ratiba:")} ${schedule}</p><button class="green" onclick="bookClassFor(${stu.id})">📅 ${t("Book First Class Now","Weka Darasa la Kwanza Sasa")}</button><button class="secondary" onclick="shareAdmission('${name}','${admissionNo}','${course.title}',${bal})">${t("Share Admission WhatsApp","Share Admission WhatsApp")}</button><button class="secondary" onclick="printAdmission('${admissionNo}')">🖨️ ${t("Print Admission Letter","Print Barua ya Admission")}</button></div>`;
  alert(t(`✅ ADMITTED!\n${name}\nAdmission No: ${admissionNo}\nCourse: ${course.title}\nFee: Ksh ${course.price.toLocaleString()}\nPaid: Ksh ${deposit.toLocaleString()}\nBalance: Ksh ${bal.toLocaleString()}`,`✅ AMEANDIKISHWA!\n${name}\nAdmission No: ${admissionNo}\nKozi: ${course.title}\nAda: Ksh ${course.price.toLocaleString()}\nAmelipa: Ksh ${deposit.toLocaleString()}\nDeni: Ksh ${bal.toLocaleString()}`));
  showTab('students'); renderAll();
}
function shareAdmission(name,adm,course,bal){ let txt=t(`🎉 ADMISSION - Ajira Driving School\n\nCongratulations ${name}!\nYou are admitted.\nAdmission No: ${adm}\nCourse: ${course}\nBalance: Ksh ${bal.toLocaleString()}\n\nWelcome! Your first class will be scheduled soon.\nWhatsApp Channel: https://wa.me/c/254777725770`,`🎉 ADMISSION - Ajira Driving School\n\nHongera ${name}!\nUmeandikishwa.\nAdmission No: ${adm}\nKozi: ${course}\nDeni: Ksh ${bal.toLocaleString()}\n\nKaribu! Darasa lako la kwanza litapangwa hivi karibuni.\nWhatsApp Channel: https://wa.me/c/254777725770`); window.open("https://wa.me/?text="+encodeURIComponent(txt),"_blank"); }
function printAdmission(adm){ let s=students.find(x=>x.admissionNo===adm); if(!s) return; let w=window.open("","_blank"); w.document.write(`<html><body style="font-family:Arial;padding:20px"><div style="border:3px double #0b2c4a;padding:20px;text-align:center"><div>🇰🇪 NPS AJIRA DRIVING SCHOOL</div><h2>ADMISSION LETTER</h2><p>Dear ${s.name},</p><p>You are admitted to ${s.courseTitle}.</p><p>Admission No: <b>${s.admissionNo}</b><br>ID No: ${s.idNo} • Phone: ${s.phone}<br>Fee: Ksh ${s.coursePrice.toLocaleString()} • Paid: Ksh ${(s.totalPaid||0).toLocaleString()} • Balance: Ksh ${getBal(s).toLocaleString()}<br>Schedule: ${s.schedule} • Plan: ${s.plan}<br>Date: ${getToday()}</p><p>Welcome! Report for your first class.</p><p>Admin: ______________ Stamp: ______________</p></div><script>window.onload=()=>window.print()<\/script></body></html>`); w.document.close(); }
function bookClassFor(id){ showTab('classes'); document.getElementById("cStudent").value=id; updateClassPayInfo(); }
// CLASSES BOOKED
function updateClassInfo(){ let id=document.getElementById("cLesson").value; let s=SYLLABUS.find(x=>x.id==id); if(!s) return; document.getElementById("cLessonInfo").innerHTML=`<b>${LANG==="sw"?s.titleSW:s.titleEN}</b><br>${LANG==="sw"?s.descSW:s.descEN}<br>${t("Duration:","Muda:")} ${s.duration} • ${s.type}`; }
function updateClassPayInfo(){ let id=document.getElementById("cStudent").value; let s=students.find(x=>x.id==id); if(!s) return; let bal=getBal(s); document.getElementById("cStudentInfo").innerHTML=`<b>${s.name} - ${s.admissionNo}</b> - ${s.courseTitle}<br>${t("Paid:","Amelipa:")} Ksh ${(s.totalPaid||0).toLocaleString()} / Ksh ${s.coursePrice.toLocaleString()} • ${t("Balance:","Deni:")} <b style="color:${bal===0?"#1a7a3a":"#b71c1c"}">Ksh ${bal.toLocaleString()}</b> • ${t("Lessons:","Masomo:")} ${s.lessonsDone||0}/20`; }
function bookClass(){
  let stuId=document.getElementById("cStudent").value; let syllabusId=document.getElementById("cLesson").value; let date=document.getElementById("cDate").value; let time=document.getElementById("cTime").value; let instructor=document.getElementById("cInstructor").value; let vehicle=document.getElementById("cVehicle").value; let loc=document.getElementById("cLocation").value; let slot=document.getElementById("cSlot").value;
  if(!stuId||!syllabusId||!date) return alert(t("Select Student, Lesson and Date","Chagua Mwanafunzi, Somo na Tarehe"));
  let stu=students.find(x=>x.id==stuId); let bal=getBal(stu);
  if(bal>10000 && (stu.lessonsDone||0)>=5){ if(!confirm(t(`⚠️ ${stu.name} has BIG BALANCE Ksh ${bal.toLocaleString()}. Cannot book until balance below 10,000. Pay now?`,`⚠️ ${stu.name} ana DENI KUBWA Ksh ${bal.toLocaleString()}. Hawezi kuweka darasa mpaka deni liwe chini ya 10,000. Lipa sasa?`))) return; showTab('payments'); document.getElementById("pStudent").value=stuId; updatePayFormInfo(); return; }
  let clash=classes.find(l=>l.vehicle===vehicle && l.date===date && l.time===time && l.status==="Scheduled");
  if(clash) return alert(t(`Vehicle ${vehicle} already booked at ${time} on ${date} for ${clash.name}.`,`Gari ${vehicle} limeshawekewa nafasi saa ${time} tarehe ${date} kwa ${clash.name}.`));
  let s=SYLLABUS.find(x=>x.id==syllabusId);
  classes.unshift({id:Date.now(),studentId:stu.id,admissionNo:stu.admissionNo,name:stu.name,phone:stu.phone,syllabusId:parseInt(syllabusId),title:LANG==="sw"?s.titleSW:s.titleEN,type:s.type,date,time,instructor,vehicle,location:loc,slot,status:"Scheduled",officer:currentUser.name,createdAt:new Date().toISOString()});
  localStorage.setItem("ajira_ds_classes",JSON.stringify(classes));
  alert(t(`✅ Class Booked!\n${stu.name} (${stu.admissionNo})\n${LANG==="sw"?s.titleSW:s.titleEN}\n${date} ${time}\nVehicle: ${vehicle}\nBalance: Ksh ${bal.toLocaleString()}`,`✅ Darasa Limewekewa Nafasi!\n${stu.name} (${stu.admissionNo})\n${LANG==="sw"?s.titleSW:s.titleEN}\n${date} ${time}\nGari: ${vehicle}\nDeni: Ksh ${bal.toLocaleString()}`));
  renderAll();
}
function markClass(id,status){ if(!isAdmin) return alert(t("Instructor only","Mwalimu tu")); let l=classes.find(x=>x.id===id); if(!l) return; l.status=status; localStorage.setItem("ajira_ds_classes",JSON.stringify(classes)); let stu=students.find(x=>x.id===l.studentId); if(status==="Completed" && stu){ stu.lessonsDone=(stu.lessonsDone||0)+1; if(stu.status==="Enrolled") stu.status="In Training"; if(stu.lessonsDone>=18) stu.status="Ready for Test"; localStorage.setItem("ajira_ds_students",JSON.stringify(students)); } alert(t(`${l.name} - ${l.title} - ${status}`,`${l.name} - ${l.title} - ${status}`)); renderAll(); }
function cancelClass(id){ let l=classes.find(x=>x.id===id); if(!l) return; if(!confirm(t("Cancel this class?","Ghairi darasa hili?"))) return; l.status="Cancelled"; localStorage.setItem("ajira_ds_classes",JSON.stringify(classes)); renderAll(); }
function changeStudentStatus(id,status){ if(!isAdmin) return alert(t("Instructor only","Mwalimu tu")); let s=students.find(x=>x.id===id); if(!s) return; s.status=status; localStorage.setItem("ajira_ds_students",JSON.stringify(students)); alert(`${s.name} - ${status}`); renderAll(); }
// PAYMENTS
function stkPushPayment(){ let stuId=document.getElementById("pStudent").value; let phone=document.getElementById("pMpesaPhone").value.trim(); let amount=parseInt(document.getElementById("pAmount").value||0); let purpose=document.getElementById("pFor").value; if(!stuId||!phone||!amount) return alert(t("Select Student, Enter Phone and Amount","Chagua Mwanafunzi, Weka Simu na Kiasi")); let s=students.find(x=>x.id==stuId); let btn=event.target; btn.innerText=t("⏳ Sending STK Push...","⏳ Tumatuma STK Push..."); btn.disabled=true; setTimeout(()=>{ btn.innerText="💚 "+t("Send STK Push","Tuma STK Push"); btn.disabled=false; let code="QK"+Math.random().toString(36).substring(2,8).toUpperCase(); document.getElementById("pCode").value=code; alert(t(`💚 STK PUSH SENT!\nStudent: ${s.name}\nAmount: Ksh ${amount.toLocaleString()}\nFor: ${purpose}\nCode: ${code}`,`💚 STK PUSH IMETUMWA!\nMwanafunzi: ${s.name}\nKiasi: Ksh ${amount.toLocaleString()}\nKwa: ${purpose}\nCode: ${code}`)); },1200); }
function savePayment(){ let stuId=document.getElementById("pStudent").value; let amount=parseInt(document.getElementById("pAmount").value||0); let method=document.getElementById("pMethod").value; let code=document.getElementById("pCode").value.trim(); let purpose=document.getElementById("pFor").value; if(!stuId||!amount) return alert(t("Select Student and Amount","Chagua Mwanafunzi na Kiasi")); let s=students.find(x=>x.id==stuId); let before=getBal(s); payments.unshift({id:Date.now(),studentId:s.id,admissionNo:s.admissionNo,name:s.name,amount,method,code:code||"CASH",for:purpose,date:getToday(),officer:currentUser.name}); localStorage.setItem("ajira_ds_payments",JSON.stringify(payments)); s.totalPaid=(s.totalPaid||0)+amount; localStorage.setItem("ajira_ds_students",JSON.stringify(students)); let after=getBal(s); document.getElementById("pAmount").value=""; document.getElementById("pCode").value=""; showReceipt(s,amount,method,code||"CASH",purpose,before,after); alert(t(`✅ Payment Recorded! ${s.name} - Ksh ${amount.toLocaleString()}\nBalance: Ksh ${after.toLocaleString()}`,`✅ Malipo Yamehifadhiwa! ${s.name} - Ksh ${amount.toLocaleString()}\nDeni: Ksh ${after.toLocaleString()}`)); renderAll(); }
function showReceipt(s,amount,method,code,purpose,before,after){ let receiptNo="REC-"+Date.now().toString().slice(-6); document.getElementById("receiptArea").innerHTML=`<div class="card"><h3>🧾 ${t("Receipt","Risiti")} - ${receiptNo}</h3><div class="receipt" id="receiptPrint"><div>🇰🇪 NPS AJIRA DRIVING SCHOOL</div><b>${t("PAYMENT RECEIPT","RISITI YA MALIPO")}</b><hr><p>${t("Student:","Mwanafunzi:")} <b>${s.name} (${s.admissionNo})</b><br>${t("Course:","Kozi:")} ${s.courseTitle}<br>${t("For:","Kwa:")} ${purpose}<br>${t("Method:","Njia:")} ${method} - ${code}<br>${t("Amount:","Kiasi:")} <b>Ksh ${amount.toLocaleString()}</b><br>${t("Balance Before:","Deni Kabla:")} Ksh ${before.toLocaleString()}<br>${t("Balance Now:","Deni Sasa:")} <b>Ksh ${after.toLocaleString()} ${after===0?"✅ PAID IN FULL":""}</b><br>${t("Date:","Tarehe:")} ${getToday()} • ${t("Received By:","Amepokea:")} ${currentUser.name}</p></div><button class="green" onclick="printReceipt()">🖨️ ${t("Print Receipt","Print Risiti")}</button></div>`; }
function printReceipt(){ let c=document.getElementById("receiptPrint")?.innerHTML; if(!c) return; let w=window.open("","_blank"); w.document.write(`<html><body>${c}<script>window.onload=()=>window.print()<\/script></body></html>`); w.document.close(); }
function payThisStudent(id){ showTab('payments'); document.getElementById("pStudent").value=id; updatePayFormInfo(); }
function updatePayFormInfo(){ let id=document.getElementById("pStudent").value; let s=students.find(x=>x.id==id); if(!s) return; let bal=getBal(s); document.getElementById("pStudentInfo").innerHTML=`<b>${s.name} - ${s.admissionNo}</b><br>${t("Paid:","Amelipa:")} Ksh ${(s.totalPaid||0).toLocaleString()} / Ksh ${s.coursePrice.toLocaleString()} (${getPct(s)}%) • ${t("Balance:","Deni:")} <b>Ksh ${bal.toLocaleString()}</b>`; if(!document.getElementById("pMpesaPhone").value) document.getElementById("pMpesaPhone").value=s.phone; }
function whatsappStudent(phone,msg){ window.open("https://wa.me/254"+phone.replace(/^0/,"").replace(/\s/g,"")+"?text="+encodeURIComponent(msg),"_blank"); }
// CERTIFICATE
function showCertificate(id){ let s=students.find(x=>x.id===id); if(!s||s.status!=="Passed") return alert(t("Certificate for passed students only","Cheti kwa waliopita tu")); let certNo="AJIRA-DS-"+String(s.id).padStart(4,"0")+"-"+new Date().getFullYear(); document.getElementById("certArea").innerHTML=`<div id="certPrint" style="border:4px double #0b2c4a;padding:20px;text-align:center;background:#fffef5"><div>🇰🇪 REPUBLIC OF KENYA</div><h2>NPS AJIRA DRIVING SCHOOL</h2><div style="font-size:28px">🏆 ${t("CERTIFICATE OF COMPLETION","CHETI CHA KUMALIZA")}</div><hr><p>${t("This is to certify that","Hiki ni kuthibitisha kuwa")}</p><h2>${s.name.toUpperCase()}</h2><p>ID: ${s.idNo} • Admission: ${s.admissionNo}</p><p>${t("Has completed and PASSED","Amemaliza na KUFAULU")}</p><h3>${s.courseTitle}</h3><p>${t("Lessons:","Masomo:")} ${s.lessonsDone}/20 • ${t("Paid:","Amelipa:")} Ksh ${(s.totalPaid||0).toLocaleString()} ✅</p><p>${t("Certificate No:","Cheti No:")} <b>${certNo}</b> • ${getToday()}</p></div><button class="green" onclick="printCert()">🖨️ ${t("Print Certificate","Print Cheti")}</button><button class="secondary" onclick="showTab('students')">← ${t("Back","Rudi")}</button>`; showTab('cert'); }
function printCert(){ let c=document.getElementById("certPrint")?.innerHTML; if(!c) return; let w=window.open("","_blank"); w.document.write(`<html><body>${c}<script>window.onload=()=>window.print()<\/script></body></html>`); w.document.close(); }
// REPORT
function generateReport(){ let month=document.getElementById("reportMonth").value||getCurrentMonth(); let mPays=payments.filter(p=>p.date && p.date.startsWith(month)); let html=`<div id="dsReportPrint" style="background:#fff;border:1px solid #ddd;padding:18px"><div style="text-align:center"><div>🇰🇪 REPUBLIC OF KENYA</div><h2>NPS AJIRA DRIVING SCHOOL</h2><div>${t("Monthly Report - ","Ripoti ya Mwezi - ")}${month}</div><hr></div><p>${t("Students:","Wanafunzi:")} ${students.length} • ${t("Passed:","Wamefaulu:")} ${students.filter(s=>s.status==="Passed").length} • ${t("Classes Booked:","Madarsa Yaliyowekwa:")} ${classes.length}<br>${t("Collected This Month:","Zimekusanywa Mwezi Huu:")} <b>Ksh ${mPays.reduce((sum,p)=>sum+p.amount,0).toLocaleString()}</b> • ${t("Total Owing:","Jumla Inayodaiwa:")} Ksh ${students.reduce((sum,s)=>sum+getBal(s),0).toLocaleString()}</p><h4>${t("STUDENTS","WANAFUNZI")}</h4><table border="1" cellpadding="5" style="width:100%;border-collapse:collapse;font-size:12px"><tr><th>${t("Admission","Admission")}</th><th>${t("Name","Jina")}</th><th>${t("Course","Kozi")}</th><th>${t("Status","Status")}</th><th>${t("Lessons","Masomo")}</th><th>${t("Paid","Amelipa")}</th><th>${t("Balance","Deni")}</th></tr>${students.map(s=>`<tr><td>${s.admissionNo}</td><td>${s.name}</td><td>${s.courseTitle}</td><td>${s.status}</td><td>${s.lessonsDone||0}/20</td><td>Ksh ${(s.totalPaid||0).toLocaleString()}</td><td>Ksh ${getBal(s).toLocaleString()}</td></tr>`).join("")}</table><h4>${t("CLASSES BOOKED","MADARSA YALIYOWEKWA")}</h4>${classes.map(c=>`<div>${c.date} ${c.time} - ${c.name} - ${c.title} - ${c.status} - ${c.vehicle}</div>`).join("")}<h4>${t("PAYMENTS","MALIPO")}</h4>${mPays.map(p=>`<div>${p.date} - ${p.name} - Ksh ${p.amount.toLocaleString()} - ${p.method} - ${p.code}</div>`).join("")||t("None","Hakuna")}</div><button class="green" onclick="printReport()">🖨️ ${t("Print / Save PDF","Print / Save PDF")}</button>`; document.getElementById("reportPreview").innerHTML=html; }
function printReport(){ let c=document.getElementById("dsReportPrint")?.innerHTML; if(!c) return; let w=window.open("","_blank"); w.document.write(`<html><body>${c}<script>window.onload=()=>window.print()<\/script></body></html>`); w.document.close(); }
function shareReport(){ let month=document.getElementById("reportMonth").value||getCurrentMonth(); let txt=t(`🇰🇪 AJIRA DRIVING SCHOOL REPORT\nMonth: ${month}\nStudents: ${students.length} • Passed: ${students.filter(s=>s.status==="Passed").length} • Classes: ${classes.length}\nCollected: Ksh ${payments.reduce((sum,p)=>sum+p.amount,0).toLocaleString()} • Owing: Ksh ${students.reduce((sum,s)=>sum+getBal(s),0).toLocaleString()}`,`🇰🇪 RIPOTI YA AJIRA DRIVING SCHOOL\nMwezi: ${month}\nWanafunzi: ${students.length} • Wamefaulu: ${students.filter(s=>s.status==="Passed").length} • Madarsa: ${classes.length}\nZimekusanywa: Ksh ${payments.reduce((sum,p)=>sum+p.amount,0).toLocaleString()} • Zinadaiwa: Ksh ${students.reduce((sum,s)=>sum+getBal(s),0).toLocaleString()}`); window.open("https://wa.me/?text="+encodeURIComponent(txt),"_blank"); }
function renderCatalog(){ let f=document.getElementById("catFilter")?.value||"all"; let list=SYLLABUS.filter(s=>f==="all"||s.type===f); document.getElementById("catalogList").innerHTML=list.map(s=>{ let title=LANG==="sw"?s.titleSW:s.titleEN; let desc=LANG==="sw"?s.descSW:s.descEN; let done=classes.filter(l=>l.syllabusId===s.id && l.status==="Completed" && (!isAdmin?l.phone===currentUser?.phone:true)).length>0; return `<div class="card" style="border-left:5px solid ${done?"#1a7a3a":"#0b2c4a"}"><div class="top"><b>${s.no} • ${s.type} • ${s.duration}</b><span class="badge" style="background:${done?"#1a7a3a":"#ffe082"};color:${done?"#fff":"#000"}">${done?"✅ "+t("Done","Nimemaliza"):"⏳ "+t("Not Done","Sijamaliza")}</span></div><h3 style="margin:6px 0">${title}</h3><span class="small">${desc}</span><br><button class="secondary" onclick="bookThisLesson(${s.id})">📅 ${t("Book This Lesson","Weka Nafasi ya Somo Hili")}</button></div>`; }).join(""); }
function bookThisLesson(id){ showTab('classes'); document.getElementById("cLesson").value=id; updateClassInfo(); }

function renderAll(){
  applyLang(); renderCatalog();
  // Dropdowns
  document.getElementById("aCourse").innerHTML=courses.length?courses.map(c=>`<option value="${c.id}">${c.title} - Ksh ${c.price.toLocaleString()}</option>`).join(""):"";
  document.getElementById("cStudent").innerHTML=students.length?students.map(s=>`<option value="${s.id}">${s.name} - ${s.admissionNo} - ${t("Balance:","Deni:")} Ksh ${getBal(s).toLocaleString()}</option>`).join(""):`<option value="">${t("No Student","Hakuna Mwanafunzi")}</option>`;
  document.getElementById("pStudent").innerHTML=students.length?students.map(s=>`<option value="${s.id}">${s.name} - ${s.admissionNo} - ${t("Balance:","Deni:")} Ksh ${getBal(s).toLocaleString()}</option>`).join(""):`<option value="">${t("No Student","Hakuna Mwanafunzi")}</option>`;
  document.getElementById("cLesson").innerHTML=SYLLABUS.map(s=>`<option value="${s.id}">${s.no} - ${LANG==="sw"?s.titleSW:s.titleEN} (${s.type})</option>`).join("");
  if(!document.getElementById("cDate").value) document.getElementById("cDate").value=getToday();
  updateAdmissionInfo(); updateClassPayInfo(); updatePayFormInfo(); updateClassInfo();

  // KPIs
  document.getElementById("kStudents").innerText=students.length;
  document.getElementById("kClasses").innerText=classes.length;
  document.getElementById("kPaid").innerText="Ksh "+payments.reduce((sum,p)=>sum+p.amount,0).toLocaleString();
  document.getElementById("kOwing").innerText="Ksh "+students.reduce((sum,s)=>sum+getBal(s),0).toLocaleString();
  document.getElementById("kLessonsDone").innerText=classes.filter(c=>c.status==="Completed").length;
  document.getElementById("kPassed").innerText=students.filter(s=>s.status==="Passed").length;

  // MY CARD
  let myStu=!isAdmin?students.filter(s=>s.phone===currentUser?.phone):[];
  let myS=myStu[0];
  if(myS){
    let bal=getBal(myS); let pct=getPct(myS);
    document.getElementById("myStatusBadge").innerText=myS.status;
    document.getElementById("myAdmissionInfo").innerHTML=`<b>${myS.name}</b> • ${myS.admissionNo}<br>${t("Course:","Kozi:")} ${myS.courseTitle}<br>${t("Schedule:","Ratiba:")} ${myS.schedule} • ${t("Plan:","Mpango:")} ${myS.plan}<br>${t("Next of Kin:","Ndugu wa Karibu:")} ${myS.nextKin||"-"} • ${myS.address||""}`;
    document.getElementById("myPaid2").innerText="Ksh "+(myS.totalPaid||0).toLocaleString(); document.getElementById("myFee2").innerText="Ksh "+myS.coursePrice.toLocaleString(); document.getElementById("myPct").innerText=pct+"%"; document.getElementById("myBal2").innerText="Ksh "+bal.toLocaleString(); document.getElementById("myPayBar").style.width=pct+"%"; document.getElementById("myPayBar").style.background=bal===0?"#1a7a3a":"#ef6c00";
    let myClasses=classes.filter(c=>c.phone===currentUser?.phone);
    document.getElementById("myLessonCount").innerText=(myS.lessonsDone||0)+"/20";
    let next=myClasses.filter(c=>c.status==="Scheduled").sort((a,b)=>a.date.localeCompare(b.date))[0];
    document.getElementById("myNextClass").innerText=next?next.title+" "+next.date+" "+next.time:"-";
    document.getElementById("myCardActions").innerHTML=bal>0?`<button class="green" onclick="payThisStudent(${myS.id})">💚 ${t("Pay Balance - Ksh ","Lipa Deni - Ksh ")}${bal.toLocaleString()}</button>`:`<button class="green" onclick="showCertificate(${myS.id})">🏆 ${t("Get Certificate","Pata Cheti")}</button>`;
    document.getElementById("myCard").style.display="block";
  } else if(isAdmin){
    document.getElementById("myStatusBadge").innerText=t("ADMIN VIEW","MTIZAMO WA ADMIN");
    document.getElementById("myAdmissionInfo").innerHTML=t(`You are viewing all students. Use Admission to add new student, Classes to book, Payments to record.`,`Unaona wanafunzi wote. Tumia Admission kuongeza mwanafunzi mpya, Classes kuweka darasa, Payments kurekodi malipo.`);
    let totalFees=students.reduce((sum,s)=>sum+s.coursePrice,0); let totalPaid=students.reduce((sum,s)=>sum+(s.totalPaid||0),0);
    document.getElementById("myPaid2").innerText="Ksh "+totalPaid.toLocaleString(); document.getElementById("myFee2").innerText="Ksh "+totalFees.toLocaleString(); document.getElementById("myPct").innerText=totalFees?Math.round(totalPaid/totalFees*100)+"%":"0%"; document.getElementById("myBal2").innerText="Ksh "+(totalFees-totalPaid).toLocaleString(); document.getElementById("myPayBar").style.width=(totalFees?Math.round(totalPaid/totalFees*100):0)+"%";
    document.getElementById("myLessonCount").innerText=classes.filter(c=>c.status==="Completed").length+"/"+classes.length;
    document.getElementById("myNextClass").innerText=classes.filter(c=>c.status==="Scheduled").length+" "+t("scheduled","zimepangwa");
    document.getElementById("myCardActions").innerHTML=`<button class="secondary" onclick="showTab('balances')">⚖️ ${t("View All Balances","Ona Madeni Yote")}</button>`;
  }

  // ALERTS
  let alertHtml="";
  if(myS){ let bal=getBal(myS); if(bal===0) alertHtml+=`<div class="alert-green">🎉 ${t("Paid in full! You can book all classes.","Amelipa yote! Unaweza kuweka madarsa yote.")}</div>`; else if(bal>10000) alertHtml+=`<div class="alert-red">🔴 ${t("BIG BALANCE: Ksh ","DENI KUBWA: Ksh ")}${bal.toLocaleString()} - ${t("Pay now to continue booking after 5 lessons.","Lipa sasa ili uendelee kuweka madarsa baada ya masomo 5.")} <button class="green" onclick="payThisStudent(${myS.id})">💚 ${t("Pay Now","Lipa Sasa")}</button></div>`; else alertHtml+=`<div class="alert-orange">💰 ${t("Balance: Ksh ","Deni: Ksh ")}${bal.toLocaleString()} - ${t("Pay in installments while you learn.","Lipa kidogo kidogo ukijifunza.")}</div>`; }
  if(isAdmin){ let big=students.filter(s=>getBal(s)>10000); if(big.length) alertHtml+=`<div class="alert-red">🔴 ${big.length} ${t("students have BIG balance - Total: Ksh ","wanafunzi wana DENI KUBWA - Jumla: Ksh ")}${big.reduce((sum,s)=>sum+getBal(s),0).toLocaleString()}</div>`; }
  let todayCls=classes.filter(c=>c.date===getToday() && (!isAdmin?c.phone===currentUser?.phone:true)); if(todayCls.length) alertHtml+=`<div class="alert-orange">📅 ${t("You have","Una")} ${todayCls.length} ${t("class(es) TODAY","darasa leo")}: ${todayCls.map(c=>c.title+" "+c.time).join(", ")}</div>`;
  if(!alertHtml) alertHtml=`<div class="alert-green">✅ ${t("Welcome - Admit student, book class, record payment!","Karibu - Mwandikishe mwanafunzi, weka darasa, rekodi malipo!")}</div>`;
  document.getElementById("alertBox").innerHTML=alertHtml;

  // STUDENTS LIST
  let stuF=document.getElementById("stuFilter")?.value||"all"; let stuS=document.getElementById("stuSearch")?.value.toLowerCase()||"";
  let fStudents=students.filter(s=>{ if(!isAdmin && s.phone!==currentUser?.phone) return false; if(stuF!=="all" && s.status!==stuF) return false; return (s.name+" "+s.phone+" "+s.admissionNo+" "+s.courseTitle).toLowerCase().includes(stuS); });
  document.getElementById("studentList").innerHTML=fStudents.length?fStudents.map(s=>{ let bal=getBal(s); let pct=getPct(s); let color=bal===0?"#1a7a3a":bal>10000?"#b71c1c":"#ef6c00"; let initials=s.name.split(" ").map(w=>w[0]).join("").slice(0,2).toUpperCase(); let sClasses=classes.filter(c=>c.studentId===s.id); return `<div class="card" style="border-left:5px solid ${color}"><div style="display:flex;gap:10px"><div class="avatar">${initials}</div><div style="flex:1"><div class="top"><b>🧑‍🎓 ${s.name}</b><span class="badge" style="background:${color};color:#fff">${s.status}</span></div><span class="small">${t("Admission:","Admission:")} <b>${s.admissionNo}</b> • ${t("Phone:","Simu:")} ${s.phone} • ID: ${s.idNo}<br>${t("Course:","Kozi:")} <b>${s.courseTitle}</b> • ${t("Plan:","Mpango:")} ${s.plan}<br>${t("Schedule:","Ratiba:")} ${s.schedule} • ${t("Lessons:","Masomo:")} ${s.lessonsDone||0}/20 • ${t("Classes Booked:","Madarsa Yaliyowekwa:")} ${sClasses.length}</span></div></div><div style="margin-top:8px"><div class="top"><span class="small">${t("Paid:","Amelipa:")} Ksh ${(s.totalPaid||0).toLocaleString()} / Ksh ${s.coursePrice.toLocaleString()} (${pct}%)</span><span class="small">${t("Balance:","Deni:")} Ksh ${bal.toLocaleString()}</span></div><div class="bar"><div class="fill" style="width:${pct}%;background:${color}"></div></div></div>${s.status==="Passed"?`<button class="green" onclick="showCertificate(${s.id})">🏆 ${t("Certificate","Cheti")}</button>`:""}<div style="display:flex;gap:6px"><button class="secondary" style="flex:1" onclick="bookClassFor(${s.id})">📅 ${t("Book Class","Weka Darasa")}</button><button class="secondary" style="flex:1" onclick="payThisStudent(${s.id})">💰 ${t("Pay","Lipa")}</button><button class="secondary" style="flex:1" onclick="printAdmission('${s.admissionNo}')">🖨️ ${t("Admission Letter","Barua")}</button></div>${isAdmin?`<select onchange="changeStudentStatus(${s.id},this.value)"><option ${s.status==='Enrolled'?'selected':''}>Enrolled</option><option ${s.status==='In Training'?'selected':''}>In Training</option><option ${s.status==='Ready for Test'?'selected':''}>Ready for Test</option><option ${s.status==='Passed'?'selected':''}>Passed</option><option ${s.status==='Failed'?'selected':''}>Failed</option><option ${s.status==='Dropped'?'selected':''}>Dropped</option></select>`:""}</div>`; }).join(""):`<p class="small">${t("No students.","Hakuna wanafunzi.")}</p>`;

  // CLASSES
  let todayAll=classes.filter(c=>c.date===getToday());
  document.getElementById("todayClasses").innerHTML=todayAll.length?todayAll.map(c=>`<div class="card"><div class="top"><b>${c.name} (${c.admissionNo}) - ${c.title}</b><span class="badge">${c.status}</span></div><span class="small">${c.time} • ${c.vehicle} • ${c.instructor} • ${c.location}</span></div>`).join(""):`<p class="small">${t("No classes today.","Hakuna madarsa leo.")}</p>`;
  let cf=document.getElementById("classFilter")?.value||"all";
  let fCls=classes.filter(c=>{ if(!isAdmin && c.phone!==currentUser?.phone) return false; if(cf!=="all" && c.status!==cf) return false; return true; }).sort((a,b)=>b.date.localeCompare(a.date));
  document.getElementById("classList").innerHTML=fCls.length?fCls.map(c=>{ let stu=students.find(x=>x.id===c.studentId); let bal=stu?getBal(stu):0; let isToday=c.date===getToday(); return `<div class="card class-slot ${c.status==="Completed"?"":isToday?"":c.status==="Cancelled"?"":""}"><div class="top"><b>${c.title} • ${c.type}</b><span class="badge" style="background:${c.status==="Completed"?"#1a7a3a":c.status==="Absent"?"#b71c1c":c.status==="Cancelled"?"#999":"#ef6c00"};color:#fff">${c.status}</span></div><span class="small">${c.name} (${c.admissionNo}) • ${c.date} ${c.time}<br>${t("Vehicle:","Gari:")} ${c.vehicle} • ${t("Instructor:","Mwalimu:")} ${c.instructor} • ${c.location}<br>${t("Balance:","Deni:")} Ksh ${bal.toLocaleString()}</span>${c.status==="Scheduled"?`<div style="display:flex;gap:6px">${isAdmin?`<button class="green" style="flex:1" onclick="markClass(${c.id},'Completed')">✅ ${t("Present","Amehudhuria")}</button><button class="red" style="flex:1" onclick="markClass(${c.id},'Absent')">❌ ${t("Absent","Hayupo")}</button>`:`<button class="secondary" style="flex:1" onclick="cancelClass(${c.id})">${t("Cancel","Ghairi")}</button>`}</div>`:""}</div>`; }).join(""):`<p class="small">${t("No classes booked yet.","Hakuna madarsa yaliyowekwa bado.")}</p>`;

  // PAYMENTS LIST
  let pf=document.getElementById("payFilter")?.value||"all";
  let fPays=payments.filter(p=>{ if(!isAdmin && p.name!==currentUser?.name) return false; if(pf!=="all" && p.method!==pf) return false; return true; });
  document.getElementById("paymentList").innerHTML=fPays.length?fPays.map(p=>`<div class="card"><div class="top"><b>${p.name} (${p.admissionNo||""}) - Ksh ${p.amount.toLocaleString()}</b><span class="badge">${p.method}</span></div><span class="small">${t("Code:","Code:")} ${p.code} • ${p.for||""} • ${p.date} • ${p.officer}</span></div>`).join(""):`<p class="small">${t("No payments.","Hakuna malipo.")}</p>`;

  // BALANCES
  let bf=document.getElementById("balFilter")?.value||"all"; let bs=document.getElementById("balSearch")?.value.toLowerCase()||"";
  let fBal=students.filter(s=>{ if(!isAdmin && s.phone!==currentUser?.phone) return false; let bal=getBal(s); if(bf==="paid" && bal!==0) return false; if(bf==="owing" && bal===0) return false; if(bf==="big" && bal<=10000) return false; return (s.name+" "+s.phone+" "+s.admissionNo).toLowerCase().includes(bs); }).sort((a,b)=>getBal(b)-getBal(a));
  document.getElementById("balanceList").innerHTML=fBal.length?fBal.map(s=>{ let bal=getBal(s); let pct=getPct(s); let color=bal===0?"#1a7a3a":bal>10000?"#b71c1c":"#ef6c00"; let myPays=payments.filter(p=>p.studentId===s.id); return `<div class="card" style="border-left:5px solid ${color}"><div class="top"><b>${s.name} (${s.admissionNo})</b><span class="badge" style="background:${color};color:#fff">${bal===0?t("✅ PAID IN FULL","✅ AMELIPA YOTE"):t("⚠️ BALANCE Ksh ","⚠️ DENI Ksh ")+bal.toLocaleString()}</span></div><span class="small">${s.courseTitle} • ${s.status} • ${t("Lessons:","Masomo:")} ${s.lessonsDone||0}/20</span><div class="bar"><div class="fill" style="width:${pct}%;background:${color}"></div></div><span class="small">${t("Paid:","Amelipa:")} Ksh ${(s.totalPaid||0).toLocaleString()} / Ksh ${s.coursePrice.toLocaleString()} (${pct}%)<br><b>${t("Payment History:","Historia ya Malipo:")}</b><br>${myPays.length?myPays.map(p=>`• ${p.date} - Ksh ${p.amount.toLocaleString()} - ${p.method} - ${p.code} - ${p.for||""}`).join("<br>"):"-"}</span>${bal>0?`<button class="green" onclick="payThisStudent(${s.id})">💚 ${t("Pay Now - Ksh ","Lipa Sasa - Ksh ")}${bal.toLocaleString()}</button><button class="secondary" onclick="whatsappStudent('${s.phone}','${t(`Hello ${s.name}, your balance at Ajira Driving School (${s.admissionNo}) is Ksh ${bal.toLocaleString()}. Please pay to continue classes.`, `Habari ${s.name}, deni lako Ajira Driving School (${s.admissionNo}) ni Ksh ${bal.toLocaleString()}. Tafadhali lipa ili uendelee na madarsa.`)}')">💬 ${t("Remind WhatsApp","Kumbusha WhatsApp")}</button>`:`<div class="alert-green">🎉 ${t("Paid in full!","Amelipa yote!")}</div>`}</div>`; }).join(""):`<p class="small">${t("No students.","Hakuna wanafunzi.")}</p>`;
}
</script>
</body>
</html>

# AJIRA-DRIVING-SCHOOL
 DRIVING AND COMPUTER
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no, viewport-fit=cover">
<meta name="theme-color" content="#0b2c4a">
<meta name="apple-mobile-web-app-capable" content="yes">
<title>AJIRA Driving School - EN / SW</title>
<link rel="manifest" href="manifest.json">
<link rel="apple-touch-icon" href="icon.png">
<style>
*{box-sizing:border-box;font-family:Arial,sans-serif;-webkit-tap-highlight-color:transparent}
body{margin:0;background:#0b2c4a;display:flex;justify-content:center}
.phone{width:100%;max-width:460px;min-height:100vh;background:#fff;display:flex;flex-direction:column}
header{background:#0b2c4a;color:#fff;padding:14px;text-align:center;position:sticky;top:0;z-index:10}
header h1{margin:0;font-size:18px} header p{margin:4px 0 0;font-size:12px;opacity:.9}
header .badge{background:#ffc107;color:#000;padding:3px 8px;border-radius:10px;font-size:11px;font-weight:700}
.lang-switch{display:flex;gap:6px;margin-top:10px}
.lang-switch button{flex:1;padding:9px;background:#fff;color:#0b2c4a;font-weight:900;min-height:38px}
.lang-switch button.active{background:#ffc107}
main{padding:14px 14px 90px;flex:1}
.card{background:#f6f6f6;border-radius:12px;padding:12px;margin-bottom:10px}
button{width:100%;padding:13px;border:0;border-radius:10px;background:#0b2c4a;color:#fff;font-weight:700;font-size:15px;cursor:pointer;margin-top:8px;min-height:48px}
button.secondary{background:#eee;color:#222}
button.green{background:#1a7a3a} button.red{background:#b71c1c} button.orange{background:#ef6c00}
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
.alert-red{background:#ffebee;border:2px solid #b71c1c;padding:12px;border-radius:10px;margin-bottom:10px;font-weight:700;color:#b71c1c}
.alert-orange{background:#fff3e0;border:2px solid #ef6c00;padding:12px;border-radius:10px;margin-bottom:10px;font-weight:700;color:#e65100}
.alert-green{background:#e8f5e9;border:1px solid #1a7a3a;padding:10px;border-radius:10px;margin-bottom:10px}
.bar{height:14px;background:#eee;border-radius:7px;overflow:hidden;margin:6px 0} .fill{height:100%;background:#1a7a3a}
#installBtn{background:#ffc107;color:#000;font-weight:900}
.avatar{width:56px;height:56px;border-radius:50%;background:#0b2c4a;color:#fff;display:flex;align-items:center;justify-content:center;font-size:22px;font-weight:900;overflow:hidden}
.quiz-opt{width:100%;text-align:left;background:#fff;border:2px solid #ddd;padding:12px;border-radius:10px;margin:5px 0;cursor:pointer;font-size:15px}
.quiz-opt.correct{border-color:#1a7a3a;background:#e8f5e9} .quiz-opt.wrong{border-color:#b71c1c;background:#ffebee}
.cert{border:4px double #0b2c4a;padding:20px;text-align:center;background:#fffef5}
.idcard{background:linear-gradient(135deg,#0b2c4a,#1a5a8a);color:#fff;border-radius:14px;padding:14px;display:flex;gap:12px}
.idcard .photo{width:80px;height:90px;background:#fff;color:#0b2c4a;border-radius:8px;display:flex;align-items:center;justify-content:center;font-size:28px;font-weight:900;overflow:hidden}
.mpesa-box{background:#e8f5e9;border:2px solid #1a7a3a;border-radius:12px;padding:12px}
</style>
</head>
<body>
<div class="phone">
<header><div>🇰🇪 NPS AJIRA DRIVING SCHOOL</div><h1 data-i18n="headerTitle">LEARN • PASS • GET LICENCE • GET JOB</h1><p data-i18n="headerSub">Courses • Quiz • Certificate • ID • M-Pesa • Jobs</p><span class="badge">NTSA APPROVED • EN / SW</span>
<div class="lang-switch"><button id="btnEN" class="active" onclick="setLang('en')">🇬🇧 ENGLISH</button><button id="btnSW" onclick="setLang('sw')">🇰🇪 KISWAHILI</button></div>
<button id="installBtn" class="hidden" onclick="installApp()">📱 Install App</button></header>
<main>
<div id="loginView">
  <h2 data-i18n="welcome">Welcome to Ajira Driving School</h2>
  <select id="userType" onchange="toggleLogin()"><option value="student" data-i18n="iAmStudent">I am a Student - I Want to Learn Driving</option><option value="instructor" data-i18n="iAmInstructor">I am an Instructor / Admin</option></select>
  <div id="studentLogin"><input id="stuName" data-ph="fullName" placeholder="Full Name *"><input id="stuPhone" data-ph="phone" placeholder="Phone e.g. 0712345678" inputmode="tel"><input id="stuId" data-ph="idNo" placeholder="ID No." inputmode="numeric"></div>
  <div id="instructorLogin" class="hidden"><input id="offName" data-ph="instructorName" placeholder="Instructor / Officer Name"><input id="offNo" data-ph="staffNo" placeholder="Staff / Service No." inputmode="numeric"><select id="offRole"><option data-i18n="roleInstructor">Instructor - Driving Teacher</option><option data-i18n="roleAdmin">Admin - Ajira Driving School</option><option data-i18n="roleOCS">OCS / MT Officer</option></select></div>
  <button onclick="login()" data-i18n="login">Login</button>
  <p class="small" data-i18n="loginHint">Student: Name + Phone only.<br>Instructor Demo: Any name + any number</p>
</div>

<div id="appView" class="hidden">
  <div class="top"><b><span data-i18n="hello">Hello</span>, <span id="userName"></span></b><button class="secondary" style="width:auto" onclick="logout()" data-i18n="logout">Logout</button></div>
  <p class="small"><span id="stationLabel"></span> • <span id="dateLabel"></span></p>
  <div id="alertBox"></div>
  <div style="display:flex;gap:6px;flex-wrap:wrap">
    <div class="card" style="flex:1;text-align:center;min-width:70px"><b id="totalCourses">0</b><br><span class="small" data-i18n="courses">Courses</span></div>
    <div class="card" style="flex:1;text-align:center;min-width:70px"><b id="totalStudents">0</b><br><span class="small" data-i18n="students">Students</span></div>
    <div class="card" style="flex:1;text-align:center;min-width:70px"><b id="totalPassed" style="color:#1a7a3a">0</b><br><span class="small" data-i18n="passed">Passed</span></div>
    <div class="card" style="flex:1;text-align:center;min-width:70px"><b id="totalPaid">Ksh 0</b><br><span class="small" data-i18n="paid">Paid</span></div>
    <div class="card" style="flex:1;text-align:center;min-width:70px"><b id="totalBalance" style="color:#b71c1c">Ksh 0</b><br><span class="small" data-i18n="balance">Balance</span></div>
  </div>
  <div class="tabs">
    <button id="tabCourses" class="active" onclick="showTab('courses')">🚗 <span data-i18n="courses">Courses</span></button>
    <button id="tabEnroll" onclick="showTab('enroll')">📝 <span data-i18n="enroll">Enroll</span></button>
    <button id="tabStudents" onclick="showTab('students')">🧑‍🎓 <span data-i18n="students">Students</span></button>
    <button id="tabQuiz" onclick="showTab('quiz')">🧠 <span data-i18n="quiz">Quiz</span></button>
    <button id="tabID" onclick="showTab('id')">🪪 <span data-i18n="idCard">ID Card</span></button>
    <button id="tabLessons" onclick="showTab('lessons')">📅 <span data-i18n="lessons">Lessons</span></button>
    <button id="tabPayments" onclick="showTab('payments')">💰 <span data-i18n="payments">Payments</span></button>
    <button id="tabExam" onclick="showTab('exam')">📝 <span data-i18n="exam">Exam</span></button>
    <button id="tabJobs" onclick="showTab('jobs')">💼 <span data-i18n="jobs">Jobs</span></button>
    <button id="tabReport" onclick="showTab('report')">📄 <span data-i18n="report">Report</span></button>
  </div>

  <div id="coursesTab">
    <div id="adminCourseForm" class="card hidden"><h3 style="margin:0" data-i18n="addCourse">+ Add New Course (Admin Only)</h3>
      <input id="cTitle" data-ph="courseEx" placeholder="Course e.g. Class B - Small Car"><select id="cClass"><option>Class A - Motorcycle / Pikipiki</option><option>Class B - Small Car / Probox</option><option>Class C - Lorry</option><option>Class D - Bus / PSV</option><option>Class B+C - Car + Lorry</option><option>Class BCE - All / Zote</option><option>Defensive Driving</option><option>Refresher - NPS Driver</option></select>
      <input id="cPrice" data-ph="price" placeholder="Price e.g. 18000" type="number" inputmode="numeric"><input id="cDuration" data-ph="duration" placeholder="Duration e.g. 4 Weeks / 20 Lessons"><input id="cInstructor" data-ph="instructor" placeholder="Instructor"><input id="cVehicle" data-ph="vehicle" placeholder="Training Vehicle e.g. KDJ 123A - Probox"><textarea id="cDesc" rows="2" data-ph="desc" placeholder="Description..."></textarea>
      <button class="green" onclick="saveCourse()" data-i18n="addCourseBtn">Add Course</button></div>
    <input id="courseSearch" data-ph="searchCourse" placeholder="Search course: B, C, PSV..." oninput="renderAll()"><div id="courseList"></div>
  </div>

  <div id="enrollTab" class="hidden">
    <div class="card"><h3 style="margin:0" data-i18n="enrollNow">📝 Enroll Now</h3>
      <label class="small" data-i18n="selectCourse">Select Course *</label><select id="eCourse" onchange="updateEnrollInfo()"></select><div id="eCourseInfo" class="small"></div>
      <input id="eName" data-ph="fullName" placeholder="Full Name *"><input id="ePhone" data-ph="phone" placeholder="Phone *" inputmode="tel"><input id="eId" data-ph="idNo" placeholder="ID No. *" inputmode="numeric"><input id="eAge" data-ph="age" placeholder="Age" type="number" inputmode="numeric">
      <select id="eGender"><option data-i18n="male">Male</option><option data-i18n="female">Female</option></select>
      <input id="eCounty" data-ph="county" placeholder="County e.g. Trans Nzoia"><input id="eEducation" data-ph="education" placeholder="Education e.g. KCSE C-">
      <select id="eHasLicence"><option data-i18n="noLicence">No Licence - Complete Beginner</option><option data-i18n="haveLicence">Have Licence - Want to Add Class</option><option data-i18n="expiredLicence">Licence Expired - Refresher</option></select>
      <input id="eLicenceNo" data-ph="licenceNo" placeholder="Licence No. (If you have one)">
      <select id="eSchedule"><option data-i18n="morning">Morning - 8am - 11am</option><option data-i18n="midday">Midday - 11am - 2pm</option><option data-i18n="afternoon">Afternoon - 2pm - 5pm</option><option data-i18n="weekend">Weekend Only - Sat / Sun</option></select>
      <div class="mpesa-box"><b>💚 <span data-i18n="payMpesa">PAY WITH M-PESA - STK PUSH</span></b><p class="small" data-i18n="stkHint">Enter phone, enter amount, tap Pay. You will get a prompt on your phone to enter your M-Pesa PIN.</p>
      <input id="eMpesaPhone" data-ph="mpesaPhone" placeholder="M-Pesa Phone e.g. 0712345678" inputmode="tel"><input id="eDeposit" data-ph="deposit" placeholder="Deposit Ksh e.g. 5000" type="number" inputmode="numeric">
      <button class="green" onclick="stkPushEnroll()">💚 <span data-i18n="payMpesaBtn">Pay with M-Pesa - STK Push</span></button>
      <p class="small"><span data-i18n="alreadyPaid">Or if you already paid:</span> <input id="eMpesaCode" data-ph="mpesaCode" placeholder="M-Pesa Code e.g. QK123ABC"></p></div>
      <button class="green" onclick="enrollStudent()" data-i18n="enrollBtn">Enroll →</button></div>
  </div>

  <div id="studentsTab" class="hidden">
    <div class="card" style="background:#e3f2fd"><h3 style="margin:0">🧑‍🎓 <span data-i18n="students">Students</span></h3></div>
    <select id="stuFilter" onchange="renderAll()"><option value="all" data-i18n="all">All</option><option value="Enrolled" data-i18n="enrolled">Enrolled</option><option value="In Training" data-i18n="inTraining">In Training</option><option value="Ready for Test" data-i18n="readyTest">Ready for Test</option><option value="Passed" data-i18n="passed">Passed</option><option value="Failed" data-i18n="failed">Failed</option><option value="Dropped" data-i18n="dropped">Dropped</option></select>
    <input id="stuSearch" data-ph="searchStudent" placeholder="Search name, phone..." oninput="renderAll()"><div id="studentList"></div>
  </div>

  <div id="quizTab" class="hidden">
    <div class="card" style="background:#fff3e0"><h3 style="margin:0">🧠 <span data-i18n="quizTitle">Practice Quiz - 50 Question Bank</span></h3><p class="small"><span data-i18n="quizSub">10 random questions every time. Pass 70%+ to be ready for NTSA.</span><br><span data-i18n="bestScore">Your best score:</span> <b id="quizBest">0%</b> • <span data-i18n="attempts">Attempts:</span> <b id="quizAttempts">0</b></p></div>
    <div class="card"><select id="quizType"><option value="all" data-i18n="quizMixed">Mixed - All Topics</option><option value="rules" data-i18n="quizRules">Traffic Rules</option><option value="signs" data-i18n="quizSigns">Road Signs</option><option value="safety" data-i18n="quizSafety">Safety + Defensive</option></select><button class="green" onclick="startQuiz()">▶️ <span data-i18n="startQuiz">Start Quiz</span></button></div>
    <div id="quizArea"></div><div id="quizResult"></div>
  </div>

  <div id="idTab" class="hidden">
    <div class="card"><h3 style="margin:0">🪪 <span data-i18n="idCardTitle">Student ID Card</span></h3><p class="small" data-i18n="idHint">Your ID card appears automatically. Admin sees all students.</p></div>
    <div id="idCardArea"></div>
  </div>

  <div id="lessonsTab" class="hidden">
    <div id="adminLessonForm" class="card hidden"><h3 style="margin:0" data-i18n="scheduleLesson">+ Schedule Lesson (Instructor Only)</h3>
      <label class="small" data-i18n="student">Student</label><select id="lStudent"></select><input id="lDate" type="date"><input id="lTime" type="time">
      <select id="lType"><option data-i18n="lessonRoad">Practical - Driving on Road</option><option data-i18n="lessonParking">Practical - Parking / Yard</option><option data-i18n="lessonTheory">Theory - Traffic Rules</option><option data-i18n="lessonSigns">Theory - Road Signs</option><option data-i18n="lessonMock">Mock Test - Practice Exam</option></select>
      <input id="lVehicle" data-ph="vehicle" placeholder="Vehicle e.g. KDJ 123A"><input id="lInstructor" data-ph="instructor" placeholder="Instructor"><input id="lLocation" data-ph="location" placeholder="Location e.g. Eldoret - Yard">
      <button class="green" onclick="saveLesson()" data-i18n="scheduleBtn">Schedule Lesson</button></div>
    <div id="lessonList"></div>
  </div>

  <div id="paymentsTab" class="hidden">
    <div class="card"><h3 style="margin:0">💰 <span data-i18n="payTitle">Pay / Record Payment</span></h3>
      <label class="small" data-i18n="student">Student</label><select id="pStudent"></select><div id="pStudentInfo" class="small"></div>
      <input id="pAmount" data-ph="amount" placeholder="Amount Ksh" type="number" inputmode="numeric"><select id="pMethod"><option>M-Pesa</option><option>Cash</option><option>Bank</option></select><input id="pCode" data-ph="receipt" placeholder="M-Pesa Code / Receipt No.">
      <button class="green" onclick="savePayment()" data-i18n="recordPayment">Record Payment</button>
      <div class="mpesa-box" style="margin-top:10px"><b>💚 STK Push - <span data-i18n="payNow">Pay Now</span></b><input id="pMpesaPhone" data-ph="mpesaPhone" placeholder="M-Pesa Phone" inputmode="tel"><button class="green" onclick="stkPushPayment()">💚 <span data-i18n="sendStk">Send STK Push</span></button></div>
    </div><div id="paymentList"></div>
  </div>

  <div id="examTab" class="hidden">
    <div id="adminExamForm" class="card hidden"><h3 style="margin:0" data-i18n="recordExam">+ Record Exam Result (Instructor Only)</h3>
      <label class="small" data-i18n="student">Student</label><select id="xStudent"></select><select id="xType"><option>NTSA Theory Test</option><option>NTSA Practical Test</option><option data-i18n="mockTest">Mock Test - School</option><option data-i18n="defensiveTest">Defensive Driving Test</option></select>
      <input id="xScore" data-ph="score" placeholder="Score % e.g. 85" type="number" inputmode="numeric"><select id="xResult"><option data-i18n="passedOpt">Passed ✅</option><option data-i18n="failedOpt">Failed ❌ - Repeat</option><option data-i18n="absentOpt">Absent - Did Not Attend</option></select><input id="xDate" type="date"><textarea id="xNotes" rows="2" data-ph="comments" placeholder="Instructor comments..."></textarea>
      <button class="orange" onclick="saveExam()" data-i18n="recordResult">Record Result</button></div>
    <div id="examList"></div>
  </div>

  <div id="jobsTab" class="hidden">
    <div class="card" style="background:#e8f5e9"><h3 style="margin:0">💼 <span data-i18n="jobsAfter">Jobs After Passing</span></h3></div><div id="jobList"></div>
  </div>

  <div id="reportTab" class="hidden">
    <div class="card"><h3 style="margin:0">📄 <span data-i18n="schoolReport">School Report</span></h3><input type="month" id="reportMonth"><button class="green" onclick="generateReport()" data-i18n="genReport">Generate Report PDF</button><button class="secondary" onclick="shareReport()" data-i18n="shareWA">Share via WhatsApp</button></div><div id="reportPreview"></div>
  </div>

  <div id="certTab" class="hidden"><div id="certArea"></div></div>
</div>
</main>
<footer>NPS AJIRA DRIVING SCHOOL • NTSA Approved<br><span data-i18n="footer">Learn • Pass • Get Job • EN / SW</span></footer>
</div>
<div class="bottom-nav" id="bottomNav" style="display:none">
  <button onclick="showTab('courses')" id="navCourses"><span>🚗</span><span data-i18n="courses">Courses</span></button>
  <button onclick="showTab('enroll')" id="navEnroll"><span>📝</span><span data-i18n="enroll">Enroll</span></button>
  <button onclick="showTab('students')" id="navStudents"><span>🧑‍🎓</span><span data-i18n="students">Students</span></button>
  <button onclick="showTab('quiz')" id="navQuiz"><span>🧠</span><span data-i18n="quiz">Quiz</span></button>
  <button onclick="showTab('id')" id="navID"><span>🪪</span><span data-i18n="idCard">ID</span></button>
  <button onclick="showTab('payments')" id="navPayments"><span>💰</span><span data-i18n="payments">Payments</span></button>
  <button onclick="showTab('exam')" id="navExam"><span>📝</span><span data-i18n="exam">Exam</span></button>
  <button onclick="showTab('jobs')" id="navJobs"><span>💼</span><span data-i18n="jobs">Jobs</span></button>
  <button onclick="showTab('report')" id="navReport"><span>📄</span><span data-i18n="report">Report</span></button>
</div>
<script>
// --- LANGUAGE SYSTEM ---
let LANG = localStorage.getItem("ajira_lang") || "en";
const I18N = {
en:{
headerTitle:"LEARN • PASS • GET LICENCE • GET JOB", headerSub:"Courses • Quiz • Certificate • ID • M-Pesa • Jobs",
welcome:"Welcome to Ajira Driving School", iAmStudent:"I am a Student - I Want to Learn Driving", iAmInstructor:"I am an Instructor / Admin",
roleInstructor:"Instructor - Driving Teacher", roleAdmin:"Admin - Ajira Driving School", roleOCS:"OCS / MT Officer",
login:"Login", loginHint:"Student: Name + Phone only.<br>Instructor Demo: Any name + any number",
hello:"Hello", logout:"Logout", courses:"Courses", students:"Students", passed:"Passed", paid:"Paid", balance:"Balance",
enroll:"Enroll", quiz:"Quiz", idCard:"ID Card", lessons:"Lessons", payments:"Payments", exam:"Exam", jobs:"Jobs", report:"Report",
addCourse:"+ Add New Course (Admin Only)", addCourseBtn:"Add Course", searchCourse:"Search course: B, C, PSV...",
enrollNow:"📝 Enroll Now", selectCourse:"Select Course *", male:"Male", female:"Female",
noLicence:"No Licence - Complete Beginner", haveLicence:"Have Licence - Want to Add Class", expiredLicence:"Licence Expired - Refresher",
morning:"Morning - 8am - 11am", midday:"Midday - 11am - 2pm", afternoon:"Afternoon - 2pm - 5pm", weekend:"Weekend Only - Sat / Sun",
payMpesa:"PAY WITH M-PESA - STK PUSH", stkHint:"Enter phone, enter amount, tap Pay. You will get a prompt on your phone to enter your M-Pesa PIN.",
payMpesaBtn:"Pay with M-Pesa - STK Push", alreadyPaid:"Or if you already paid:", enrollBtn:"Enroll →",
all:"All", enrolled:"Enrolled", inTraining:"In Training", readyTest:"Ready for Test", failed:"Failed", dropped:"Dropped",
quizTitle:"Practice Quiz - 50 Question Bank", quizSub:"10 random questions every time. Pass 70%+ to be ready for NTSA.",
bestScore:"Your best score:", attempts:"Attempts:", quizMixed:"Mixed - All Topics", quizRules:"Traffic Rules", quizSigns:"Road Signs", quizSafety:"Safety + Defensive", startQuiz:"Start Quiz",
idCardTitle:"Student ID Card", idHint:"Your ID card appears automatically. Admin sees all students.",
scheduleLesson:"+ Schedule Lesson (Instructor Only)", student:"Student", lessonRoad:"Practical - Driving on Road", lessonParking:"Practical - Parking / Yard", lessonTheory:"Theory - Traffic Rules", lessonSigns:"Theory - Road Signs", lessonMock:"Mock Test - Practice Exam", scheduleBtn:"Schedule Lesson",
payTitle:"Pay / Record Payment", recordPayment:"Record Payment", payNow:"Pay Now", sendStk:"Send STK Push",
recordExam:"+ Record Exam Result (Instructor Only)", mockTest:"Mock Test - School", defensiveTest:"Defensive Driving Test",
passedOpt:"Passed ✅", failedOpt:"Failed ❌ - Repeat", absentOpt:"Absent - Did Not Attend", recordResult:"Record Result",
jobsAfter:"Jobs After Passing", schoolReport:"School Report", genReport:"Generate Report PDF", shareWA:"Share via WhatsApp",
footer:"Learn • Pass • Get Job • EN / SW",
ph:{fullName:"Full Name *", phone:"Phone e.g. 0712345678", idNo:"ID No.", instructorName:"Instructor / Officer Name", staffNo:"Staff / Service No.", courseEx:"Course e.g. Class B - Small Car", price:"Price e.g. 18000", duration:"Duration e.g. 4 Weeks / 20 Lessons", instructor:"Instructor", vehicle:"Training Vehicle e.g. KDJ 123A - Probox", desc:"Description...", searchStudent:"Search name, phone...", age:"Age", county:"County e.g. Trans Nzoia", education:"Education e.g. KCSE C-", licenceNo:"Licence No. (If you have one)", mpesaPhone:"M-Pesa Phone e.g. 0712345678", deposit:"Deposit Ksh e.g. 5000", mpesaCode:"M-Pesa Code e.g. QK123ABC", amount:"Amount Ksh", receipt:"M-Pesa Code / Receipt No.", score:"Score % e.g. 85", comments:"Instructor comments...", location:"Location e.g. Eldoret - Yard"}
},
sw:{
headerTitle:"JIFUNZE • FAULU • PATA LESENI • PATA KAZI", headerSub:"Kozi • Quiz • Cheti • ID • M-Pesa • Ajira",
welcome:"Karibu Ajira Driving School", iAmStudent:"Mimi ni Mwanafunzi - Nataka Kujifunza Kuendesha", iAmInstructor:"Mimi ni Mwalimu / Admin",
roleInstructor:"Mwalimu - Mwalimu wa Udereva", roleAdmin:"Admin - Ajira Driving School", roleOCS:"OCS / Afisa MT",
login:"Ingia", loginHint:"Mwanafunzi: Jina + Simu tu.<br>Mwalimu Demo: Jina lolote + Namba lolote",
hello:"Habari", logout:"Toka", courses:"Kozi", students:"Wanafunzi", passed:"Wamefaulu", paid:"Amelipa", balance:"Deni",
enroll:"Jiandikishe", quiz:"Quiz", idCard:"Kadi ya ID", lessons:"Masomo", payments:"Malipo", exam:"Mtihani", jobs:"Ajira", report:"Ripoti",
addCourse:"+ Ongeza Kozi Mpya (Admin Tu)", addCourseBtn:"Ongeza Kozi", searchCourse:"Tafuta kozi: B, C, PSV...",
enrollNow:"📝 Jiandikishe Sasa", selectCourse:"Chagua Kozi *", male:"Kiume", female:"Kike",
noLicence:"Sina Leseni - Mgeni Kabisa", haveLicence:"Nina Leseni - Nataka Kuongeza Class", expiredLicence:"Leseni Ime-expire - Refresher",
morning:"Asubuhi - 8am - 11am", midday:"Mchana - 11am - 2pm", afternoon:"Jioni - 2pm - 5pm", weekend:"Weekend Tu - Sat / Sun",
payMpesa:"LIPA NA M-PESA - STK PUSH", stkHint:"Weka simu, weka kiasi, bonyeza Lipa. Utapata ujumbe kwenye simu yako kuweka M-Pesa PIN.",
payMpesaBtn:"Lipa na M-Pesa - STK Push", alreadyPaid:"Au kama umeshalipa:", enrollBtn:"Jiandikishe →",
all:"Wote", enrolled:"Amejiandikisha", inTraining:"Mafunzoni", readyTest:"Tayari kwa Mtihani", failed:"Amefail", dropped:"Ameacha",
quizTitle:"Quiz ya Mazoezi - Maswali 50", quizSub:"Maswali 10 random kila mara. Faulu 70%+ ili uwe tayari kwa NTSA.",
bestScore:"Alama yako bora:", attempts:"Mara uliyojaribu:", quizMixed:"Mchanganyiko - Zote", quizRules:"Sheria za Barabara", quizSigns:"Alama za Barabara", quizSafety:"Usalama + Defensive", startQuiz:"Anza Quiz",
idCardTitle:"Kadi ya Mwanafunzi", idHint:"Kadi yako inaonekana yenyewe. Admin anaona wanafunzi wote.",
scheduleLesson:"+ Panga Somo (Mwalimu Tu)", student:"Mwanafunzi", lessonRoad:"Practical - Kuendesha Barabarani", lessonParking:"Practical - Parking / Yard", lessonTheory:"Theory - Sheria za Barabara", lessonSigns:"Theory - Alama za Barabara", lessonMock:"Mock Test - Mtihani wa Mazoezi", scheduleBtn:"Panga Somo",
payTitle:"Lipa / Rekodi Malipo", recordPayment:"Rekodi Malipo", payNow:"Lipa Sasa", sendStk:"Tuma STK Push",
recordExam:"+ Rekodi Matokeo ya Mtihani (Mwalimu Tu)", mockTest:"Mock Test - Shule", defensiveTest:"Mtihani wa Defensive Driving",
passedOpt:"Amefaulu ✅", failedOpt:"Amefail ❌ - Rudia", absentOpt:"Hayupo - Hakufika", recordResult:"Rekodi Matokeo",
jobsAfter:"Ajira Baada ya Kufaulu", schoolReport:"Ripoti ya Shule", genReport:"Tengeneza Ripoti PDF", shareWA:"Share kupitia WhatsApp",
footer:"Jifunze • Faulu • Pata Kazi • EN / SW",
ph:{fullName:"Jina Kamili *", phone:"Simu e.g. 0712345678", idNo:"Namba ya ID", instructorName:"Jina la Mwalimu / Afisa", staffNo:"Namba ya Staff / Service", courseEx:"Kozi e.g. Class B - Gari Ndogo", price:"Bei e.g. 18000", duration:"Muda e.g. Wiki 4 / Masomo 20", instructor:"Mwalimu", vehicle:"Gari la Mafunzo e.g. KDJ 123A - Probox", desc:"Maelezo...", searchStudent:"Tafuta jina, simu...", age:"Umri", county:"County e.g. Trans Nzoia", education:"Elimu e.g. KCSE C-", licenceNo:"Namba ya Leseni (Kama unayo)", mpesaPhone:"Simu ya M-Pesa e.g. 0712345678", deposit:"Deposit Ksh e.g. 5000", mpesaCode:"M-Pesa Code e.g. QK123ABC", amount:"Kiasi Ksh", receipt:"M-Pesa Code / Risiti No.", score:"Alama % e.g. 85", comments:"Maoni ya mwalimu...", location:"Mahali e.g. Eldoret - Yard"}
}
};
function setLang(l){ LANG=l; localStorage.setItem("ajira_lang",l); document.getElementById("btnEN").classList.toggle("active",l==="en"); document.getElementById("btnSW").classList.toggle("active",l==="sw"); applyLang(); renderAll(); }
function applyLang(){
  let d=I18N[LANG];
  document.querySelectorAll("[data-i18n]").forEach(el=>{ let k=el.getAttribute("data-i18n"); if(d[k]) el.innerHTML=d[k]; });
  document.querySelectorAll("[data-ph]").forEach(el=>{ let k=el.getAttribute("data-ph"); if(d.ph[k]) el.placeholder=d.ph[k]; });
  // Quiz questions also switch
  if(window.QUIZ_BANK) QUIZ_BANK = LANG==="sw" ? QUIZ_BANK_SW : QUIZ_BANK_EN;
}
function t(en,sw){ return LANG==="sw"?sw:en; }

// --- QUIZ BANKS EN + SW ---
const QUIZ_BANK_EN=[
{q:"What distance should you keep from the vehicle in front?",cat:"safety",opts:["1 metre only","2 seconds rule - keep 2 seconds gap","Very close","Does not matter"],a:1,exp:"Use the 2-second rule."},
{q:"What does a red octagon STOP sign mean?",cat:"signs",opts:["Slow down","Stop completely, look, then go","Continue","Hoot only"],a:1,exp:"STOP = Stop completely."},
{q:"What is the legal alcohol limit for a driver in Kenya?",cat:"rules",opts:["A little is okay","0 - Do not drink at all when driving","2 beers is okay","At night only"],a:1,exp:"Do not drink at all when driving."},
{q:"You want to turn right, what do you do first?",cat:"rules",opts:["Turn immediately","Mirror, Indicator, Blind Spot, Turn","Hoot and turn","Brake suddenly"],a:1,exp:"Mirror - Signal - Blind Spot."},
{q:"What does a yellow triangle sign mean?",cat:"signs",opts:["Warning - danger ahead","Stop","High speed","Parking"],a:0,exp:"Yellow triangle = Warning."},
{q:"Heavy rain is falling, what do you do?",cat:"safety",opts:["Drive fast","Slow down, switch on lights, increase gap","Switch off lights","Drive in the middle"],a:1,exp:"Rain = slow down, lights on."},
{q:"A child is crossing without looking, what do you do?",cat:"safety",opts:["Hoot and continue","Slow down / Stop, give way","Shout at them","Pass quickly"],a:1,exp:"Children have priority - stop."},
{q:"At a red traffic light, what do you do?",cat:"rules",opts:["Go if no car","Stop completely until green","Pass slowly","Turn only"],a:1,exp:"Red = Stop."},
{q:"A red circle with 50 inside means?",cat:"signs",opts:["Distance is 50km","Maximum speed is 50 km/h","50 people","Parking 50"],a:1,exp:"Speed limit."},
{q:"Before a journey, what should you check?",cat:"safety",opts:["Fuel, tyres, brakes, lights, water","Radio only","Car colour","Does not matter"],a:0,exp:"Check fuel, tyres, brakes, lights."},
{q:"At night with other vehicles, which lights do you use?",cat:"rules",opts:["Full light always","Dim / Low beam","Switch off lights","Hazard only"],a:1,exp:"Night + other cars = dim light."},
{q:"You feel very tired while driving, what do you do?",cat:"safety",opts:["Continue","Stop, rest / change driver","Drink alcohol","Open window only"],a:1,exp:"Tiredness = Stop and rest."},
{q:"What is a zebra crossing for?",cat:"signs",opts:["Cars to park","Pedestrians to cross","Motorcycles to pass","Selling goods"],a:1,exp:"Zebra = pedestrians cross."},
{q:"An ambulance is behind you with siren, what do you do?",cat:"rules",opts:["Continue","Give way - move aside immediately","Follow closely","Stop in the middle"],a:1,exp:"Emergency vehicle = give way."},
{q:"Who must wear a helmet on a motorcycle?",cat:"safety",opts:["Driver only","Driver + all passengers","Not necessary","Children only"],a:1,exp:"Driver + all passengers."},
];
const QUIZ_BANK_SW=[
{q:"Ukiendesha, umbali gani unatakiwa kuacha na gari la mbele?",cat:"safety",opts:["Mita 1 tu","Mita 2 - Kanuni ya sekunde 2","Karibu sana","Haijalishi"],a:1,exp:"Tumia kanuni ya sekunde 2."},
{q:"Alama nyekundu ya octagon (STOP) inamaanisha?",cat:"signs",opts:["Punguza mwendo","Simama kabisa, angalia, endelea","Endelea","Honi tu"],a:1,exp:"STOP = Simama kabisa."},
{q:"Kiwango cha pombe kinachoruhusiwa kwa dereva?",cat:"rules",opts:["Kidogo sawa","0 - Usinywe kabisa ukiendesha","Bia 2 sawa","Usiku tu"],a:1,exp:"Usinywe kabisa."},
{q:"Unataka kugeuka kulia, unafanya nini kwanza?",cat:"rules",opts:["Geuka mara moja","Kioo, Indicator, Blind Spot, Geuka","Honi na ugeuke","Breki ghafla"],a:1,exp:"Kioo - Ishara - Blind Spot."},
{q:"Alama ya njano ya pembetatu inamaanisha?",cat:"signs",opts:["Tahadhari - hatari mbele","Simama","Mbio za juu","Parking"],a:0,exp:"Pembetatu njano = Onyo."},
{q:"Mvua kubwa, unafanya nini?",cat:"safety",opts:["Endesha haraka","Punguza mwendo, washa taa, ongeza umbali","Zima taa","Pita katikati"],a:1,exp:"Mvua = punguza mwendo."},
{q:"Mtoto anavuka bila kuangalia, unafanya?",cat:"safety",opts:["Honi na uendelee","Punguza / Simama, mpe nafasi","Mpigie kelele","Mpite kwa kasi"],a:1,exp:"Watoto wana kipaumbele."},
{q:"Taa nyekundu (red light) unafanya?",cat:"rules",opts:["Endelea kama hakuna gari","Simama mpaka iwe kijani","Pita polepole","Geuka tu"],a:1,exp:"Nyekundu = Simama."},
{q:"Mduara mwekundu na 50 ndani inamaanisha?",cat:"signs",opts:["Umbali 50km","Kasi ya juu ni 50 km/h","Watu 50","Parking 50"],a:1,exp:"Kikomo cha kasi."},
{q:"Kabla ya safari, unaangalia nini?",cat:"safety",opts:["Mafuta, matairi, breki, taa, maji","Radio tu","Rangi ya gari","Haijalishi"],a:0,exp:"Angalia mafuta, matairi, breki."},
{q:"Usiku na magari mengine, unatumia taa gani?",cat:"rules",opts:["Full light daima","Dim / Low beam","Zima taa","Hazard tu"],a:1,exp:"Usiku = Dim light."},
{q:"Ukichoka sana ukiendesha, unafanya?",cat:"safety",opts:["Endelea","Simama, pumzika / badilisha dereva","Kunywa pombe","Fungua dirisha tu"],a:1,exp:"Uchovu = Simama pumzika."},
{q:"Zebra crossing ni kwa ajili ya?",cat:"signs",opts:["Magari kupaki","Watangatangaji kuvuka","Pikipiki","Kuuzia bidhaa"],a:1,exp:"Zebra = watembea kuvuka."},
{q:"Ambulansi nyuma yako na sauti, unafanya?",cat:"rules",opts:["Endelea","Pisha - sogea pembeni mara moja","Mfuate karibu","Simama katikati"],a:1,exp:"Gari la dharura = mpe nafasi."},
{q:"Helmet kwa pikipiki ni ya nani?",cat:"safety",opts:["Dereva tu","Dereva + abiria wote","Si lazima","Watoto tu"],a:1,exp:"Dereva + abiria wote."},
];
let QUIZ_BANK = QUIZ_BANK_EN;

let deferredPrompt=null;
window.addEventListener('beforeinstallprompt', e=>{ e.preventDefault(); deferredPrompt=e; document.getElementById('installBtn').classList.remove('hidden'); });
function installApp(){ if(deferredPrompt){ deferredPrompt.prompt(); deferredPrompt.userChoice.then(r=>{ if(r.outcome==='accepted') document.getElementById('installBtn').classList.add('hidden'); deferredPrompt=null; }); } else { alert(t("To Install:\nAndroid: Menu (⋮) → Add to Home Screen\n\niPhone: Share (⬆️) → Add to Home Screen","Kuweka App:\nAndroid: Menu (⋮) → Add to Home Screen\n\niPhone: Share (⬆️) → Add to Home Screen")); } }
if('serviceWorker' in navigator){ navigator.serviceWorker.register('sw.js').catch(()=>{}); }
let courses = JSON.parse(localStorage.getItem("ajira_ds_courses")||"[]");
let students = JSON.parse(localStorage.getItem("ajira_ds_students")||"[]");
let lessons = JSON.parse(localStorage.getItem("ajira_ds_lessons")||"[]");
let payments = JSON.parse(localStorage.getItem("ajira_ds_payments")||"[]");
let exams = JSON.parse(localStorage.getItem("ajira_ds_exams")||"[]");
let quizHistory = JSON.parse(localStorage.getItem("ajira_ds_quiz")||"[]");
let currentUser=null, isAdmin=false, quizQuestions=[], quizIndex=0, quizScore=0, quizAnswers=[];
function getToday(){ return new Date().toISOString().slice(0,10); }
function getCurrentMonth(){ return new Date().toISOString().slice(0,7); }
function toggleLogin(){ let tt=document.getElementById("userType").value; document.getElementById("studentLogin").classList.toggle("hidden", tt!=="student"); document.getElementById("instructorLogin").classList.toggle("hidden", tt!=="student"); }
function login(){
  let type=document.getElementById("userType").value;
  if(type==="student"){ let name=document.getElementById("stuName").value.trim(); let phone=document.getElementById("stuPhone").value.trim(); let id=document.getElementById("stuId").value.trim(); if(!name||!phone) return alert(t("Enter Name and Phone","Jaza Jina na Simu")); currentUser={name,phone,id,role:t("Student","Mwanafunzi")}; isAdmin=false; }
  else { let name=document.getElementById("offName").value.trim(); let no=document.getElementById("offNo").value.trim(); let role=document.getElementById("offRole").value; if(!name||!no) return alert(t("Enter Name and Staff No.","Jaza Jina na Staff No.")); currentUser={name,no,role,station:"Ajira Driving School - Eldoret"}; isAdmin=true; }
  document.getElementById("loginView").classList.add("hidden"); document.getElementById("appView").classList.remove("hidden"); document.getElementById("bottomNav").style.display="flex";
  document.getElementById("userName").innerText=currentUser.name+" ("+currentUser.role+")"; document.getElementById("stationLabel").innerText=currentUser.station||t("Student","Mwanafunzi"); document.getElementById("dateLabel").innerText=new Date().toLocaleDateString();
  document.getElementById("adminCourseForm").classList.toggle("hidden", !isAdmin); document.getElementById("adminLessonForm").classList.toggle("hidden", !isAdmin); document.getElementById("adminExamForm").classList.toggle("hidden", !isAdmin);
  if(courses.length===0){
    courses=[{id:1,title:t("Class B - Small Car / Probox","Class B - Gari Ndogo / Probox"),cls:"Class B",price:18000,duration:t("4 Weeks / 20 Lessons","Wiki 4 / Masomo 20"),instructor:"Instr. David Otieno",vehicle:"KDJ 123A - Probox",desc:t("Theory + Practical, Parking, Town, NTSA Test.","Theory + Practical, Parking, Town, NTSA Test."),createdAt:new Date().toISOString()},{id:2,title:t("Class C - Lorry","Class C - Lorry"),cls:"Class C",price:25000,duration:t("5 Weeks / 25 Lessons","Wiki 5 / Masomo 25"),instructor:"Instr. Peter Kamau",vehicle:"KDJ 456B - Lorry",desc:t("Lorry, Reversing, Highway.","Lorry, Reversing, Highway."),createdAt:new Date().toISOString()},{id:3,title:t("Class D - Bus / PSV","Class D - Bus / PSV"),cls:"Class D",price:28000,duration:t("6 Weeks / 30 Lessons","Wiki 6 / Masomo 30"),instructor:"Instr. Jane Wanjiru",vehicle:"KDJ 789C - Bus",desc:t("Bus + PSV, Safety, NTSA PSV.","Bus + PSV, Safety, NTSA PSV."),createdAt:new Date().toISOString()},{id:4,title:t("Class A - Motorcycle","Class A - Pikipiki"),cls:"Class A",price:12000,duration:t("3 Weeks / 15 Lessons","Wiki 3 / Masomo 15"),instructor:"Instr. Mary Achieng",vehicle:"KMDA 101 - Honda",desc:t("Motorcycle, Traffic, Helmet.","Pikipiki, Traffic, Helmet."),createdAt:new Date().toISOString()},{id:5,title:t("Class B+C - Car + Lorry","Class B+C - Gari + Lorry"),cls:"Class B+C",price:35000,duration:t("8 Weeks / 40 Lessons","Wiki 8 / Masomo 40"),instructor:"Instr. David Otieno",vehicle:"KDJ 123A + KDJ 456B",desc:t("Combo - Best for NPS Driver Jobs!","Combo - Best kwa Ajira NPS!"),createdAt:new Date().toISOString()},{id:6,title:t("Defensive Driving - NPS Driver","Defensive Driving - Dereva wa NPS"),cls:"Defensive",price:15000,duration:t("2 Weeks / 10 Lessons","Wiki 2 / Masomo 10"),instructor:"Instr. Peter Kamau",vehicle:"KDJ 123A",desc:t("Defensive, Fuel saving.","Defensive, Fuel saving."),createdAt:new Date().toISOString()}];
    localStorage.setItem("ajira_ds_courses",JSON.stringify(courses));
    students=[{id:1,name:"John Kiprop",phone:"0711111111",idNo:"40111111",age:24,gender:t("Male","Kiume"),county:"Trans Nzoia",education:"KCSE C-",courseId:1,courseTitle:courses[0].title,coursePrice:18000,hasLicence:t("No Licence - Complete Beginner","Sina Leseni - Mgeni Kabisa"),licenceNo:"",schedule:t("Morning - 8am - 11am","Asubuhi - 8am - 11am"),status:"In Training",lessonsDone:12,totalPaid:12000,photo:"",officer:"Admin",createdAt:new Date().toISOString(),day:getToday()},{id:2,name:"Faith Chebet",phone:"0722222222",idNo:"40222222",age:22,gender:t("Female","Kike"),county:"Uasin Gishu",education:"KCSE C",courseId:5,courseTitle:courses[4].title,coursePrice:35000,hasLicence:t("No Licence - Complete Beginner","Sina Leseni - Mgeni Kabisa"),licenceNo:"",schedule:t("Midday - 11am - 2pm","Mchana - 11am - 2pm"),status:"Ready for Test",lessonsDone:38,totalPaid:35000,photo:"",officer:"Admin",createdAt:new Date().toISOString(),day:getToday()},{id:3,name:"Kevin Barasa",phone:"0733333333",idNo:"40333333",age:28,gender:t("Male","Kiume"),county:"Bungoma",education:"KCSE C-",courseId:2,courseTitle:courses[1].title,coursePrice:25000,hasLicence:t("Have Licence - Want to Add Class","Nina Leseni - Nataka Kuongeza Class"),licenceNo:"DL999111",schedule:t("Afternoon - 2pm - 5pm","Jioni - 2pm - 5pm"),status:"Passed",lessonsDone:25,totalPaid:25000,photo:"",officer:"Admin",createdAt:new Date().toISOString(),day:getToday()}];
    localStorage.setItem("ajira_ds_students",JSON.stringify(students));
    payments=[{id:1,studentId:1,name:"John Kiprop",amount:5000,method:"M-Pesa",code:"QK111AAA",date:getToday(),officer:"Admin"},{id:2,studentId:1,name:"John Kiprop",amount:7000,method:"M-Pesa",code:"QK222BBB",date:getToday(),officer:"Admin"},{id:3,studentId:2,name:"Faith Chebet",amount:35000,method:"M-Pesa",code:"QK333CCC",date:getToday(),officer:"Admin"},{id:4,studentId:3,name:"Kevin Barasa",amount:25000,method:"Cash",code:"REC001",date:getToday(),officer:"Admin"}];
    localStorage.setItem("ajira_ds_payments",JSON.stringify(payments));
    exams=[{id:1,studentId:3,name:"Kevin Barasa",type:"NTSA Practical Test",score:88,result:t("Passed ✅","Amefaulu ✅"),date:getToday(),notes:t("Very good, clean parking","Vizuri sana"),officer:"Instr. Peter Kamau"},{id:2,studentId:2,name:"Faith Chebet",type:t("Mock Test - School","Mock Test - Shule"),score:92,result:t("Passed ✅","Amefaulu ✅"),date:getToday(),notes:t("Ready for NTSA","Tayari kwa NTSA"),officer:"Instr. David Otieno"}];
    localStorage.setItem("ajira_ds_exams",JSON.stringify(exams));
  }
  if(!isAdmin){ document.getElementById("eName").value=currentUser.name; document.getElementById("ePhone").value=currentUser.phone; document.getElementById("eId").value=currentUser.id||""; document.getElementById("eMpesaPhone").value=currentUser.phone; }
  if(document.getElementById("reportMonth")) document.getElementById("reportMonth").value=getCurrentMonth();
  applyLang(); renderAll(); renderIDCard();
}
function logout(){ location.reload(); }
function showTab(tt){
  ["courses","enroll","students","quiz","id","lessons","payments","exam","jobs","report","cert"].forEach(k=>{ let el=document.getElementById(k+"Tab"); if(el) el.classList.toggle("hidden",k!==tt); });
  ["Courses","Enroll","Students","Quiz","ID","Lessons","Payments","Exam","Jobs","Report"].forEach(k=>{ let el=document.getElementById("tab"+k); if(el) el.classList.toggle("active",k.toLowerCase()===tt); });
  ["Courses","Enroll","Students","Quiz","ID","Lessons","Payments","Exam","Jobs","Report"].forEach(k=>{let el=document.getElementById("nav"+k); if(el) el.classList.toggle("active",k.toLowerCase()===tt);});
  if(tt==="id") renderIDCard();
  renderAll(); window.scrollTo({top:0,behavior:"smooth"});
}
function stkPushEnroll(){
  let phone=document.getElementById("eMpesaPhone").value.trim()||document.getElementById("ePhone").value.trim(); let amount=parseInt(document.getElementById("eDeposit").value||0);
  if(!phone||!amount) return alert(t("Enter M-Pesa Phone and Amount","Weka Simu ya M-Pesa na Kiasi"));
  let btn=event.target; btn.innerText=t("⏳ Sending STK Push...","⏳ Tumatuma STK Push..."); btn.disabled=true;
  setTimeout(()=>{ btn.innerText="💚 "+t("Pay with M-Pesa - STK Push","Lipa na M-Pesa - STK Push"); btn.disabled=false; let code="QK"+Math.random().toString(36).substring(2,8).toUpperCase(); document.getElementById("eMpesaCode").value=code; alert(t(`💚 STK PUSH SENT!\n\nPhone: ${phone}\nAmount: Ksh ${amount.toLocaleString()}\n\n1. Check your phone\n2. Enter M-Pesa PIN\n3. Press OK\n\nCode: ${code}`,`💚 STK PUSH IMETUMWA!\n\nSimu: ${phone}\nKiasi: Ksh ${amount.toLocaleString()}\n\n1. Angalia simu yako\n2. Weka M-Pesa PIN\n3. Bonyeza OK\n\nCode: ${code}`)); },1500);
}
function stkPushPayment(){
  let phone=document.getElementById("pMpesaPhone").value.trim(); let amount=parseInt(document.getElementById("pAmount").value||0);
  if(!phone||!amount) return alert(t("Enter Phone and Amount","Weka Simu na Kiasi"));
  setTimeout(()=>{ let code="QK"+Math.random().toString(36).substring(2,8).toUpperCase(); document.getElementById("pCode").value=code; alert(t(`💚 STK PUSH SENT!\nPhone: ${phone}\nAmount: Ksh ${amount.toLocaleString()}\nCode: ${code}`,`💚 STK PUSH IMETUMWA!\nSimu: ${phone}\nKiasi: Ksh ${amount.toLocaleString()}\nCode: ${code}`)); },800);
}
function startQuiz(){ let type=document.getElementById("quizType").value; let pool=type==="all"?[...QUIZ_BANK]:QUIZ_BANK.filter(q=>q.cat===type); pool=pool.sort(()=>Math.random()-0.5).slice(0,10); quizQuestions=pool; quizIndex=0; quizScore=0; quizAnswers=[]; document.getElementById("quizResult").innerHTML=""; renderQuizQuestion(); }
function renderQuizQuestion(){ if(quizIndex>=quizQuestions.length){ finishQuiz(); return; } let q=quizQuestions[quizIndex]; document.getElementById("quizArea").innerHTML=`<div class="card"><div class="top"><b>${t("Question","Swali")} ${quizIndex+1} / ${quizQuestions.length}</b><span class="badge">${quizScore} ${t("Correct","Sahihi")}</span></div><div class="bar"><div class="fill" style="width:${quizIndex/quizQuestions.length*100}%"></div></div><h3 style="font-size:17px;line-height:1.4">${q.q}</h3>${q.opts.map((o,i)=>`<button class="quiz-opt" onclick="answerQuiz(${i})">${["A","B","C","D"][i]}. ${o}</button>`).join("")}</div>`; }
function answerQuiz(i){ let q=quizQuestions[quizIndex]; let correct=i===q.a; if(correct) quizScore++; quizAnswers.push({q:q.q, chosen:q.opts[i], correct:q.opts[q.a], isCorrect:correct, exp:q.exp}); let btns=document.querySelectorAll(".quiz-opt"); btns.forEach((b,idx)=>{ if(idx===q.a) b.classList.add("correct"); else if(idx===i) b.classList.add("wrong"); b.disabled=true; }); document.getElementById("quizArea").innerHTML+=`<div class="card" style="background:${correct?"#e8f5e9":"#ffebee"}"><b>${correct?t("✅ Correct!","✅ Sahihi!"):t("❌ Wrong.","❌ Sio sahihi.")}</b><br>${q.exp}<br><button class="green" onclick="nextQuiz()">${t("Next Question →","Swali Linalofuata →")}</button></div>`; }
function nextQuiz(){ quizIndex++; renderQuizQuestion(); }
function finishQuiz(){ let total=quizQuestions.length; let pct=Math.round(quizScore/total*100); let passed=pct>=70; quizHistory.unshift({name:currentUser?currentUser.name:"",phone:currentUser?currentUser.phone:"",score:pct,correct:quizScore,total,date:getToday(),createdAt:new Date().toISOString()}); localStorage.setItem("ajira_ds_quiz",JSON.stringify(quizHistory)); let review=quizAnswers.map((a,i)=>`<div class="card" style="border-left:5px solid ${a.isCorrect?"#1a7a3a":"#b71c1c"}"><b>${i+1}. ${a.q}</b><br>${t("You answered:","Ulijibu:")} ${a.chosen} ${a.isCorrect?"✅":"❌"}<br>${!a.isCorrect?`${t("Correct Answer:","Jibu Sahihi:")} <b>${a.correct}</b><br>`:""}<span class="small">${a.exp}</span></div>`).join(""); document.getElementById("quizArea").innerHTML=""; document.getElementById("quizResult").innerHTML=`<div class="card" style="background:${passed?"#e8f5e9":"#ffebee"};border:2px solid ${passed?"#1a7a3a":"#b71c1c"}"><h2 style="text-align:center;margin:0">${passed?t("🎉 YOU PASSED!","🎉 UMEFAULU!"):t("😔 YOU FAILED - Try Again","😔 UMEFAIL - Jaribu Tena")}</h2><p style="text-align:center;font-size:22px"><b>${quizScore}/${total} = ${pct}%</b></p><p style="text-align:center">${passed?t("You are ready for NTSA Theory Test!","Uko tayari kwa NTSA Theory Test!"):t("You need 70%+ to pass.","Unahitaji 70%+ ili ufaulu.")}</p><button class="green" onclick="startQuiz()">${t("🔁 Try Again","🔁 Jaribu Tena")}</button><button class="secondary" onclick="shareQuizResult(${pct})">${t("Share Result WhatsApp","Share Matokeo WhatsApp")}</button></div>${review}`; renderAll(); }
function shareQuizResult(pct){ let txt=t(`🧠 Ajira Driving School - Quiz\nName: ${currentUser?currentUser.name:""}\nScore: ${pct}%\n${pct>=70?"✅ I passed!":"❌ I will try again"}`,`🧠 Ajira Driving School - Quiz\nJina: ${currentUser?currentUser.name:""}\nAlama: ${pct}%\n${pct>=70?"✅ Nimefaulu!":"❌ Najaribu tena"}`); window.open("https://wa.me/?text="+encodeURIComponent(txt),"_blank"); }
function renderIDCard(){
  let list=!isAdmin?students.filter(s=>s.phone===currentUser?.phone):students;
  if(list.length===0){ document.getElementById("idCardArea").innerHTML="<p class='small'>"+t("You have not enrolled yet. Enroll first to get your ID Card.","Hujajiandikisha bado. Jiandikishe kwanza ili upate ID Card.")+"</p>"; return; }
  document.getElementById("idCardArea").innerHTML=list.map(s=>{ let initials=s.name.split(" ").map(w=>w[0]).join("").slice(0,2).toUpperCase(); let idNo="ADS-"+String(s.id).padStart(4,"0")+"-"+new Date().getFullYear(); let bal=Math.max(0,s.coursePrice-(s.totalPaid||0)); return `<div id="idPrint-${s.id}" class="idcard"><div class="photo">${initials}</div><div style="flex:1"><div style="font-size:11px;opacity:.9">🇰🇪 NPS AJIRA DRIVING SCHOOL</div><div style="font-size:18px;font-weight:900">${s.name.toUpperCase()}</div><div style="font-size:12px">ID: ${idNo} • ${s.courseTitle}<br>${t("Phone:","Simu:")} ${s.phone} • ID No: ${s.idNo}<br>${t("Status:","Status:")} ${s.status} • ${t("Schedule:","Ratiba:")} ${s.schedule}<br>${t("Balance:","Deni:")} Ksh ${bal.toLocaleString()}</div></div><div style="text-align:center;font-size:30px">🪪<div style="font-size:9px">STUDENT</div></div></div><button class="secondary" onclick="printID(${s.id})">🖨️ ${t("Print ID Card","Print Kadi ya ID")}</button><button class="secondary" onclick="shareID('${s.name}','${s.courseTitle}','${idNo}')">${t("Share ID WhatsApp","Share ID WhatsApp")}</button>`; }).join("");
}
function printID(id){ let el=document.getElementById("idPrint-"+id); if(!el) return; let w=window.open("","_blank"); w.document.write(`<html><body style="font-family:Arial;padding:20px">${el.outerHTML}<style>.idcard{width:400px}</style><script>window.onload=()=>window.print()<\/script></body></html>`); w.document.close(); }
function shareID(name,course,idNo){ let txt=t(`🪪 AJIRA DRIVING SCHOOL - STUDENT ID\n\nName: ${name}\nCourse: ${course}\nStudent ID: ${idNo}`,`🪪 AJIRA DRIVING SCHOOL - KADI YA MWANAFUNZI\n\nJina: ${name}\nKozi: ${course}\nStudent ID: ${idNo}`); window.open("https://wa.me/?text="+encodeURIComponent(txt),"_blank"); }
function showCertificate(studentId){ let s=students.find(x=>x.id===studentId); if(!s) return; if(s.status!=="Passed"){ alert(t("Certificate is for passed students only. ","Cheti kwa waliopita tu. ")+s.name+" "+t("is still","bado ni ")+s.status); return; } let exam=exams.find(e=>e.studentId===s.id && e.result.includes("Passed")) || {score:85,type:"NTSA Practical Test"}; let certNo="AJIRA-DS-"+String(s.id).padStart(4,"0")+"-"+new Date().getFullYear(); document.getElementById("certArea").innerHTML=`<div id="certPrint" class="cert"><div>🇰🇪 REPUBLIC OF KENYA</div><h2 style="color:#0b2c4a;margin:5px 0">NPS AJIRA DRIVING SCHOOL</h2><div style="font-size:12px">NTSA APPROVED • Eldoret • Kitale</div><div style="font-size:28px;margin:12px 0">${t("🏆 CERTIFICATE OF COMPLETION","🏆 CHETI CHA KUMALIZA")}</div><hr><p>${t("This is to certify that","Hiki ni kuthibitisha kuwa")}</p><h2 style="margin:5px 0">${s.name.toUpperCase()}</h2><p>ID No: ${s.idNo} • ${t("Phone:","Simu:")} ${s.phone}</p><p>${t("Has completed and PASSED the course","Amemaliza na KUFAULU kozi ya")}</p><h3 style="color:#1a7a3a;margin:5px 0">${s.courseTitle}</h3><p>${t("Exam Score:","Alama ya Mtihani:")} <b>${exam.score}% - ${exam.type}</b><br>${t("Lessons Done:","Masomo Aliyofanya:")} <b>${s.lessonsDone||0}</b> • ${t("Paid:","Amelipa:")} Ksh ${(s.totalPaid||0).toLocaleString()}</p><p>${t("Certificate No:","Cheti No:")} <b>${certNo}</b> • ${t("Date:","Tarehe:")} ${getToday()}</p><br><table style="width:100%"><tr><td>${t("Instructor:","Mwalimu:")}<br><br>______________</td><td>Admin:<br><br>______________</td><td>${t("Stamp:","Muhuri:")}<br><br>______________</td></tr></table></div><button class="green" onclick="printCert()">🖨️ ${t("Print / Save Certificate PDF","Print / Save Cheti PDF")}</button><button class="secondary" onclick="shareCert('${s.name}','${s.courseTitle}','${certNo}')">${t("Share Certificate WhatsApp","Share Cheti WhatsApp")}</button><button class="secondary" onclick="showTab('students')">← ${t("Back","Rudi")}</button>`; showTab('cert'); }
function printCert(){ let c=document.getElementById("certPrint")?.innerHTML; if(!c) return alert(t("Generate certificate first","Tengeneza cheti kwanza")); let w=window.open("","_blank"); w.document.write(`<html><body style="font-family:Arial;padding:20px">${c}<script>window.onload=()=>window.print()<\/script></body></html>`); w.document.close(); }
function shareCert(name,course,certNo){ let txt=t(`🏆 CERTIFICATE - Ajira Driving School\n\nCongratulations ${name}!\nYou completed and passed: ${course}\nCertificate No: ${certNo}`,`🏆 CHETI - Ajira Driving School\n\nHongera ${name}!\nUmemaliza na kufaulu: ${course}\nCheti No: ${certNo}`); window.open("https://wa.me/?text="+encodeURIComponent(txt),"_blank"); }
function saveCourse(){ if(!isAdmin) return alert(t("Admin only","Admin tu")); let title=document.getElementById("cTitle").value.trim(); let cls=document.getElementById("cClass").value; let price=parseInt(document.getElementById("cPrice").value||0); let duration=document.getElementById("cDuration").value.trim(); let instructor=document.getElementById("cInstructor").value.trim(); let vehicle=document.getElementById("cVehicle").value.trim(); let desc=document.getElementById("cDesc").value.trim(); if(!title||!price) return alert(t("Enter Course and Price","Jaza Kozi na Bei")); courses.unshift({id:Date.now(),title,cls,price,duration,instructor,vehicle,desc,createdAt:new Date().toISOString()}); localStorage.setItem("ajira_ds_courses",JSON.stringify(courses)); ["cTitle","cPrice","cDuration","cInstructor","cVehicle","cDesc"].forEach(id=>document.getElementById(id).value=""); alert(t(`Course Added: ${title}`,`Kozi Imeongezwa: ${title}`)); renderAll(); }
function quickEnroll(courseId){ showTab('enroll'); document.getElementById("eCourse").value=courseId; updateEnrollInfo(); window.scrollTo({top:0,behavior:"smooth"}); }
function updateEnrollInfo(){ let id=document.getElementById("eCourse").value; let c=courses.find(x=>x.id==id); if(!c) return; document.getElementById("eCourseInfo").innerHTML=`<b>${c.title}</b><br>${t("Price:","Bei:")} <b>Ksh ${c.price.toLocaleString()}</b> • ${t("Duration:","Muda:")} ${c.duration}<br>${t("Instructor:","Mwalimu:")} ${c.instructor} • ${t("Vehicle:","Gari:")} ${c.vehicle}<br>${c.desc}`; }
function enrollStudent(){ let courseId=document.getElementById("eCourse").value; let name=document.getElementById("eName").value.trim(); let phone=document.getElementById("ePhone").value.trim(); let idNo=document.getElementById("eId").value.trim(); let age=document.getElementById("eAge").value; let gender=document.getElementById("eGender").value; let county=document.getElementById("eCounty").value.trim(); let edu=document.getElementById("eEducation").value.trim(); let hasLic=document.getElementById("eHasLicence").value; let licNo=document.getElementById("eLicenceNo").value.trim(); let schedule=document.getElementById("eSchedule").value; let deposit=parseInt(document.getElementById("eDeposit").value||0); let mpesa=document.getElementById("eMpesaCode").value.trim(); if(!courseId||!name||!phone||!idNo) return alert(t("Enter Course, Name, Phone, ID","Jaza Kozi, Jina, Simu, ID")); let course=courses.find(x=>x.id==courseId); if(students.find(s=>s.phone===phone && s.courseId==courseId)) return alert(t("You are already enrolled in this course!","Umeshaandikishwa kwa hii kozi!")); let stu={id:Date.now(),name,phone,idNo,age,gender,county,education:edu,courseId:parseInt(courseId),courseTitle:course.title,coursePrice:course.price,hasLicence:hasLic,licenceNo:licNo,schedule,status:"Enrolled",lessonsDone:0,totalPaid:deposit,photo:"",officer:currentUser.name,createdAt:new Date().toISOString(),day:getToday()}; students.unshift(stu); localStorage.setItem("ajira_ds_students",JSON.stringify(students)); if(deposit>0){ payments.unshift({id:Date.now()+1,studentId:stu.id,name,amount:deposit,method:"M-Pesa",code:mpesa||"DEPOSIT",date:getToday(),officer:currentUser.name}); localStorage.setItem("ajira_ds_payments",JSON.stringify(payments)); } alert(t(`✅ Enrolled!\nCourse: ${course.title}\nPrice: Ksh ${course.price.toLocaleString()}\nPaid: Ksh ${deposit.toLocaleString()}\nBalance: Ksh ${(course.price-deposit).toLocaleString()}`,`✅ Umejiandikisha!\nKozi: ${course.title}\nBei: Ksh ${course.price.toLocaleString()}\nUmelipa: Ksh ${deposit.toLocaleString()}\nDeni: Ksh ${(course.price-deposit).toLocaleString()}`)); showTab('students'); renderAll(); renderIDCard(); }
function changeStudentStatus(id,status){ if(!isAdmin) return alert(t("Instructor only","Mwalimu tu")); let s=students.find(x=>x.id===id); if(!s) return; s.status=status; localStorage.setItem("ajira_ds_students",JSON.stringify(students)); alert(`${s.name} - ${status}`); renderAll(); }
function addLessonDone(id){ if(!isAdmin) return alert(t("Instructor only","Mwalimu tu")); let s=students.find(x=>x.id===id); if(!s) return; s.lessonsDone=(s.lessonsDone||0)+1; if(s.status==="Enrolled") s.status="In Training"; localStorage.setItem("ajira_ds_students",JSON.stringify(students)); renderAll(); }
function saveLesson(){ if(!isAdmin) return alert(t("Instructor only","Mwalimu tu")); let stuId=document.getElementById("lStudent").value; let date=document.getElementById("lDate").value; let time=document.getElementById("lTime").value; let type=document.getElementById("lType").value; let vehicle=document.getElementById("lVehicle").value.trim(); let instructor=document.getElementById("lInstructor").value.trim(); let loc=document.getElementById("lLocation").value.trim(); if(!stuId||!date) return alert(t("Select Student and Date","Chagua Mwanafunzi na Tarehe")); let s=students.find(x=>x.id==stuId); if(!s) return; lessons.unshift({id:Date.now(),studentId:s.id,name:s.name,phone:s.phone,date,time,type,vehicle,instructor,location:loc,status:"Scheduled",officer:currentUser.name,createdAt:new Date().toISOString()}); localStorage.setItem("ajira_ds_lessons",JSON.stringify(lessons)); alert(t(`Lesson Scheduled: ${s.name} - ${type}`,`Somo Limepangwa: ${s.name} - ${type}`)); renderAll(); }
function completeLesson(id){ let l=lessons.find(x=>x.id===id); if(!l) return; l.status="Completed"; localStorage.setItem("ajira_ds_lessons",JSON.stringify(lessons)); let s=students.find(x=>x.id===l.studentId); if(s){ s.lessonsDone=(s.lessonsDone||0)+1; if(s.status==="Enrolled") s.status="In Training"; localStorage.setItem("ajira_ds_students",JSON.stringify(students)); } alert(t(`Lesson Completed: ${l.name}`,`Somo Limekamilika: ${l.name}`)); renderAll(); }
function savePayment(){ let stuId=document.getElementById("pStudent").value; let amount=parseInt(document.getElementById("pAmount").value||0); let method=document.getElementById("pMethod").value; let code=document.getElementById("pCode").value.trim(); if(!stuId||!amount) return alert(t("Select Student and Amount","Chagua Mwanafunzi na Kiasi")); let s=students.find(x=>x.id==stuId); if(!s) return; payments.unshift({id:Date.now(),studentId:s.id,name:s.name,amount,method,code,date:getToday(),officer:currentUser.name}); localStorage.setItem("ajira_ds_payments",JSON.stringify(payments)); s.totalPaid=(s.totalPaid||0)+amount; localStorage.setItem("ajira_ds_students",JSON.stringify(students)); document.getElementById("pAmount").value=""; document.getElementById("pCode").value=""; alert(t(`Payment: ${s.name} - Ksh ${amount.toLocaleString()}\nBalance: Ksh ${Math.max(0,s.coursePrice-s.totalPaid).toLocaleString()}`,`Malipo: ${s.name} - Ksh ${amount.toLocaleString()}\nDeni: Ksh ${Math.max(0,s.coursePrice-s.totalPaid).toLocaleString()}`)); renderAll(); }
function saveExam(){ if(!isAdmin) return alert(t("Instructor only","Mwalimu tu")); let stuId=document.getElementById("xStudent").value; let type=document.getElementById("xType").value; let score=parseInt(document.getElementById("xScore").value||0); let result=document.getElementById("xResult").value; let date=document.getElementById("xDate").value; let notes=document.getElementById("xNotes").value.trim(); if(!stuId) return alert(t("Select Student","Chagua Mwanafunzi")); let s=students.find(x=>x.id==stuId); if(!s) return; exams.unshift({id:Date.now(),studentId:s.id,name:s.name,type,score,result,date,notes,officer:currentUser.name}); localStorage.setItem("ajira_ds_exams",JSON.stringify(exams)); if(result.includes("Passed")||result.includes("Amefaulu")) s.status="Passed"; else if(result.includes("Failed")||result.includes("Amefail")) s.status="Failed"; localStorage.setItem("ajira_ds_students",JSON.stringify(students)); document.getElementById("xScore").value=""; document.getElementById("xNotes").value=""; alert(t(`Result: ${s.name} - ${score}% - ${result}`,`Matokeo: ${s.name} - ${score}% - ${result}`)); renderAll(); }
function whatsappStudent(phone,name,msg){ window.open("https://wa.me/254"+phone.replace(/^0/,"").replace(/\s/g,"")+"?text="+encodeURIComponent(msg),"_blank"); }
function generateReport(){ let month=document.getElementById("reportMonth").value||getCurrentMonth(); let mPayments=payments.filter(p=>p.date && p.date.startsWith(month)); let mExams=exams.filter(e=>e.date && e.date.startsWith(month)); let html=`<div id="dsReportPrint" style="background:#fff;border:1px solid #ddd;padding:18px;border-radius:8px"><div style="text-align:center"><div>🇰🇪 REPUBLIC OF KENYA</div><h2>NPS AJIRA DRIVING SCHOOL</h2><div>${t("Monthly Report - ","Ripoti ya Mwezi - ")}${month}</div><hr></div><p>${t("Students:","Wanafunzi:")} <b>${students.length}</b> • ${t("Passed:","Wamefaulu:")} <b>${students.filter(s=>s.status==="Passed").length}</b><br>${t("Payments This Month:","Malipo Mwezi Huu:")} <b>Ksh ${mPayments.reduce((sum,p)=>sum+p.amount,0).toLocaleString()}</b> • ${t("Balance:","Deni:")} Ksh ${students.reduce((sum,s)=>sum+Math.max(0,s.coursePrice-(s.totalPaid||0)),0).toLocaleString()} • ${t("Quiz Attempts:","Quiz Attempts:")} ${quizHistory.length}</p><h4>${t("STUDENTS","WANAFUNZI")}</h4><table border="1" cellpadding="5" style="width:100%;border-collapse:collapse;font-size:12px"><tr><th>${t("Name","Jina")}</th><th>${t("Course","Kozi")}</th><th>${t("Status","Status")}</th><th>${t("Lessons","Masomo")}</th><th>${t("Paid","Amelipa")}</th><th>${t("Balance","Deni")}</th></tr>${students.map(s=>`<tr><td>${s.name}</td><td>${s.courseTitle}</td><td>${s.status}</td><td>${s.lessonsDone||0}</td><td>Ksh ${(s.totalPaid||0).toLocaleString()}</td><td>Ksh ${Math.max(0,s.coursePrice-(s.totalPaid||0)).toLocaleString()}</td></tr>`).join("")}</table><h4>${t("EXAMS","MITIHANI")}</h4>${mExams.map(e=>`<div>${e.name} - ${e.type} - ${e.score}% - ${e.result}</div>`).join("")||"<p>"+t("None","Hakuna")+"</p>"}<br><br><table style="width:100%"><tr><td>Admin:<br><br>______________<br>${currentUser?currentUser.name:""}</td><td style="text-align:right">OCS / Stamp:<br><br>______________</td></tr></table></div><button class="green" onclick="printReport()">🖨️ ${t("Print / Save as PDF","Print / Save kama PDF")}</button>`; document.getElementById("reportPreview").innerHTML=html; }
function printReport(){ let c=document.getElementById("dsReportPrint")?.innerHTML; if(!c) return alert(t("Generate report first","Tengeneza ripoti kwanza")); let w=window.open("","_blank"); w.document.write(`<html><body>${c}<script>window.onload=()=>window.print()<\/script></body></html>`); w.document.close(); }
function shareReport(){ let month=document.getElementById("reportMonth").value||getCurrentMonth(); let txt=t(`🇰🇪 AJIRA DRIVING SCHOOL REPORT\nMonth: ${month}\nStudents: ${students.length} • Passed: ${students.filter(s=>s.status==="Passed").length}\nTotal Payments: Ksh ${payments.reduce((sum,p)=>sum+p.amount,0).toLocaleString()}`,`🇰🇪 RIPOTI YA AJIRA DRIVING SCHOOL\nMwezi: ${month}\nWanafunzi: ${students.length} • Wamefaulu: ${students.filter(s=>s.status==="Passed").length}\nMalipo Yote: Ksh ${payments.reduce((sum,p)=>sum+p.amount,0).toLocaleString()}`); window.open("https://wa.me/?text="+encodeURIComponent(txt),"_blank"); }
function renderAll(){
  applyLang();
  let alertHtml=""; let myStu=!isAdmin?students.filter(s=>s.phone===currentUser?.phone):[]; if(!isAdmin && myStu.length>0){ let passed=myStu.filter(s=>s.status==="Passed"); if(passed.length) alertHtml+=`<div class="alert-green">🎉 ${t("CONGRATULATIONS! You passed: ","HONGERA! Umepita: ")}${passed.map(s=>s.courseTitle).join(", ")} - ${t("Get your Certificate + ID!","Pata Cheti + ID yako!")}</div>`; let bal=myStu.reduce((sum,s)=>sum+Math.max(0,s.coursePrice-(s.totalPaid||0)),0); if(bal>0) alertHtml+=`<div class="alert-orange">💰 ${t("Your Balance:","Deni Lako:")} Ksh ${bal.toLocaleString()}</div>`; } if(isAdmin){ let unpaid=students.filter(s=>(s.coursePrice-(s.totalPaid||0))>0); if(unpaid.length) alertHtml+=`<div class="alert-orange">💰 ${unpaid.length} ${t("students have balance -","wanafunzi wana deni -")} Ksh ${unpaid.reduce((sum,s)=>sum+(s.coursePrice-(s.totalPaid||0)),0).toLocaleString()}</div>`; } if(!alertHtml) alertHtml=`<div class="alert-green">✅ ${t("Welcome to Ajira Driving School - Choose course, enroll, learn, pass, get a job!","Karibu Ajira Driving School - Chagua kozi, jiandikishe, jifunze, faulu, pata kazi!")}</div>`; document.getElementById("alertBox").innerHTML=alertHtml;
  let myQuiz=quizHistory.filter(q=>q.phone===currentUser?.phone); if(document.getElementById("quizBest")){ document.getElementById("quizBest").innerText=(myQuiz.length?Math.max(...myQuiz.map(q=>q.score)):0)+"%"; document.getElementById("quizAttempts").innerText=myQuiz.length; }
  document.getElementById("eCourse").innerHTML=courses.length?courses.map(c=>`<option value="${c.id}">${c.title} - Ksh ${c.price.toLocaleString()}</option>`).join(""):`<option value="">${t("No Course","Hakuna Kozi")}</option>`;
  document.getElementById("lStudent").innerHTML=students.length?students.map(s=>`<option value="${s.id}">${s.name} - ${s.courseTitle}</option>`).join(""):`<option value="">${t("None","Hakuna")}</option>`;
  document.getElementById("pStudent").innerHTML=students.length?students.map(s=>`<option value="${s.id}">${s.name} - ${t("Balance","Deni")} Ksh ${Math.max(0,s.coursePrice-(s.totalPaid||0)).toLocaleString()}</option>`).join(""):`<option value="">${t("None","Hakuna")}</option>`;
  document.getElementById("xStudent").innerHTML=students.length?students.map(s=>`<option value="${s.id}">${s.name} - ${s.courseTitle}</option>`).join(""):`<option value="">${t("None","Hakuna")}</option>`;
  updateEnrollInfo();
  let cSearch=document.getElementById("courseSearch")?.value.toLowerCase()||""; let fCourses=courses.filter(c=>(c.title+" "+c.cls).toLowerCase().includes(cSearch));
  document.getElementById("courseList").innerHTML=fCourses.length?fCourses.map(c=>{ let count=students.filter(s=>s.courseId===c.id).length; return `<div class="card" style="border-left:5px solid #1a7a3a"><div class="top"><b>🚗 ${c.title}</b><span class="badge">Ksh ${c.price.toLocaleString()}</span></div><span class="small">${t("Duration:","Muda:")} ${c.duration} • ${t("Instructor:","Mwalimu:")} ${c.instructor}<br>${t("Vehicle:","Gari:")} ${c.vehicle}<br>${t("Students:","Wanafunzi:")} ${count}<br>${c.desc}</span><br><button class="green" onclick="quickEnroll(${c.id})">📝 ${t("Enroll -","Jiandikishe -")} Ksh ${c.price.toLocaleString()}</button></div>`}).join(""):`<p class='small'>${t("No courses.","Hakuna kozi.")}</p>`;
  let stuF=document.getElementById("stuFilter")?.value||"all"; let stuS=document.getElementById("stuSearch")?.value.toLowerCase()||""; let fStudents=students.filter(s=>{ if(!isAdmin && s.phone!==currentUser?.phone) return false; if(stuF!=="all" && s.status!==stuF) return false; return (s.name+" "+s.phone+" "+s.courseTitle).toLowerCase().includes(stuS); });
  document.getElementById("studentList").innerHTML=fStudents.length?fStudents.map(s=>{ let bal=Math.max(0,s.coursePrice-(s.totalPaid||0)); let pct=s.coursePrice?Math.round((s.totalPaid||0)/s.coursePrice*100):0; let color=s.status==="Passed"?"#1a7a3a":s.status==="Failed"?"#b71c1c":s.status==="Ready for Test"?"#ef6c00":"#0b2c4a"; let initials=s.name.split(" ").map(w=>w[0]).join("").slice(0,2).toUpperCase(); return `<div class="card" style="border-left:5px solid ${color}"><div style="display:flex;gap:10px"><div class="avatar">${initials}</div><div style="flex:1"><div class="top"><b>🧑‍🎓 ${s.name}</b><span class="badge" style="background:${color};color:#fff">${s.status}</span></div><span class="small">${t("Phone:","Simu:")} ${s.phone} • ID: ${s.idNo} • ${s.county}<br>${t("Course:","Kozi:")} <b>${s.courseTitle}</b><br>${t("Schedule:","Ratiba:")} ${s.schedule} • ${t("Lessons:","Masomo:")} ${s.lessonsDone||0}</span></div></div><div style="margin-top:8px"><div class="top"><span class="small">${t("Paid:","Amelipa:")} Ksh ${(s.totalPaid||0).toLocaleString()} / Ksh ${s.coursePrice.toLocaleString()} (${pct}%)</span><span class="small">${t("Balance:","Deni:")} Ksh ${bal.toLocaleString()}</span></div><div class="bar"><div class="fill" style="width:${pct}%;background:${bal===0?"#1a7a3a":"#ef6c00"}"></div></div></div>${s.status==="Passed"?`<button class="green" onclick="showCertificate(${s.id})">🏆 ${t("View / Print Certificate","Ona / Print Cheti")}</button>`:""}${isAdmin?`<div style="display:flex;gap:6px"><button class="secondary" style="flex:1" onclick="addLessonDone(${s.id})">${t("+ 1 Lesson","+ Somo 1")}</button><button class="secondary" style="flex:1" onclick="changeStudentStatus(${s.id},'Ready for Test')">${t("Ready for Test","Tayari kwa Mtihani")}</button><button class="secondary" style="flex:1" onclick="whatsappStudent('${s.phone}','${s.name}','Hello ${s.name}, your lesson tomorrow is ${s.schedule}.')">💬 WhatsApp</button></div><select onchange="changeStudentStatus(${s.id},this.value)"><option ${s.status==='Enrolled'?'selected':''}>Enrolled</option><option ${s.status==='In Training'?'selected':''}>In Training</option><option ${s.status==='Ready for Test'?'selected':''}>Ready for Test</option><option ${s.status==='Passed'?'selected':''}>Passed</option><option ${s.status==='Failed'?'selected':''}>Failed</option><option ${s.status==='Dropped'?'selected':''}>Dropped</option></select>`:""}</div>`}).join(""):`<p class='small'>${t("No students.","Hakuna wanafunzi.")}</p>`;
  let fLessons=!isAdmin?lessons.filter(l=>l.phone===currentUser?.phone):lessons; document.getElementById("lessonList").innerHTML=fLessons.length?fLessons.map(l=>`<div class="card"><div class="top"><b>${l.name} - ${l.type}</b><span class="badge">${l.status}</span></div><span class="small">${l.date} ${l.time} • ${t("Vehicle:","Gari:")} ${l.vehicle} • ${t("Instructor:","Mwalimu:")} ${l.instructor}<br>${t("Location:","Mahali:")} ${l.location}</span>${l.status==="Scheduled"&&isAdmin?`<button class="green" onclick="completeLesson(${l.id})">✅ ${t("Lesson Completed","Somo Limekamilika")}</button>`:""}</div>`).join(""):`<p class='small'>${t("No lessons.","Hakuna masomo.")}</p>`;
  let fPays=!isAdmin?payments.filter(p=>p.name===currentUser?.name):payments; document.getElementById("paymentList").innerHTML=fPays.length?fPays.map(p=>`<div class="card"><div class="top"><b>${p.name} - Ksh ${p.amount.toLocaleString()}</b><span class="badge">${p.method}</span></div><span class="small">${t("Code:","Code:")} ${p.code} • ${p.date}</span></div>`).join(""):`<p class='small'>${t("No payments.","Hakuna malipo.")}</p>`;
  let fExams=!isAdmin?exams.filter(e=>e.name===currentUser?.name):exams; document.getElementById("examList").innerHTML=fExams.length?fExams.map(e=>`<div class="card"><div class="top"><b>${e.name} - ${e.type}</b><b style="color:${e.result.includes("Passed")||e.result.includes("Amefaulu")?"#1a7a3a":"#b71c1c"}">${e.score}% - ${e.result}</b></div><span class="small">${e.date} • ${e.notes||"-"}</span></div>`).join(""):`<p class='small'>${t("No results.","Hakuna matokeo.")}</p>`;
  let passedStudents=students.filter(s=>s.status==="Passed"); document.getElementById("jobList").innerHTML=`<div class="card"><h3 style="margin:0">💼 ${t("Jobs for Passed Students","Ajira kwa Waliopita")}</h3><p class="small">${passedStudents.length} ${t("students passed.","wanafunzi wamefaulu.")}</p></div>`+[{title:t("Driver - NPS MT - Eldoret","Dereva - NPS MT - Eldoret"),salary:"Ksh 35,000 - 50,000",req:t("Class B+C + Licence","Class B+C + Leseni")},{title:t("Driver - Private Company - Kitale","Dereva - Kampuni Binafsi - Kitale"),salary:"Ksh 30,000 - 40,000",req:t("Class B + Licence","Class B + Leseni")},{title:t("Lorry Driver - Transport Company","Dereva wa Lori - Kampuni ya Usafiri"),salary:"Ksh 40,000 - 60,000",req:t("Class C + Licence","Class C + Leseni")},{title:t("Bus Driver - PSV Sacco","Dereva wa Basi - PSV Sacco"),salary:"Ksh 35,000 - 55,000",req:t("Class D + PSV","Class D + PSV")},{title:t("Rider - Delivery - Eldoret","Rider - Delivery - Eldoret"),salary:"Ksh 25,000 - 35,000",req:t("Class A + Licence","Class A + Leseni")}].map(j=>`<div class="card"><div class="top"><b>${j.title}</b><span class="badge">${j.salary}</span></div><span class="small">${t("Requirements:","Mahitaji:")} ${j.req}<br>${t("Passed:","Waliopita:")} ${passedStudents.map(s=>s.name).join(", ")||t("None yet","Hakuna bado")}</span><br><button class="green" onclick="alert('${t("Apply for Job: ","Omba Ajira: ")}${j.title}')">${t("Apply for This Job","Omba Ajira Hii")}</button></div>`).join("");
  document.getElementById("totalCourses").innerText=courses.length; document.getElementById("totalStudents").innerText=students.length; document.getElementById("totalPassed").innerText=students.filter(s=>s.status==="Passed").length; document.getElementById("totalPaid").innerText="Ksh "+payments.reduce((sum,p)=>sum+p.amount,0).toLocaleString(); document.getElementById("totalBalance").innerText="Ksh "+students.reduce((sum,s)=>sum+Math.max(0,s.coursePrice-(s.totalPaid||0)),0).toLocaleString();
  let pInfo=document.getElementById("pStudentInfo"); if(pInfo && document.getElementById("pStudent").value){ let s=students.find(x=>x.id==document.getElementById("pStudent").value); if(s) pInfo.innerHTML=`<b>${s.name} - ${s.courseTitle}</b><br>${t("Paid:","Amelipa:")} Ksh ${(s.totalPaid||0).toLocaleString()} • ${t("Balance:","Deni:")} Ksh ${Math.max(0,s.coursePrice-(s.totalPaid||0)).toLocaleString()}`; }
}
// Init language on load
document.addEventListener("DOMContentLoaded",()=>{ document.getElementById("btnEN").classList.toggle("active",LANG==="en"); document.getElementById("btnSW").classList.toggle("active",LANG==="sw"); applyLang(); });
</script>
</body>
</html>

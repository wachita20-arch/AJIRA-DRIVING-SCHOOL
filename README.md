<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no, viewport-fit=cover">
<meta name="theme-color" content="#0b2c4a">
<title>AJIRA Driving School - ADMISSION • MEDICAL • LESSONS • PAYMENTS • CERTIFICATE</title>
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
.receipt{background:#fff;border:2px dashed #0b2c4a;border-radius:10px;padding:14px;text-align:center}
.kpi{display:grid;grid-template-columns:1fr 1fr;gap:8px}
.kpi div{background:#fff;border-radius:10px;padding:10px;text-align:center}
.cred-box{background:#e3f2fd;border:2px solid #0b2c4a;border-radius:10px;padding:10px;margin-top:10px;font-size:12px}
.med-box{background:#e8f5e9;border:2px solid #1a7a3a;border-radius:10px;padding:10px}
.med-box.red{background:#ffebee;border-color:#b71c1c}
.cert-box{border:4px double #0b2c4a;padding:18px;text-align:center;background:#fffef5}
</style>
</head>
<body>
<div class="phone">
<header><div>AJIRA DRIVING SCHOOL</div><h1>ADMISSION • MEDICAL • LESSONS • FEES • CERTIFICATE</h1><p>One App - Everything</p><span class="badge">NTSA APPROVED • EN / SW • v6 - MEDICAL + NTSA CERTIFICATE</span>
<div class="lang"><button id="btnEN" class="active" onclick="setLang('en')">ENGLISH</button><button id="btnSW" onclick="setLang('sw')">KISWAHILI</button></div>
<a href="https://wa.me/c/254777725770" target="_blank" style="text-decoration:none"><button style="background:#25D366">JOIN WHATSAPP CHANNEL - 0777 725 770</button></a>
</header>
<main>
<div id="loginView">
  <h2>Welcome - Ajira Driving School</h2>
  <p class="small">Secure Login - Username + Password</p>
  <label class="small">Login As *</label>
  <select id="userType" onchange="toggleLogin()"><option value="student">Student</option><option value="instructor">Instructor</option><option value="admin">Admin</option></select>
  <div id="studentLogin"><label class="small">Student Username / Phone *</label><input id="stuUser" placeholder="e.g. john.kiprop OR 0711111111"><label class="small">Password *</label><input id="stuPass" type="password" placeholder="Password *"><p class="small">No account? <a href="#" onclick="document.getElementById('registerLoginBox').classList.remove('hidden');return false">Create Student Account</a></p></div>
  <div id="instructorLogin" class="hidden"><label class="small">Instructor Username *</label><input id="instUser" placeholder="e.g. david.otieno"><label class="small">Password *</label><input id="instPass" type="password" placeholder="Password *"><label class="small">Staff No.</label><input id="instStaff" placeholder="STF001"></div>
  <div id="adminLogin" class="hidden"><label class="small">Admin Username *</label><input id="admUser" placeholder="e.g. admin"><label class="small">Admin Password *</label><input id="admPass" type="password" placeholder="Admin Password *"><label class="small">Admin Code *</label><input id="admCode" placeholder="1234" inputmode="numeric"></div>
  <button onclick="login()">Login Securely</button>
  <button class="secondary" onclick="fillDemo('student')">Fill Demo Student</button>
  <button class="secondary" onclick="fillDemo('instructor')">Fill Demo Instructor</button>
  <button class="secondary" onclick="fillDemo('admin')">Fill Demo Admin</button>
  <div class="cred-box"><b>DEMO CREDENTIALS:</b><br><b>Student:</b> john.kiprop / Ajira123<br><b>Instructor:</b> david.otieno / Instr123 / STF001<br><b>Admin:</b> admin / Admin123 / Code 1234</div>
  <div id="registerLoginBox" class="card hidden" style="margin-top:12px"><h3>Create Student Account</h3><input id="regName" placeholder="Full Name *"><input id="regUser" placeholder="Choose Username e.g. john.kiprop *"><input id="regPhone" placeholder="Phone *"><input id="regId" placeholder="ID No. *"><input id="regPass" type="password" placeholder="Choose Password (min 6) *"><input id="regPass2" type="password" placeholder="Confirm Password *"><button class="green" onclick="registerStudentAccount()">Create Account → Login</button></div>
  <button class="secondary" onclick="resetDemo()">Reset Demo Data</button>
</div>

<div id="appView" class="hidden">
  <div class="top"><b>Hello, <span id="userName"></span></b><button class="secondary" style="width:auto" onclick="logout()">Logout</button></div>
  <p class="small"><span id="stationLabel"></span> • <span id="dateLabel"></span> • <span id="roleLabel"></span></p>
  <div id="alertBox"></div>
  <div class="kpi">
    <div><b id="kStudents" style="font-size:22px;color:#0b2c4a">0</b><br><span class="small">Students</span></div>
    <div><b id="kClasses" style="font-size:22px;color:#0b2c4a">0</b><br><span class="small">Classes Booked</span></div>
    <div><b id="kPaid" style="font-size:18px;color:#1a7a3a">Ksh 0</b><br><span class="small">Collected</span></div>
    <div><b id="kOwing" style="font-size:18px;color:#b71c1c">Ksh 0</b><br><span class="small">Still Owing</span></div>
    <div><b id="kLessonsDone" style="font-size:22px">0</b><br><span class="small">Lessons Completed</span></div>
    <div><b id="kPassed" style="font-size:22px;color:#1a7a3a">0</b><br><span class="small">Passed</span></div>
    <div><b id="kMedFit" style="font-size:22px;color:#1a7a3a">0</b><br><span class="small">Medical FIT</span></div>
    <div><b id="kMedUnfit" style="font-size:22px;color:#b71c1c">0</b><br><span class="small">Medical UNFIT / Pending</span></div>
  </div>
  <div class="card" id="myCard" style="margin-top:10px">
    <div class="top"><b>My Admission + Medical</b><span class="badge" id="myStatusBadge">-</span></div>
    <div id="myAdmissionInfo" class="small"></div>
    <div id="myMedicalInfo" class="small" style="margin-top:8px"></div>
    <div style="margin-top:8px"><div class="top"><span class="small">Paid <b id="myPaid2">Ksh 0</b> / <b id="myFee2">Ksh 0</b> (<b id="myPct">0%</b>)</span><span class="small">Balance: <b id="myBal2" style="color:#b71c1c">Ksh 0</b></span></div><div class="bar"><div class="fill" id="myPayBar" style="width:0%"></div></div></div>
    <div style="margin-top:8px"><div class="top"><span class="small">Lessons <b id="myLessonCount">0/20</b></span><span class="small">Next Class: <b id="myNextClass">-</b></span></div></div>
    <div id="myCardActions"></div><div id="myDeregBox"></div><div id="myCertBox"></div>
  </div>
  <div class="tabs">
    <button id="tabAdmission" class="active" onclick="showTab('admission')">Admission</button>
    <button id="tabStudents" onclick="showTab('students')">Students</button>
    <button id="tabMedical" onclick="showTab('medical')">Medical</button>
    <button id="tabClasses" onclick="showTab('classes')">Classes</button>
    <button id="tabLessons" onclick="showTab('lessons')">Lessons</button>
    <button id="tabPayments" onclick="showTab('payments')">Payments</button>
    <button id="tabBalances" onclick="showTab('balances')">Balances</button>
    <button id="tabDereg" onclick="showTab('dereg')">Dereg</button>
    <button id="tabCertificate" onclick="showTab('certificate')">Certificate</button>
    <button id="tabReport" onclick="showTab('report')">Report</button>
  </div>

  <!-- ADMISSION + PARTICULARS + MEDICAL -->
  <div id="admissionTab">
    <div class="card"><h3 style="margin:0">Admission Form - Student Particulars</h3><p class="small">Fill once. Student gets Admission No + Username + Password + Medical Record.</p>
      <label class="small">Select Course *</label><select id="aCourse" onchange="updateAdmissionInfo()"></select><div id="aCourseInfo" class="small"></div>
      <h4 style="margin:10px 0 0">A. STUDENT PARTICULARS</h4>
      <input id="aName" placeholder="Full Name *"><input id="aPhone" placeholder="Phone *" inputmode="tel"><input id="aId" placeholder="ID Card Number * (For Certificate)" inputmode="numeric">
      <input id="aAge" placeholder="Age" type="number"><select id="aGender"><option>Male</option><option>Female</option></select>
      <input id="aDOB" type="date"><span class="small">Date of Birth</span>
      <input id="aCounty" placeholder="County e.g. Trans Nzoia"><input id="aEducation" placeholder="Education e.g. KCSE C-">
      <input id="aNextKin" placeholder="Next of Kin Name + Phone"><input id="aAddress" placeholder="Home / Estate e.g. Eldoret - Kapsoya">
      <select id="aHasLicence"><option>No Licence - Beginner</option><option>Have Licence - Add Class</option><option>Licence Expired - Refresher</option></select>
      <input id="aLicenceNo" placeholder="Licence No. (If any)">
      <h4>B. LOGIN CREDENTIALS</h4><div style="background:#e3f2fd;border:2px solid #0b2c4a;border-radius:10px;padding:10px"><input id="aUsername" placeholder="Username e.g. john.kiprop"><input id="aPassword" placeholder="Password" value="Ajira123"><div class="small" id="aCredPreview"></div></div>
      <h4>C. MEDICAL REPORT - STUDENT (Required Before Practical)</h4><div class="med-box">
        <label class="small">Blood Group *</label><select id="aBlood"><option>Select Blood Group</option><option>O+</option><option>O-</option><option>A+</option><option>A-</option><option>B+</option><option>B-</option><option>AB+</option><option>AB-</option><option>Not Known</option></select>
        <label class="small">Medical Exam Date *</label><input id="aMedDate" type="date">
        <label class="small">Examined By - Doctor / Clinical Officer *</label><input id="aMedDoctor" placeholder="e.g. Dr. Otieno - Eldoret Hospital">
        <label class="small">Medical Centre / Hospital *</label><input id="aMedCentre" placeholder="e.g. Eldoret Hospital - Medical Dept">
        <label class="small">Vision / Eyesight *</label><select id="aMedVision"><option>Normal - 6/6 - No Glasses</option><option>Normal With Glasses</option><option>Poor Vision - Needs Glasses</option><option>Colour Blind</option></select>
        <label class="small">Hearing *</label><select id="aMedHearing"><option>Normal Hearing</option><option>Partial Hearing Loss</option><option>Hearing Aid Used</option></select>
        <label class="small">Blood Pressure</label><input id="aMedBP" placeholder="e.g. 120/80">
        <label class="small">Height (cm) / Weight (kg)</label><input id="aMedHW" placeholder="e.g. 175cm / 70kg">
        <label class="small">Any Chronic Illness / Disability?</label><select id="aMedChronic"><option>None - Healthy</option><option>Epilepsy</option><option>Diabetes</option><option>Heart Condition</option><option>Asthma</option><option>Physical Disability</option><option>Other - See Notes</option></select>
        <textarea id="aMedNotes" rows="2" placeholder="Medical Notes: Allergies, medication, operations..."></textarea>
        <label class="small">Doctor's Fitness Decision *</label><select id="aMedFitness"><option>FIT TO DRIVE - No Restrictions</option><option>FIT WITH GLASSES - Must Wear Glasses While Driving</option><option>FIT WITH CONDITIONS - See Notes</option><option>UNFIT - Cannot Drive - Needs Treatment</option><option>PENDING - Needs Further Tests</option></select>
        <label class="small">Medical Report No. / Ref</label><input id="aMedRef" placeholder="e.g. MED-2026-001">
      </div>
      <h4>D. NTSA / TEST DETAILS (Fill at Test Time - Can Edit Later)</h4>
      <input id="aPDL" placeholder="PDL Number e.g. PDL-2026-12345 (Provisional Driving Licence)">
      <input id="aTestForm" placeholder="Test Form Number e.g. TF-2026-7890">
      <input id="aNTSACert" placeholder="NTSA Certification Number e.g. NTSA-CERT-2026-001 (Fill after Passing)">
      <select id="aSchedule"><option>Morning - 8am - 11am</option><option>Midday - 11am - 2pm</option><option>Afternoon - 2pm - 5pm</option><option>Weekend Only - Sat / Sun</option></select>
      <label class="small">Payment Plan *</label><select id="aPlan" onchange="updateAdmissionInfo()"><option value="full">Pay in Full</option><option value="2">2 Installments</option><option value="3">3 Installments</option><option value="4">4 Installments</option></select><div id="aPlanInfo" class="small"></div>
      <div style="background:#e8f5e9;border:2px solid #1a7a3a;border-radius:10px;padding:10px"><b>Pay Deposit - M-Pesa STK</b><input id="aMpesaPhone" placeholder="M-Pesa Phone"><input id="aDeposit" placeholder="Deposit Ksh" type="number"><button class="green" onclick="stkAdmission()">Send STK Push</button><input id="aMpesaCode" placeholder="M-Pesa Code"></div>
      <button class="green" onclick="admitStudent()">Admit Student → Create Admission + Medical + Login</button>
    </div><div id="admissionSuccess"></div>
  </div>

  <!-- STUDENTS -->
  <div id="studentsTab" class="hidden">
    <select id="stuFilter" onchange="renderAll()"><option value="all">All</option><option value="Enrolled">Enrolled</option><option value="In Training">In Training</option><option value="Ready for Test">Ready for Test</option><option value="Passed">Passed</option><option value="Failed">Failed</option><option value="Dropped">Dropped</option><option value="Deregistered">Deregistered</option></select>
    <input id="stuSearch" placeholder="Search name, phone, admission, username, ID, PDL..." oninput="renderAll()">
    <div id="studentList"></div>
  </div>

  <!-- MEDICAL -->
  <div id="medicalTab" class="hidden">
    <div class="card"><h3 style="margin:0">Medical Report - Students + Instructors</h3><p class="small">Every student MUST be FIT before Practical. Every instructor MUST have valid medical (renew yearly). UNFIT = Cannot Drive / Cannot Teach.</p>
      <div style="display:flex;gap:6px"><button class="green" style="flex:1" onclick="showMedForm('student')">+ Student Medical</button><button class="secondary" style="flex:1" onclick="showMedForm('instructor')">+ Instructor Medical</button></div>
      <div id="medFormBox" class="hidden" style="margin-top:10px">
        <label class="small">Person Type</label><select id="medType" onchange="updateMedPersonList()"><option value="student">Student</option><option value="instructor">Instructor</option></select>
        <label class="small">Select Person *</label><select id="medPerson"></select><div id="medPersonInfo" class="small"></div>
        <label class="small">Blood Group</label><select id="medBlood"><option>O+</option><option>O-</option><option>A+</option><option>A-</option><option>B+</option><option>B-</option><option>AB+</option><option>AB-</option><option>Not Known</option></select>
        <input id="medDate" type="date"><span class="small">Medical Exam Date</span>
        <input id="medDoctor" placeholder="Doctor / Clinical Officer">
        <input id="medCentre" placeholder="Hospital / Centre">
        <select id="medVision"><option>Normal - 6/6 - No Glasses</option><option>Normal With Glasses</option><option>Poor Vision - Needs Glasses</option><option>Colour Blind</option></select>
        <select id="medHearing"><option>Normal Hearing</option><option>Partial Hearing Loss</option><option>Hearing Aid Used</option></select>
        <input id="medBP" placeholder="Blood Pressure e.g. 120/80"><input id="medHW" placeholder="Height / Weight">
        <select id="medChronic"><option>None - Healthy</option><option>Epilepsy</option><option>Diabetes</option><option>Heart Condition</option><option>Asthma</option><option>Physical Disability</option><option>Other</option></select>
        <textarea id="medNotes" rows="2" placeholder="Medical Notes..."></textarea>
        <select id="medFitness"><option>FIT TO DRIVE - No Restrictions</option><option>FIT WITH GLASSES - Must Wear Glasses While Driving</option><option>FIT WITH CONDITIONS - See Notes</option><option>UNFIT - Cannot Drive - Needs Treatment</option><option>PENDING - Needs Further Tests</option></select>
        <input id="medRef" placeholder="Medical Report No. e.g. MED-2026-001">
        <button class="green" onclick="saveMedical()">Save Medical Report</button>
      </div>
    </div>
    <select id="medFilter" onchange="renderAll()"><option value="all">All Medical Reports</option><option value="FIT">FIT Only</option><option value="UNFIT">UNFIT Only</option><option value="PENDING">PENDING Only</option><option value="student">Students Only</option><option value="instructor">Instructors Only</option></select>
    <div id="medicalList"></div>
    <div class="card"><h3>Instructor Particulars + Medical</h3><div id="instructorList"></div></div>
  </div>

  <!-- CLASSES -->
  <div id="classesTab" class="hidden">
    <div class="card"><h3 style="margin:0">Book a Class</h3><label class="small">Student</label><select id="cStudent" onchange="updateClassPayInfo()"></select><div id="cStudentInfo" class="small"></div><label class="small">Lesson *</label><select id="cLesson" onchange="updateClassInfo()"></select><div id="cLessonInfo" class="small"></div><input id="cDate" type="date"><input id="cTime" type="time"><select id="cInstructor"><option>Instr. David Otieno - Class B / B+C</option><option>Instr. Peter Kamau - Class C / Defensive</option><option>Instr. Jane Wanjiru - Class D / PSV</option><option>Instr. Mary Achieng - Class A / Motorcycle</option></select><select id="cVehicle"><option>KDJ 123A - Probox (Class B)</option><option>KDJ 456B - Lorry (Class C)</option><option>KDJ 789C - Bus (Class D)</option><option>KMDA 101 - Honda (Class A)</option></select><select id="cLocation"><option>Eldoret - Yard</option><option>Eldoret - Town Driving</option><option>Kitale - Yard</option><option>Kitale - Town</option></select><select id="cSlot"><option>Morning - 8am - 11am</option><option>Midday - 11am - 2pm</option><option>Afternoon - 2pm - 5pm</option><option>Weekend Only - Sat / Sun</option></select><button class="green" onclick="bookClass()">Book Class</button></div>
    <div class="card"><h3 style="margin:0">Classes Today</h3><div id="todayClasses"></div></div>
    <select id="classFilter" onchange="renderAll()"><option value="all">All</option><option value="Scheduled">Scheduled</option><option value="Completed">Completed</option><option value="Absent">Absent</option><option value="Cancelled">Cancelled</option></select><div id="classList"></div>
  </div>
  <div id="lessonsTab" class="hidden"><select id="catFilter" onchange="renderCatalog()"><option value="all">All Lessons</option><option value="Theory">Theory Only</option><option value="Practical">Practical Only</option><option value="Mock">Mock Test Only</option></select><div id="catalogList"></div></div>
  <div id="paymentsTab" class="hidden">
    <div class="card" style="background:#e8f5e9;border:2px solid #1a7a3a"><h3 style="margin:0">Pay Fee - M-Pesa STK</h3><label class="small">Student</label><select id="pStudent" onchange="updatePayFormInfo()"></select><div id="pStudentInfo" class="small"></div><input id="pMpesaPhone" placeholder="M-Pesa Phone"><input id="pAmount" placeholder="Amount Ksh" type="number"><select id="pFor"><option>Deposit / Admission Fee</option><option>Installment - Paying Balance</option><option>Full Payment - Clear Balance</option><option>NTSA Test Fee</option></select><button class="green" onclick="stkPushPayment()">Send STK Push</button><input id="pCode" placeholder="M-Pesa Code"><select id="pMethod"><option>M-Pesa</option><option>Cash</option><option>Bank</option></select><button class="green" onclick="savePayment()">Record Payment</button></div>
    <select id="payFilter" onchange="renderAll()"><option value="all">All Payments</option><option value="M-Pesa">M-Pesa Only</option><option value="Cash">Cash Only</option><option value="Bank">Bank Only</option></select><div id="paymentList"></div><div id="receiptArea"></div>
  </div>
  <div id="balancesTab" class="hidden"><div class="card" style="background:#e3f2fd"><h3 style="margin:0">Balances - Who Owes What?</h3></div><select id="balFilter" onchange="renderAll()"><option value="all">All Students</option><option value="paid">Paid in Full</option><option value="owing">Has Balance</option><option value="big">Big Balance > 10,000</option></select><input id="balSearch" placeholder="Search..." oninput="renderAll()"><div id="balanceList"></div></div>
  <div id="deregTab" class="hidden">
    <div class="card" style="background:#ffebee;border:2px solid #b71c1c"><h3 style="margin:0">Deregistration</h3><p class="small">Deregistration does NOT delete payment / medical history. Student cannot login, cannot book.</p><label class="small">Select Student *</label><select id="deregStudent"></select><div id="deregStudentInfo" class="small"></div><label class="small">Reason *</label><select id="deregReason"><option>Student Request - Voluntary Withdrawal</option><option>Non-Payment - Balance Not Paid</option><option>Discipline - Misconduct</option><option>Transferred to Another School</option><option>Medical Reasons - UNFIT</option><option>Failed Test Multiple Times</option><option>Relocation</option><option>Other</option></select><textarea id="deregNotes" rows="2" placeholder="Details..."></textarea><label class="small">Refund / Settlement</label><select id="deregRefund"><option>No Refund - Fee Non-Refundable</option><option>Partial Refund</option><option>Full Refund</option><option>Balance Waived</option></select><input id="deregRefundAmt" placeholder="Refund Amount Ksh" type="number"><label class="small">Admin Password *</label><input id="deregAdminPass" type="password" placeholder="Admin123"><button class="red" onclick="deregisterStudent()">Deregister Student - Confirm</button></div>
    <div class="card"><h3 style="margin:0">Deregistered List</h3><div id="deregList"></div></div><div id="deregSuccess"></div>
  </div>

  <!-- CERTIFICATE -->
  <div id="certificateTab" class="hidden">
    <div class="card"><h3 style="margin:0">Final Certificate - NTSA Certification</h3><p class="small">Certificate includes: Student Particulars + Medical FIT + ID Card Number + PDL Number + Test Form Number + NTSA Certification Number. Fill NTSA numbers before generating.</p>
      <label class="small">Select Student (Passed / Ready for Test) *</label><select id="certStudent" onchange="updateCertForm()"></select><div id="certStudentInfo" class="small"></div>
      <div style="background:#fff3e0;border:2px solid #ef6c00;border-radius:10px;padding:10px">
        <label class="small">ID Card Number * (From Particulars)</label><input id="certIdNo" placeholder="e.g. 40111111">
        <label class="small">PDL Number * (Provisional Driving Licence)</label><input id="certPDL" placeholder="e.g. PDL-2026-12345">
        <label class="small">Test Form Number *</label><input id="certTestForm" placeholder="e.g. TF-2026-7890">
        <label class="small">NTSA Certification Number *</label><input id="certNTSA" placeholder="e.g. NTSA-CERT-2026-001">
        <label class="small">Test Date</label><input id="certTestDate" type="date">
        <label class="small">Test Centre</label><input id="certTestCentre" placeholder="e.g. Eldoret NTSA Test Centre">
        <label class="small">Test Result</label><select id="certResult"><option>PASS - First Attempt</option><option>PASS - Second Attempt</option><option>PASS - Third Attempt</option></select>
        <label class="small">Instructor Who Trained</label><input id="certInstructor" placeholder="e.g. David Otieno - STF001">
        <label class="small">Medical Fitness at Test Time</label><input id="certMedical" placeholder="e.g. FIT TO DRIVE - No Restrictions" readonly>
      </div>
      <button class="green" onclick="saveCertDetails()">Save NTSA Details to Student</button>
      <button class="green" onclick="generateCertificate()">Generate Final Certificate</button>
    </div>
    <div id="certPreview"></div>
    <div id="certArea"></div>
  </div>

  <div id="reportTab" class="hidden"><div class="card"><h3 style="margin:0">School Report</h3><input type="month" id="reportMonth"><button class="green" onclick="generateReport()">Generate Report PDF</button><button class="secondary" onclick="shareReport()">Share via WhatsApp</button></div><div id="reportPreview"></div></div>
  <div id="certTab" class="hidden"><div id="certArea2"></div></div>
</div>
</main>
<footer>AJIRA DRIVING SCHOOL • NTSA Approved<br>Learn • Pass • Get Job • <a href="https://wa.me/c/254777725770" target="_blank">WhatsApp Channel</a></footer>
</div>
<div class="bottom-nav" id="bottomNav" style="display:none">
  <button onclick="showTab('admission')" id="navAdmission"><span>📝</span>Admission</button>
  <button onclick="showTab('students')" id="navStudents"><span>🧑‍🎓</span>Students</button>
  <button onclick="showTab('medical')" id="navMedical"><span>🩺</span>Medical</button>
  <button onclick="showTab('classes')" id="navClasses"><span>📅</span>Classes</button>
  <button onclick="showTab('payments')" id="navPayments"><span>💰</span>Payments</button>
  <button onclick="showTab('certificate')" id="navCertificate"><span>🏆</span>Cert</button>
  <button onclick="showTab('report')" id="navReport"><span>📄</span>Report</button>
</div>
<script>
let LANG = localStorage.getItem("ajira_lang") || "en";
function setLang(l){ LANG=l; localStorage.setItem("ajira_lang",l); document.getElementById("btnEN").classList.toggle("active",l==="en"); document.getElementById("btnSW").classList.toggle("active",l==="sw"); }
function t(en,sw){ return LANG==="sw"?sw:en; }
let users = JSON.parse(localStorage.getItem("ajira_users")||"[]");
let courses = JSON.parse(localStorage.getItem("ajira_ds_courses")||"[]");
let students = JSON.parse(localStorage.getItem("ajira_ds_students")||"[]");
let classes = JSON.parse(localStorage.getItem("ajira_ds_classes")||"[]");
let payments = JSON.parse(localStorage.getItem("ajira_ds_payments")||"[]");
let deregistered = JSON.parse(localStorage.getItem("ajira_deregistered")||"[]");
let medicals = JSON.parse(localStorage.getItem("ajira_medicals")||"[]");
let instructors = JSON.parse(localStorage.getItem("ajira_instructors")||"[]");
let currentUser=null, currentRole="", isAdmin=false, isInstructor=false;
function getToday(){ return new Date().toISOString().slice(0,10); }
function getCurrentMonth(){ return new Date().toISOString().slice(0,7); }
function getBal(s){ return Math.max(0, s.coursePrice - (s.totalPaid||0)); }
function getPct(s){ return s.coursePrice?Math.round((s.totalPaid||0)/s.coursePrice*100):0; }
function genAdmissionNo(){ let max=0; [...students,...deregistered].forEach(s=>{ let m=(s.admissionNo||"").match(/ADS-(\d+)/); if(m) max=Math.max(max,parseInt(m[1])); }); return "ADS-"+String(max+1).padStart(4,"0")+"-"+new Date().getFullYear(); }
function makeUsername(name){ return name.trim().toLowerCase().replace(/[^a-z ]/g,"").replace(/\s+/g,".").replace(/\.+/g,"."); }
function resetDemo(){ if(!confirm("Reset all data?")) return; ["ajira_users","ajira_ds_courses","ajira_ds_students","ajira_ds_classes","ajira_ds_payments","ajira_deregistered","ajira_medicals","ajira_instructors"].forEach(k=>localStorage.removeItem(k)); location.reload(); }
function toggleLogin(){ let tt=document.getElementById("userType").value; document.getElementById("studentLogin").classList.toggle("hidden",tt!=="student"); document.getElementById("instructorLogin").classList.toggle("hidden",tt!=="instructor"); document.getElementById("adminLogin").classList.toggle("hidden",tt!=="admin"); }
function fillDemo(role){ if(role==="student"){ document.getElementById("userType").value="student"; toggleLogin(); document.getElementById("stuUser").value="john.kiprop"; document.getElementById("stuPass").value="Ajira123"; } if(role==="instructor"){ document.getElementById("userType").value="instructor"; toggleLogin(); document.getElementById("instUser").value="david.otieno"; document.getElementById("instPass").value="Instr123"; document.getElementById("instStaff").value="STF001"; } if(role==="admin"){ document.getElementById("userType").value="admin"; toggleLogin(); document.getElementById("admUser").value="admin"; document.getElementById("admPass").value="Admin123"; document.getElementById("admCode").value="1234"; } }
function seedUsers(){
  if(users.length===0){ users=[{username:"john.kiprop",phone:"0711111111",password:"Ajira123",role:"student",name:"John Kiprop",admissionNo:"ADS-0001-2026"},{username:"grace.wanjiku",phone:"0744444444",password:"Ajira123",role:"student",name:"Grace Wanjiku",admissionNo:"ADS-0004-2026"},{username:"faith.chebet",phone:"0722222222",password:"Ajira123",role:"student",name:"Faith Chebet",admissionNo:"ADS-0002-2026"},{username:"kevin.barasa",phone:"0733333333",password:"Ajira123",role:"student",name:"Kevin Barasa",admissionNo:"ADS-0003-2026"},{username:"david.otieno",phone:"0710000001",password:"Instr123",role:"instructor",name:"David Otieno",staffNo:"STF001"},{username:"peter.kamau",phone:"0710000002",password:"Instr123",role:"instructor",name:"Peter Kamau",staffNo:"STF002"},{username:"jane.wanjiru",phone:"0710000003",password:"Instr123",role:"instructor",name:"Jane Wanjiru",staffNo:"STF003"},{username:"admin",phone:"0777725770",password:"Admin123",role:"admin",name:"Admin - Ajira",code:"1234"},{username:"manager",phone:"0777725771",password:"Admin123",role:"admin",name:"Manager - Ajira",code:"1234"}]; localStorage.setItem("ajira_users",JSON.stringify(users)); }
  if(instructors.length===0){
    instructors=[
      {id:1,username:"david.otieno",name:"David Otieno",staffNo:"STF001",phone:"0710000001",idNo:"30100001",age:38,gender:"Male",county:"Uasin Gishu",address:"Eldoret - Pioneer",licenceNo:"DL-INST-001",licenceClasses:"B,C,D,BCE",licenceExpiry:"2027-05-20",experience:12,qualification:"NTSA Approved Instructor - Class B,C,D",medical:{blood:"O+",date:getToday(),doctor:"Dr. Otieno - Eldoret Hospital",centre:"Eldoret Hospital",vision:"Normal - 6/6 - No Glasses",hearing:"Normal Hearing",bp:"120/80",hw:"175cm / 75kg",chronic:"None - Healthy",notes:"Fit - No restrictions",fitness:"FIT TO DRIVE - No Restrictions",ref:"MED-INST-001"}},
      {id:2,username:"peter.kamau",name:"Peter Kamau",staffNo:"STF002",phone:"0710000002",idNo:"30200002",age:42,gender:"Male",county:"Trans Nzoia",address:"Kitale - Town",licenceNo:"DL-INST-002",licenceClasses:"C,D,BCE",licenceExpiry:"2027-02-15",experience:15,qualification:"NTSA Approved Instructor - Defensive Driving",medical:{blood:"A+",date:getToday(),doctor:"Dr. Wanjiru - Kitale Hospital",centre:"Kitale Hospital",vision:"Normal With Glasses",hearing:"Normal Hearing",bp:"125/85",hw:"170cm / 80kg",chronic:"None - Healthy",notes:"Must wear glasses while teaching",fitness:"FIT WITH GLASSES - Must Wear Glasses While Driving",ref:"MED-INST-002"}},
      {id:3,username:"jane.wanjiru",name:"Jane Wanjiru",staffNo:"STF003",phone:"0710000003",idNo:"30300003",age:35,gender:"Female",county:"Uasin Gishu",address:"Eldoret - Langas",licenceNo:"DL-INST-003",licenceClasses:"B,D",licenceExpiry:"2026-12-30",experience:9,qualification:"NTSA Approved Instructor - PSV / Bus",medical:{blood:"B+",date:getToday(),doctor:"Dr. Kiprop - Eldoret Hospital",centre:"Eldoret Hospital",vision:"Normal - 6/6 - No Glasses",hearing:"Normal Hearing",bp:"118/78",hw:"165cm / 65kg",chronic:"None - Healthy",notes:"Fit",fitness:"FIT TO DRIVE - No Restrictions",ref:"MED-INST-003"}},
    ]; localStorage.setItem("ajira_instructors",JSON.stringify(instructors));
  }
}
function registerStudentAccount(){
  let name=document.getElementById("regName").value.trim(); let user=document.getElementById("regUser").value.trim().toLowerCase(); let phone=document.getElementById("regPhone").value.trim(); let idNo=document.getElementById("regId").value.trim(); let p1=document.getElementById("regPass").value; let p2=document.getElementById("regPass2").value;
  if(!name||!user||!phone||!idNo||!p1) return alert("Fill all fields"); if(p1.length<6) return alert("Password min 6"); if(p1!==p2) return alert("Passwords do not match"); seedUsers(); if(users.find(u=>u.username===user)) return alert("Username taken"); if(users.find(u=>u.phone===phone)) return alert("Phone already registered");
  users.push({username:user,phone,password:p1,role:"student",name,idNo}); localStorage.setItem("ajira_users",JSON.stringify(users)); alert("Account Created! Username: "+user+" Password: "+p1); document.getElementById("userType").value="student"; toggleLogin(); document.getElementById("stuUser").value=user; document.getElementById("stuPass").value=p1;
}
function login(){
  seedUsers(); let type=document.getElementById("userType").value; let found=null;
  if(type==="student"){ let u=document.getElementById("stuUser").value.trim().toLowerCase(); let p=document.getElementById("stuPass").value; if(!u||!p) return alert("Enter Username/Phone and Password"); found=users.find(x=>x.role==="student" && (x.username===u || x.phone===u) && x.password===p); if(!found) return alert("Wrong Student Username/Phone or Password. Demo: john.kiprop / Ajira123"); let isDereg=deregistered.find(d=>d.username===found.username || d.phone===found.phone); if(isDereg) return alert("DEREGISTERED on "+isDereg.deregDate+" - "+isDereg.reason); currentUser={name:found.name,phone:found.phone,username:found.username,role:"Student",admissionNo:found.admissionNo}; currentRole="student"; isAdmin=false; isInstructor=false; }
  else if(type==="instructor"){ let u=document.getElementById("instUser").value.trim().toLowerCase(); let p=document.getElementById("instPass").value; let staff=document.getElementById("instStaff").value.trim(); if(!u||!p) return alert("Enter Instructor Username and Password"); found=users.find(x=>x.role==="instructor" && x.username===u && x.password===p); if(!found) return alert("Wrong Instructor. Demo: david.otieno / Instr123"); if(staff && found.staffNo && staff!==found.staffNo) return alert("Staff No. mismatch"); currentUser={name:found.name,phone:found.phone,username:found.username,role:"Instructor",staffNo:found.staffNo}; currentRole="instructor"; isAdmin=false; isInstructor=true; }
  else { let u=document.getElementById("admUser").value.trim().toLowerCase(); let p=document.getElementById("admPass").value; let code=document.getElementById("admCode").value.trim(); if(!u||!p||!code) return alert("Enter Admin Username, Password and Code"); found=users.find(x=>x.role==="admin" && x.username===u && x.password===p); if(!found) return alert("Wrong Admin. Demo: admin / Admin123 / 1234"); if(found.code && code!==found.code) return alert("Wrong Admin Code"); currentUser={name:found.name,phone:found.phone,username:found.username,role:"Admin"}; currentRole="admin"; isAdmin=true; isInstructor=false; }
  document.getElementById("loginView").classList.add("hidden"); document.getElementById("appView").classList.remove("hidden"); document.getElementById("bottomNav").style.display="flex";
  document.getElementById("userName").innerText=currentUser.name+" ("+currentUser.role+")"; document.getElementById("stationLabel").innerText="Ajira Driving School - Eldoret"; document.getElementById("dateLabel").innerText=new Date().toLocaleDateString(); document.getElementById("roleLabel").innerText="Role: "+currentRole.toUpperCase()+" • User: "+currentUser.username;
  if(courses.length===0){
    courses=[{id:1,title:"Class B - Small Car / Probox",price:18000,duration:"4 Weeks / 20 Lessons",instructor:"David Otieno",vehicle:"KDJ 123A - Probox"},{id:2,title:"Class C - Lorry",price:25000,duration:"5 Weeks / 25 Lessons",instructor:"Peter Kamau",vehicle:"KDJ 456B - Lorry"},{id:3,title:"Class D - Bus / PSV",price:28000,duration:"6 Weeks / 30 Lessons",instructor:"Jane Wanjiru",vehicle:"KDJ 789C - Bus"},{id:4,title:"Class A - Motorcycle",price:12000,duration:"3 Weeks / 15 Lessons",instructor:"Mary Achieng",vehicle:"KMDA 101 - Honda"},{id:5,title:"Class B+C - Car + Lorry",price:35000,duration:"8 Weeks / 40 Lessons",instructor:"David Otieno",vehicle:"KDJ 123A + KDJ 456B"},{id:6,title:"Defensive Driving",price:15000,duration:"2 Weeks / 10 Lessons",instructor:"Peter Kamau",vehicle:"KDJ 123A"}]; localStorage.setItem("ajira_ds_courses",JSON.stringify(courses));
    students=[
      {id:1,admissionNo:"ADS-0001-2026",username:"john.kiprop",password:"Ajira123",name:"John Kiprop",phone:"0711111111",idNo:"40111111",age:24,dob:"2002-05-10",gender:"Male",county:"Trans Nzoia",education:"KCSE C-",nextKin:"Mary Kiprop - 0710000000",address:"Eldoret - Kapsoya",courseId:1,courseTitle:courses[0].title,coursePrice:18000,hasLicence:"No Licence - Beginner",licenceNo:"",schedule:"Morning - 8am - 11am",plan:"3 Installments",status:"In Training",lessonsDone:8,totalPaid:12000,officer:"Admin",pdlNo:"PDL-2026-12345",testFormNo:"TF-2026-7890",ntsaCertNo:"",testDate:"",testCentre:"Eldoret NTSA Test Centre",testResult:"",certInstructor:"David Otieno - STF001",medical:{blood:"O+",date:"2026-11-10",doctor:"Dr. Otieno - Eldoret Hospital",centre:"Eldoret Hospital",vision:"Normal - 6/6 - No Glasses",hearing:"Normal Hearing",bp:"120/80",hw:"175cm / 70kg",chronic:"None - Healthy",notes:"No allergies",fitness:"FIT TO DRIVE - No Restrictions",ref:"MED-2026-001"}},
      {id:2,admissionNo:"ADS-0002-2026",username:"faith.chebet",password:"Ajira123",name:"Faith Chebet",phone:"0722222222",idNo:"40222222",age:22,dob:"2004-03-15",gender:"Female",county:"Uasin Gishu",education:"KCSE C",nextKin:"Peter Chebet - 0720000000",address:"Eldoret - Pioneer",courseId:5,courseTitle:courses[4].title,coursePrice:35000,hasLicence:"No Licence - Beginner",licenceNo:"",schedule:"Midday - 11am - 2pm",plan:"2 Installments",status:"Ready for Test",lessonsDone:18,totalPaid:35000,officer:"Admin",pdlNo:"PDL-2026-12346",testFormNo:"TF-2026-7891",ntsaCertNo:"",testDate:"",testCentre:"Eldoret NTSA Test Centre",testResult:"",certInstructor:"David Otieno - STF001",medical:{blood:"A+",date:"2026-11-12",doctor:"Dr. Wanjiru - Eldoret Hospital",centre:"Eldoret Hospital",vision:"Normal With Glasses",hearing:"Normal Hearing",bp:"118/76",hw:"165cm / 60kg",chronic:"None - Healthy",notes:"Wears glasses",fitness:"FIT WITH GLASSES - Must Wear Glasses While Driving",ref:"MED-2026-002"}},
      {id:3,admissionNo:"ADS-0003-2026",username:"kevin.barasa",password:"Ajira123",name:"Kevin Barasa",phone:"0733333333",idNo:"40333333",age:28,dob:"1998-07-20",gender:"Male",county:"Bungoma",education:"KCSE C-",nextKin:"Jane Barasa - 0730000000",address:"Kitale - Town",courseId:2,courseTitle:courses[1].title,coursePrice:25000,hasLicence:"Have Licence - Add Class",licenceNo:"DL999111",schedule:"Afternoon - 2pm - 5pm",plan:"Pay in Full",status:"Passed",lessonsDone:20,totalPaid:25000,officer:"Admin",pdlNo:"PDL-2026-12347",testFormNo:"TF-2026-7892",ntsaCertNo:"NTSA-CERT-2026-001",testDate:"2026-11-20",testCentre:"Eldoret NTSA Test Centre",testResult:"PASS - First Attempt",certInstructor:"Peter Kamau - STF002",medical:{blood:"B+",date:"2026-11-08",doctor:"Dr. Kiprop - Kitale Hospital",centre:"Kitale Hospital",vision:"Normal - 6/6 - No Glasses",hearing:"Normal Hearing",bp:"122/82",hw:"178cm / 78kg",chronic:"None - Healthy",notes:"Fit",fitness:"FIT TO DRIVE - No Restrictions",ref:"MED-2026-003"}},
      {id:4,admissionNo:"ADS-0004-2026",username:"grace.wanjiku",password:"Ajira123",name:"Grace Wanjiku",phone:"0744444444",idNo:"40444444",age:21,dob:"2005-01-12",gender:"Female",county:"Uasin Gishu",education:"KCSE C+",nextKin:"John Wanjiku - 0740000000",address:"Eldoret - Langas",courseId:1,courseTitle:courses[0].title,coursePrice:18000,hasLicence:"No Licence - Beginner",licenceNo:"",schedule:"Morning - 8am - 11am",plan:"4 Installments",status:"Enrolled",lessonsDone:2,totalPaid:5000,officer:"Admin",pdlNo:"PDL-2026-12348",testFormNo:"TF-2026-7893",ntsaCertNo:"",testDate:"",testCentre:"Eldoret NTSA Test Centre",testResult:"",certInstructor:"David Otieno - STF001",medical:{blood:"O-",date:"2026-11-15",doctor:"Dr. Otieno - Eldoret Hospital",centre:"Eldoret Hospital",vision:"Normal - 6/6 - No Glasses",hearing:"Normal Hearing",bp:"115/75",hw:"160cm / 55kg",chronic:"None - Healthy",notes:"Fit",fitness:"FIT TO DRIVE - No Restrictions",ref:"MED-2026-004"}},
    ]; localStorage.setItem("ajira_ds_students",JSON.stringify(students));
    medicals=[
      {id:1,type:"student",personId:1,name:"John Kiprop",admissionNo:"ADS-0001-2026",blood:"O+",date:"2026-11-10",doctor:"Dr. Otieno - Eldoret Hospital",centre:"Eldoret Hospital",vision:"Normal - 6/6 - No Glasses",hearing:"Normal Hearing",bp:"120/80",hw:"175cm / 70kg",chronic:"None - Healthy",notes:"No allergies",fitness:"FIT TO DRIVE - No Restrictions",ref:"MED-2026-001",by:"Admin"},
      {id:2,type:"student",personId:3,name:"Kevin Barasa",admissionNo:"ADS-0003-2026",blood:"B+",date:"2026-11-08",doctor:"Dr. Kiprop - Kitale Hospital",centre:"Kitale Hospital",vision:"Normal - 6/6 - No Glasses",hearing:"Normal Hearing",bp:"122/82",hw:"178cm / 78kg",chronic:"None - Healthy",notes:"Fit",fitness:"FIT TO DRIVE - No Restrictions",ref:"MED-2026-003",by:"Admin"},
      {id:3,type:"instructor",personId:1,name:"David Otieno",admissionNo:"STF001",blood:"O+",date:getToday(),doctor:"Dr. Otieno - Eldoret Hospital",centre:"Eldoret Hospital",vision:"Normal - 6/6 - No Glasses",hearing:"Normal Hearing",bp:"120/80",hw:"175cm / 75kg",chronic:"None - Healthy",notes:"Fit",fitness:"FIT TO DRIVE - No Restrictions",ref:"MED-INST-001",by:"Admin"},
    ]; localStorage.setItem("ajira_medicals",JSON.stringify(medicals));
    payments=[{id:1,studentId:1,admissionNo:"ADS-0001-2026",name:"John Kiprop",amount:5000,method:"M-Pesa",code:"QK111AAA",for:"Deposit / Admission Fee",date:getToday(),officer:"Admin"},{id:2,studentId:1,admissionNo:"ADS-0001-2026",name:"John Kiprop",amount:7000,method:"M-Pesa",code:"QK222BBB",for:"Installment - Paying Balance",date:getToday(),officer:"Admin"},{id:3,studentId:2,admissionNo:"ADS-0002-2026",name:"Faith Chebet",amount:17500,method:"M-Pesa",code:"QK333CCC",for:"Deposit / Admission Fee",date:getToday(),officer:"Admin"},{id:4,studentId:2,admissionNo:"ADS-0002-2026",name:"Faith Chebet",amount:17500,method:"Cash",code:"REC002",for:"Full Payment - Clear Balance",date:getToday(),officer:"Admin"},{id:5,studentId:3,admissionNo:"ADS-0003-2026",name:"Kevin Barasa",amount:25000,method:"Cash",code:"REC001",for:"Full Payment - Clear Balance",date:getToday(),officer:"Admin"},{id:6,studentId:4,admissionNo:"ADS-0004-2026",name:"Grace Wanjiku",amount:5000,method:"M-Pesa",code:"QK444DDD",for:"Deposit / Admission Fee",date:getToday(),officer:"Admin"}]; localStorage.setItem("ajira_ds_payments",JSON.stringify(payments));
    classes=[{id:101,studentId:1,admissionNo:"ADS-0001-2026",name:"John Kiprop",phone:"0711111111",syllabusId:9,title:"Parking - Bay & Parallel",type:"Practical",date:getToday(),time:"09:00",instructor:"David Otieno",vehicle:"KDJ 123A - Probox",location:"Eldoret - Yard",slot:"Morning",status:"Scheduled",officer:"Admin"},{id:102,studentId:2,admissionNo:"ADS-0002-2026",name:"Faith Chebet",phone:"0722222222",syllabusId:17,title:"Mock Test 1 - Full NTSA Simulation",type:"Mock",date:getToday(),time:"11:30",instructor:"David Otieno",vehicle:"KDJ 123A + KDJ 456B",location:"Eldoret - Town",slot:"Midday",status:"Scheduled",officer:"Admin"},{id:103,studentId:4,admissionNo:"ADS-0004-2026",name:"Grace Wanjiku",phone:"0744444444",syllabusId:5,title:"Car Controls - Start, Stop, Clutch",type:"Practical",date:getToday(),time:"08:00",instructor:"David Otieno",vehicle:"KDJ 123A - Probox",location:"Eldoret - Yard",slot:"Morning",status:"Scheduled",officer:"Admin"}]; localStorage.setItem("ajira_ds_classes",JSON.stringify(classes));
  }
  if(currentRole==="student"){ document.getElementById("aName").value=currentUser.name; document.getElementById("aPhone").value=currentUser.phone; document.getElementById("aMpesaPhone").value=currentUser.phone; }
  if(document.getElementById("reportMonth")) document.getElementById("reportMonth").value=getCurrentMonth();
  renderAll(); renderCatalog();
}
function logout(){ location.reload(); }
function showTab(tt){ ["admission","students","medical","classes","lessons","payments","balances","dereg","certificate","report","cert"].forEach(k=>{let el=document.getElementById(k+"Tab"); if(el) el.classList.toggle("hidden",k!==tt);}); ["Admission","Students","Medical","Classes","Lessons","Payments","Balances","Dereg","Certificate","Report"].forEach(k=>{let el=document.getElementById("tab"+k); if(el) el.classList.toggle("active",k.toLowerCase()===tt);}); ["Admission","Students","Medical","Classes","Payments","Certificate","Report"].forEach(k=>{let el=document.getElementById("nav"+k); if(el) el.classList.toggle("active",k.toLowerCase()===tt);}); renderAll(); window.scrollTo({top:0,behavior:"smooth"}); }
function updateAdmissionInfo(){ let id=document.getElementById("aCourse").value; let c=courses.find(x=>x.id==id); if(!c) return; document.getElementById("aCourseInfo").innerHTML=`<b>${c.title}</b><br>Fee: <b>Ksh ${c.price.toLocaleString()}</b> • ${c.duration}`; let plan=document.getElementById("aPlan").value; let deposit=plan==="full"?c.price:plan==="2"?Math.round(c.price/2):plan==="3"?Math.round(c.price/3):5000; document.getElementById("aPlanInfo").innerHTML=`Plan: ${document.getElementById("aPlan").options[document.getElementById("aPlan").selectedIndex].text}<br>Suggested Deposit: <b>Ksh ${deposit.toLocaleString()}</b> • Admission No: <b>${genAdmissionNo()}</b>`; if(!document.getElementById("aDeposit").value) document.getElementById("aDeposit").value=deposit; let nm=document.getElementById("aName").value.trim(); if(nm && !document.getElementById("aUsername").value) document.getElementById("aUsername").value=makeUsername(nm); document.getElementById("aCredPreview").innerHTML=`Login: Username <b>${document.getElementById("aUsername").value||makeUsername(nm||"student")}</b> / Password <b>${document.getElementById("aPassword").value||"Ajira123"}</b>`; }
function stkAdmission(){ let phone=document.getElementById("aMpesaPhone").value.trim(); let amount=parseInt(document.getElementById("aDeposit").value||0); if(!phone||!amount) return alert("Enter M-Pesa Phone and Deposit"); let btn=event.target; btn.innerText="Sending STK..."; btn.disabled=true; setTimeout(()=>{ btn.innerText="Send STK Push"; btn.disabled=false; let code="QK"+Math.random().toString(36).substring(2,8).toUpperCase(); document.getElementById("aMpesaCode").value=code; alert(`STK SENT!\nPhone: ${phone}\nDeposit: Ksh ${amount.toLocaleString()}\nCode: ${code}`); },1200); }
function admitStudent(){
  if(currentRole==="student") return alert("Students cannot admit others - Admin / Instructor only");
  let courseId=document.getElementById("aCourse").value; let name=document.getElementById("aName").value.trim(); let phone=document.getElementById("aPhone").value.trim(); let idNo=document.getElementById("aId").value.trim(); let username=document.getElementById("aUsername").value.trim().toLowerCase()||makeUsername(name); let password=document.getElementById("aPassword").value||"Ajira123";
  let age=document.getElementById("aAge").value; let gender=document.getElementById("aGender").value; let dob=document.getElementById("aDOB").value; let county=document.getElementById("aCounty").value.trim(); let edu=document.getElementById("aEducation").value.trim(); let nextKin=document.getElementById("aNextKin").value.trim(); let address=document.getElementById("aAddress").value.trim(); let hasLic=document.getElementById("aHasLicence").value; let licNo=document.getElementById("aLicenceNo").value.trim();
  let med={blood:document.getElementById("aBlood").value,date:document.getElementById("aMedDate").value,doctor:document.getElementById("aMedDoctor").value.trim(),centre:document.getElementById("aMedCentre").value.trim(),vision:document.getElementById("aMedVision").value,hearing:document.getElementById("aMedHearing").value,bp:document.getElementById("aMedBP").value.trim(),hw:document.getElementById("aMedHW").value.trim(),chronic:document.getElementById("aMedChronic").value,notes:document.getElementById("aMedNotes").value.trim(),fitness:document.getElementById("aMedFitness").value,ref:document.getElementById("aMedRef").value.trim()||("MED-"+new Date().getFullYear()+"-"+String(students.length+1).padStart(3,"0"))};
  let pdl=document.getElementById("aPDL").value.trim(); let testForm=document.getElementById("aTestForm").value.trim(); let ntsa=document.getElementById("aNTSACert").value.trim();
  let schedule=document.getElementById("aSchedule").value; let plan=document.getElementById("aPlan").options[document.getElementById("aPlan").selectedIndex].text; let deposit=parseInt(document.getElementById("aDeposit").value||0); let mpesa=document.getElementById("aMpesaCode").value.trim();
  if(!courseId||!name||!phone||!idNo) return alert("Enter Course, Name, Phone, ID Card Number");
  if(!med.date || !med.doctor) return alert("Medical Report Required: Enter Medical Date + Doctor");
  if(med.fitness.includes("UNFIT")){ if(!confirm("Medical is UNFIT - Student cannot do Practical until treated. Still admit as PENDING?")) return; }
  seedUsers(); if(users.find(u=>u.username===username)) return alert("Username taken"); if(users.find(u=>u.phone===phone)) return alert("Phone already has account");
  let course=courses.find(x=>x.id==courseId); let admissionNo=genAdmissionNo();
  let stu={id:Date.now(),admissionNo,username,password,name,phone,idNo,age,dob,gender,county,education:edu,nextKin,address,courseId:parseInt(courseId),courseTitle:course.title,coursePrice:course.price,hasLicence:hasLic,licenceNo:licNo,schedule,plan,status:"Enrolled",lessonsDone:0,totalPaid:deposit,officer:currentUser.name,medical:med,pdlNo:pdl,testFormNo:testForm,ntsaCertNo:ntsa,testDate:"",testCentre:"Eldoret NTSA Test Centre",testResult:"",certInstructor:"",createdAt:new Date().toISOString(),day:getToday()};
  students.unshift(stu); localStorage.setItem("ajira_ds_students",JSON.stringify(students));
  medicals.unshift({id:Date.now(),type:"student",personId:stu.id,name,admissionNo,...med,by:currentUser.name}); localStorage.setItem("ajira_medicals",JSON.stringify(medicals));
  users.push({username,phone,password,role:"student",name,admissionNo}); localStorage.setItem("ajira_users",JSON.stringify(users));
  if(deposit>0){ payments.unshift({id:Date.now()+1,studentId:stu.id,admissionNo,name,amount:deposit,method:"M-Pesa",code:mpesa||"DEPOSIT",for:"Deposit / Admission Fee",date:getToday(),officer:currentUser.name}); localStorage.setItem("ajira_ds_payments",JSON.stringify(payments)); }
  let bal=course.price-deposit;
  document.getElementById("admissionSuccess").innerHTML=`<div class="card" style="background:#e8f5e9;border:2px solid #1a7a3a"><h3>ADMITTED + MEDICAL SAVED!</h3><p><b>${name}</b> • ${admissionNo}<br>Course: ${course.title} • Fee: Ksh ${course.price.toLocaleString()} • Paid: Ksh ${deposit.toLocaleString()} • Balance: Ksh ${bal.toLocaleString()}<br>ID Card: ${idNo} • PDL: ${pdl||"-"} • Test Form: ${testForm||"-"}<br>Medical: ${med.fitness} • Blood: ${med.blood} • Doctor: ${med.doctor} • Ref: ${med.ref}</p><div style="background:#fff;border:1px dashed #0b2c4a;padding:10px">LOGIN: Username <b>${username}</b> / Password <b>${password}</b></div><button class="green" onclick="bookClassFor(${stu.id})">Book First Class</button><button class="secondary" onclick="printAdmission('${admissionNo}')">Print Admission + Medical</button></div>`;
  alert(`ADMITTED!\n${name}\nAdmission: ${admissionNo}\nID: ${idNo} • PDL: ${pdl||"-"} • Medical: ${med.fitness}\nLogin: ${username} / ${password}`);
  showTab('students'); renderAll();
}
function printAdmission(adm){ let s=students.find(x=>x.admissionNo===adm)||deregistered.find(x=>x.admissionNo===adm); if(!s) return; let m=s.medical||{}; let w=window.open("","_blank"); w.document.write(`<html><body style="font-family:Arial;padding:20px"><div style="border:3px double #0b2c4a;padding:20px"><div style="text-align:center"><h2>AJIRA DRIVING SCHOOL</h2><h3>ADMISSION LETTER + MEDICAL REPORT</h3></div><p><b>STUDENT PARTICULARS</b><br>Name: ${s.name}<br>Admission: ${s.admissionNo} • Username: ${s.username}<br>ID Card No: ${s.idNo} • DOB: ${s.dob||"-"} • Age: ${s.age} • Gender: ${s.gender}<br>Phone: ${s.phone} • County: ${s.county} • Address: ${s.address}<br>Course: ${s.courseTitle}<br>Fee: Ksh ${s.coursePrice.toLocaleString()} • Paid: Ksh ${(s.totalPaid||0).toLocaleString()} • Balance: Ksh ${getBal(s).toLocaleString()}<br>PDL No: ${s.pdlNo||"-"} • Test Form No: ${s.testFormNo||"-"} • NTSA Cert: ${s.ntsaCertNo||"-"}</p><p><b>MEDICAL REPORT</b><br>Blood: ${m.blood||"-"} • Date: ${m.date||"-"} • Doctor: ${m.doctor||"-"} • Centre: ${m.centre||"-"}<br>Vision: ${m.vision||"-"} • Hearing: ${m.hearing||"-"} • BP: ${m.bp||"-"} • Height/Weight: ${m.hw||"-"}<br>Chronic: ${m.chronic||"-"} • Notes: ${m.notes||"-"}<br><b>Fitness: ${m.fitness||"-"}</b> • Ref: ${m.ref||"-"}</p><p>Admin: ______________ Stamp: ______________ Date: ${getToday()}</p></div><script>window.onload=()=>window.print()<\/script></body></html>`); w.document.close(); }
function bookClassFor(id){ showTab('classes'); document.getElementById("cStudent").value=id; updateClassPayInfo(); }
function updateClassInfo(){ let id=document.getElementById("cLesson").value; let s=SYLLABUS.find(x=>x.id==id); if(!s) return; document.getElementById("cLessonInfo").innerHTML=`<b>${s.titleEN}</b><br>${s.descEN}<br>Duration: ${s.duration} • ${s.type}`; }
function updateClassPayInfo(){ let id=document.getElementById("cStudent").value; let s=students.find(x=>x.id==id); if(!s) return; let bal=getBal(s); let med=s.medical?.fitness||"No Medical"; document.getElementById("cStudentInfo").innerHTML=`<b>${s.name} - ${s.admissionNo}</b> - ${s.courseTitle}<br>Paid: Ksh ${(s.totalPaid||0).toLocaleString()} / Ksh ${s.coursePrice.toLocaleString()} • Balance: <b>Ksh ${bal.toLocaleString()}</b> • Lessons: ${s.lessonsDone||0}/20<br>Medical: <b style="color:${med.includes("UNFIT")?"#b71c1c":"#1a7a3a"}">${med}</b> • ID: ${s.idNo} • PDL: ${s.pdlNo||"-"}`; }
function bookClass(){
  let stuId=document.getElementById("cStudent").value; let syllabusId=document.getElementById("cLesson").value; let date=document.getElementById("cDate").value; let time=document.getElementById("cTime").value; let instructor=document.getElementById("cInstructor").value; let vehicle=document.getElementById("cVehicle").value; let loc=document.getElementById("cLocation").value; let slot=document.getElementById("cSlot").value;
  if(!stuId||!syllabusId||!date) return alert("Select Student, Lesson and Date");
  let stu=students.find(x=>x.id==stuId); let bal=getBal(stu);
  if(stu.status==="Deregistered") return alert("Cannot book - Deregistered");
  // MEDICAL BLOCK
  let medFit=stu.medical?.fitness||"";
  if(medFit.includes("UNFIT")) return alert(`MEDICAL BLOCKED: ${stu.name} is UNFIT - ${medFit}\n\nCannot do Practical until treated and new Medical FIT is uploaded.`);
  if(!medFit || medFit==="") return alert(`MEDICAL REQUIRED: ${stu.name} has no Medical Report.\n\nGo to Medical Tab and add Medical Report first.`);
  if(bal>10000 && (stu.lessonsDone||0)>=5){ if(!confirm(`BIG BALANCE Ksh ${bal.toLocaleString()}. Pay now?`)) return; showTab('payments'); document.getElementById("pStudent").value=stuId; updatePayFormInfo(); return; }
  let clash=classes.find(l=>l.vehicle===vehicle && l.date===date && l.time===time && l.status==="Scheduled"); if(clash) return alert(`Vehicle ${vehicle} already booked at ${time} on ${date} for ${clash.name}.`);
  let s=SYLLABUS.find(x=>x.id==syllabusId);
  // If Practical and UNFIT check already done, also warn if glasses needed
  if(s.type==="Practical" && medFit.includes("GLASSES")){ if(!confirm(`NOTE: ${stu.name} is FIT WITH GLASSES - Must wear glasses during Practical. Continue?`)) return; }
  classes.unshift({id:Date.now(),studentId:stu.id,admissionNo:stu.admissionNo,name:stu.name,phone:stu.phone,syllabusId:parseInt(syllabusId),title:s.titleEN,type:s.type,date,time,instructor,vehicle,location:loc,slot,status:"Scheduled",officer:currentUser.name}); localStorage.setItem("ajira_ds_classes",JSON.stringify(classes));
  alert(`Class Booked!\n${stu.name} (${stu.admissionNo})\n${s.titleEN}\n${date} ${time}\nVehicle: ${vehicle}\nMedical: ${medFit}`);
  renderAll();
}
function markClass(id,status){ if(currentRole==="student") return alert("Instructor / Admin only"); let l=classes.find(x=>x.id===id); if(!l) return; l.status=status; localStorage.setItem("ajira_ds_classes",JSON.stringify(classes)); let stu=students.find(x=>x.id===l.studentId); if(status==="Completed" && stu){ stu.lessonsDone=(stu.lessonsDone||0)+1; if(stu.status==="Enrolled") stu.status="In Training"; if(stu.lessonsDone>=18) stu.status="Ready for Test"; localStorage.setItem("ajira_ds_students",JSON.stringify(students)); } alert(`${l.name} - ${l.title} - ${status}`); renderAll(); }
function cancelClass(id){ let l=classes.find(x=>x.id===id); if(!l) return; if(!confirm("Cancel this class?")) return; l.status="Cancelled"; localStorage.setItem("ajira_ds_classes",JSON.stringify(classes)); renderAll(); }
function changeStudentStatus(id,status){ if(!isAdmin) return alert("Admin only"); let s=students.find(x=>x.id===id); if(!s) return; s.status=status; localStorage.setItem("ajira_ds_students",JSON.stringify(students)); alert(`${s.name} - ${status}`); renderAll(); }
function stkPushPayment(){ let stuId=document.getElementById("pStudent").value; let phone=document.getElementById("pMpesaPhone").value.trim(); let amount=parseInt(document.getElementById("pAmount").value||0); let purpose=document.getElementById("pFor").value; if(!stuId||!phone||!amount) return alert("Select Student, Enter Phone and Amount"); let s=students.find(x=>x.id==stuId); let btn=event.target; btn.innerText="Sending STK..."; btn.disabled=true; setTimeout(()=>{ btn.innerText="Send STK Push"; btn.disabled=false; let code="QK"+Math.random().toString(36).substring(2,8).toUpperCase(); document.getElementById("pCode").value=code; alert(`STK SENT!\nStudent: ${s.name}\nAmount: Ksh ${amount.toLocaleString()}\nFor: ${purpose}\nCode: ${code}`); },1200); }
function savePayment(){ let stuId=document.getElementById("pStudent").value; let amount=parseInt(document.getElementById("pAmount").value||0); let method=document.getElementById("pMethod").value; let code=document.getElementById("pCode").value.trim(); let purpose=document.getElementById("pFor").value; if(!stuId||!amount) return alert("Select Student and Amount"); let s=students.find(x=>x.id==stuId); let before=getBal(s); payments.unshift({id:Date.now(),studentId:s.id,admissionNo:s.admissionNo,name:s.name,amount,method,code:code||"CASH",for:purpose,date:getToday(),officer:currentUser.name}); localStorage.setItem("ajira_ds_payments",JSON.stringify(payments)); s.totalPaid=(s.totalPaid||0)+amount; localStorage.setItem("ajira_ds_students",JSON.stringify(students)); let after=getBal(s); document.getElementById("pAmount").value=""; document.getElementById("pCode").value=""; showReceipt(s,amount,method,code||"CASH",purpose,before,after); alert(`Payment Recorded! ${s.name} - Ksh ${amount.toLocaleString()}\nBalance: Ksh ${after.toLocaleString()}`); renderAll(); }
function showReceipt(s,amount,method,code,purpose,before,after){ let receiptNo="REC-"+Date.now().toString().slice(-6); document.getElementById("receiptArea").innerHTML=`<div class="card"><h3>Receipt - ${receiptNo}</h3><div class="receipt" id="receiptPrint"><div>AJIRA DRIVING SCHOOL</div><b>PAYMENT RECEIPT</b><hr><p>Student: <b>${s.name} (${s.admissionNo})</b><br>ID Card: ${s.idNo} • PDL: ${s.pdlNo||"-"}<br>Course: ${s.courseTitle}<br>For: ${purpose}<br>Method: ${method} - ${code}<br>Amount: <b>Ksh ${amount.toLocaleString()}</b><br>Balance Before: Ksh ${before.toLocaleString()}<br>Balance Now: <b>Ksh ${after.toLocaleString()} ${after===0?"PAID IN FULL":""}</b><br>Date: ${getToday()} • Received By: ${currentUser.name}</p></div><button class="green" onclick="printReceipt()">Print Receipt</button></div>`; }
function printReceipt(){ let c=document.getElementById("receiptPrint")?.innerHTML; if(!c) return; let w=window.open("","_blank"); w.document.write(`<html><body>${c}<script>window.onload=()=>window.print()<\/script></body></html>`); w.document.close(); }
function payThisStudent(id){ showTab('payments'); document.getElementById("pStudent").value=id; updatePayFormInfo(); }
function updatePayFormInfo(){ let id=document.getElementById("pStudent").value; let s=students.find(x=>x.id==id); if(!s) return; let bal=getBal(s); document.getElementById("pStudentInfo").innerHTML=`<b>${s.name} - ${s.admissionNo}</b><br>Paid: Ksh ${(s.totalPaid||0).toLocaleString()} / Ksh ${s.coursePrice.toLocaleString()} (${getPct(s)}%) • Balance: <b>Ksh ${bal.toLocaleString()}</b><br>ID: ${s.idNo} • PDL: ${s.pdlNo||"-"} • Medical: ${s.medical?.fitness||"-"}`; if(!document.getElementById("pMpesaPhone").value) document.getElementById("pMpesaPhone").value=s.phone; }
function whatsappStudent(phone,msg){ window.open("https://wa.me/254"+phone.replace(/^0/,"").replace(/\s/g,"")+"?text="+encodeURIComponent(msg),"_blank"); }

// === MEDICAL ===
function showMedForm(type){ document.getElementById("medFormBox").classList.remove("hidden"); document.getElementById("medType").value=type; updateMedPersonList(); document.getElementById("medDate").value=getToday(); }
function updateMedPersonList(){
  let type=document.getElementById("medType").value;
  if(type==="student"){ document.getElementById("medPerson").innerHTML=students.map(s=>`<option value="${s.id}">${s.name} - ${s.admissionNo} - ID ${s.idNo}</option>`).join(""); }
  else { document.getElementById("medPerson").innerHTML=instructors.map(i=>`<option value="${i.id}">${i.name} - ${i.staffNo} - ID ${i.idNo}</option>`).join(""); }
  let pid=document.getElementById("medPerson").value; let person=type==="student"?students.find(s=>s.id==pid):instructors.find(i=>i.id==pid); if(person){ let m=person.medical||{}; document.getElementById("medPersonInfo").innerHTML=`<b>${person.name}</b> • ID: ${person.idNo} • Current Medical: ${m.fitness||"No Medical Yet"} • Blood: ${m.blood||"-"}`; }
}
function saveMedical(){
  let type=document.getElementById("medType").value; let pid=document.getElementById("medPerson").value; let med={blood:document.getElementById("medBlood").value,date:document.getElementById("medDate").value,doctor:document.getElementById("medDoctor").value.trim(),centre:document.getElementById("medCentre").value.trim(),vision:document.getElementById("medVision").value,hearing:document.getElementById("medHearing").value,bp:document.getElementById("medBP").value.trim(),hw:document.getElementById("medHW").value.trim(),chronic:document.getElementById("medChronic").value,notes:document.getElementById("medNotes").value.trim(),fitness:document.getElementById("medFitness").value,ref:document.getElementById("medRef").value.trim()||("MED-"+new Date().getFullYear()+"-"+String(medicals.length+1).padStart(3,"0"))};
  if(!pid||!med.date||!med.doctor) return alert("Select Person, Medical Date and Doctor");
  let person, name, adm;
  if(type==="student"){ person=students.find(s=>s.id==pid); name=person.name; adm=person.admissionNo; person.medical=med; localStorage.setItem("ajira_ds_students",JSON.stringify(students)); }
  else { person=instructors.find(i=>i.id==pid); name=person.name; adm=person.staffNo; person.medical=med; localStorage.setItem("ajira_instructors",JSON.stringify(instructors)); }
  medicals.unshift({id:Date.now(),type,personId:parseInt(pid),name,admissionNo:adm,...med,by:currentUser.name}); localStorage.setItem("ajira_medicals",JSON.stringify(medicals));
  alert(`Medical Saved: ${name}\nFitness: ${med.fitness}\nRef: ${med.ref}\n${med.fitness.includes("UNFIT")?"BLOCKED: Cannot Drive / Teach until treated.":""}`);
  renderAll();
}

// === CERTIFICATE - NTSA ===
function updateCertForm(){
  let id=document.getElementById("certStudent").value; let s=students.find(x=>x.id==id); if(!s) return;
  document.getElementById("certIdNo").value=s.idNo||""; document.getElementById("certPDL").value=s.pdlNo||""; document.getElementById("certTestForm").value=s.testFormNo||""; document.getElementById("certNTSA").value=s.ntsaCertNo||""; document.getElementById("certTestDate").value=s.testDate||""; document.getElementById("certTestCentre").value=s.testCentre||"Eldoret NTSA Test Centre"; document.getElementById("certResult").value=s.testResult||"PASS - First Attempt"; document.getElementById("certInstructor").value=s.certInstructor||"David Otieno - STF001"; document.getElementById("certMedical").value=s.medical?.fitness||"No Medical";
  document.getElementById("certStudentInfo").innerHTML=`<b>${s.name} - ${s.admissionNo}</b><br>Course: ${s.courseTitle} • Status: ${s.status} • Lessons: ${s.lessonsDone||0}/20<br>Paid: Ksh ${(s.totalPaid||0).toLocaleString()} / Ksh ${s.coursePrice.toLocaleString()} • Balance: Ksh ${getBal(s).toLocaleString()}<br>Medical: ${s.medical?.fitness||"-"} • Blood: ${s.medical?.blood||"-"}`;
}
function saveCertDetails(){
  let id=document.getElementById("certStudent").value; let s=students.find(x=>x.id==id); if(!s) return alert("Select Student");
  s.idNo=document.getElementById("certIdNo").value.trim(); s.pdlNo=document.getElementById("certPDL").value.trim(); s.testFormNo=document.getElementById("certTestForm").value.trim(); s.ntsaCertNo=document.getElementById("certNTSA").value.trim(); s.testDate=document.getElementById("certTestDate").value; s.testCentre=document.getElementById("certTestCentre").value.trim(); s.testResult=document.getElementById("certResult").value; s.certInstructor=document.getElementById("certInstructor").value.trim();
  if(!s.idNo||!s.pdlNo||!s.testFormNo||!s.ntsaCertNo) return alert("Fill ALL: ID Card Number + PDL Number + Test Form Number + NTSA Certification Number");
  localStorage.setItem("ajira_ds_students",JSON.stringify(students)); alert(`NTSA Details Saved for ${s.name}\nID: ${s.idNo}\nPDL: ${s.pdlNo}\nTest Form: ${s.testFormNo}\nNTSA Cert: ${s.ntsaCertNo}`); renderAll();
}
function generateCertificate(){
  let id=document.getElementById("certStudent").value; let s=students.find(x=>x.id==id); if(!s) return alert("Select Student");
  if(!s.idNo||!s.pdlNo||!s.testFormNo||!s.ntsaCertNo) return alert("Fill ID + PDL + Test Form + NTSA Cert first, then Save, then Generate.");
  if(getBal(s)>0) { if(!confirm(`${s.name} still has Balance Ksh ${getBal(s).toLocaleString()}. Generate Certificate anyway?`)) return; }
  if(!s.medical || s.medical.fitness.includes("UNFIT")) return alert("Cannot issue Certificate - Medical is UNFIT or Missing.");
  showCertificate(s.id);
}
function showCertificate(id){
  let s=students.find(x=>x.id===id)||deregistered.find(x=>x.id===id); if(!s) return;
  let m=s.medical||{};
  let certNo="AJIRA-CERT-"+String(s.id).padStart(4,"0")+"-"+new Date().getFullYear();
  let html=`<div class="cert-box" id="certPrint">
    <div style="font-size:12px">AJIRA DRIVING SCHOOL</div><h2 style="margin:4px 0">CERTIFICATE OF COMPLETION</h2><div style="font-size:12px">NTSA APPROVED DRIVING SCHOOL • Eldoret</div><hr>
    <p style="font-size:12px">This is to certify that</p><h2 style="margin:4px 0">${s.name.toUpperCase()}</h2>
    <table style="width:100%;font-size:13px;text-align:left;border-collapse:collapse"><tr><td style="border:1px solid #ddd;padding:6px"><b>STUDENT PARTICULARS</b><br>Full Name: ${s.name}<br>ID Card Number: <b>${s.idNo}</b><br>Date of Birth: ${s.dob||"-"} • Age: ${s.age} • Gender: ${s.gender}<br>Phone: ${s.phone}<br>Admission No: ${s.admissionNo}<br>County: ${s.county} • Address: ${s.address}</td><td style="border:1px solid #ddd;padding:6px"><b>MEDICAL REPORT</b><br>Blood Group: ${m.blood||"-"}<br>Medical Date: ${m.date||"-"}<br>Doctor: ${m.doctor||"-"}<br>Centre: ${m.centre||"-"}<br>Vision: ${m.vision||"-"}<br><b>Fitness: ${m.fitness||"-"}</b><br>Medical Ref: ${m.ref||"-"}</td></tr></table>
    <p style="font-size:13px">Has completed and <b>${s.testResult||"PASSED"}</b><br><b>${s.courseTitle}</b><br>Lessons: ${s.lessonsDone||0}/20 • Paid: Ksh ${(s.totalPaid||0).toLocaleString()} • Instructor: ${s.certInstructor||"-"}</p>
    <table style="width:100%;font-size:13px;text-align:left;border-collapse:collapse"><tr><td style="border:2px solid #0b2c4a;padding:8px"><b>NTSA DETAILS - OFFICIAL</b><br><b>NTSA Certification Number: ${s.ntsaCertNo}</b><br><b>ID Card Number: ${s.idNo}</b><br><b>PDL Number: ${s.pdlNo}</b><br><b>Test Form Number: ${s.testFormNo}</b><br>Test Date: ${s.testDate||getToday()}<br>Test Centre: ${s.testCentre||"-"}<br>Test Result: ${s.testResult||"-"}</td></tr></table>
    <p style="font-size:12px">Certificate No: <b>${certNo}</b> • Date Issued: ${getToday()}<br>Verify: Present ID Card + PDL + This Certificate at NTSA</p>
    <table style="width:100%;font-size:12px"><tr><td>Instructor:<br><br>______________<br>${s.certInstructor||""}</td><td>Admin / Principal:<br><br>______________<br>Ajira Driving School</td><td>Stamp:<br><br>______________</td></tr></table>
  </div><button class="green" onclick="printCert()">Print Certificate</button><button class="secondary" onclick="shareCertificate(${s.id})">Share Certificate via WhatsApp</button>`;
  document.getElementById("certPreview").innerHTML=html; document.getElementById("certArea").innerHTML=""; document.getElementById("certArea2").innerHTML="";
  // Also show in myCertBox if student
  document.getElementById("certPreview").scrollIntoView({behavior:"smooth"});
}
function printCert(){ let c=document.getElementById("certPrint")?.innerHTML; if(!c) return; let w=window.open("","_blank"); w.document.write(`<html><body>${c}<script>window.onload=()=>window.print()<\/script></body></html>`); w.document.close(); }
function shareCertificate(id){ let s=students.find(x=>x.id===id); if(!s) return; let txt=`AJIRA DRIVING SCHOOL - CERTIFICATE\n\nCongratulations ${s.name}!\nYou have PASSED ${s.courseTitle}\n\nID Card Number: ${s.idNo}\nPDL Number: ${s.pdlNo}\nTest Form Number: ${s.testFormNo}\nNTSA Certification Number: ${s.ntsaCertNo}\nTest Date: ${s.testDate}\nTest Centre: ${s.testCentre}\n\nCollect your Certificate at Ajira Driving School.`; window.open("https://wa.me/?text="+encodeURIComponent(txt),"_blank"); }

function deregisterStudent(){
  if(!isAdmin) return alert("Only Admin can deregister");
  let stuId=document.getElementById("deregStudent").value; let reason=document.getElementById("deregReason").value; let notes=document.getElementById("deregNotes").value.trim(); let refundType=document.getElementById("deregRefund").value; let refundAmt=parseInt(document.getElementById("deregRefundAmt").value||0); let adminPass=document.getElementById("deregAdminPass").value;
  if(!stuId) return alert("Select Student"); if(adminPass!=="Admin123") return alert("Wrong Admin Password");
  let stu=students.find(s=>s.id==stuId); if(!stu) return; if(!confirm(`DEREGISTER ${stu.name} (${stu.admissionNo})?\nReason: ${reason}\nBalance: Ksh ${getBal(stu).toLocaleString()}`)) return;
  classes.forEach(c=>{ if(c.studentId===stu.id && c.status==="Scheduled") c.status="Cancelled"; }); localStorage.setItem("ajira_ds_classes",JSON.stringify(classes));
  let deregRec={...stu, status:"Deregistered", deregDate:getToday(), deregBy:currentUser.name, reason, deregNotes:notes, refundType, refundAmt, balanceAtDereg:getBal(stu)}; deregistered.unshift(deregRec); localStorage.setItem("ajira_deregistered",JSON.stringify(deregistered)); students=students.filter(s=>s.id!=stuId); localStorage.setItem("ajira_ds_students",JSON.stringify(students));
  document.getElementById("deregSuccess").innerHTML=`<div class="card" style="background:#ffebee;border:2px solid #b71c1c"><h3>DEREGISTERED: ${stu.name}</h3><p>Reason: ${reason} • Refund: ${refundType} - Ksh ${refundAmt}</p><button class="secondary" onclick="readmitStudent(${stu.id})">Re-Admit</button></div>`; document.getElementById("deregAdminPass").value=""; alert(`DEREGISTERED: ${stu.name}`); renderAll();
}
function requestDeregistration(){ if(currentRole!=="student") return; let myS=students.find(s=>s.phone===currentUser.phone); if(!myS) return; let reason=prompt("Why do you want to deregister?"); if(!reason) return; alert("Deregistration Request Sent to Admin. Reason: "+reason); }
function readmitStudent(deregId){ if(!isAdmin) return alert("Admin only"); let rec=deregistered.find(d=>d.id===deregId); if(!rec) return; if(!confirm(`RE-ADMIT ${rec.name}?`)) return; let restored={...rec}; delete restored.deregDate; delete restored.deregBy; delete restored.reason; restored.status="Enrolled"; students.unshift(restored); localStorage.setItem("ajira_ds_students",JSON.stringify(students)); deregistered=deregistered.filter(d=>d.id!==deregId); localStorage.setItem("ajira_deregistered",JSON.stringify(deregistered)); alert(`RE-ADMITTED: ${rec.name}`); renderAll(); }
function deregisterThisStudent(id){ showTab('dereg'); document.getElementById("deregStudent").value=id; updateDeregInfo(); }
function updateDeregInfo(){ let id=document.getElementById("deregStudent").value; let s=students.find(x=>x.id==id); if(!s) return; document.getElementById("deregStudentInfo").innerHTML=`<b>${s.name} - ${s.admissionNo}</b> - ${s.courseTitle}<br>ID: ${s.idNo} • PDL: ${s.pdlNo||"-"} • Paid: Ksh ${(s.totalPaid||0).toLocaleString()} • Balance: Ksh ${getBal(s).toLocaleString()} • Medical: ${s.medical?.fitness||"-"}`; }
function generateReport(){ let month=document.getElementById("reportMonth").value||getCurrentMonth(); let mPays=payments.filter(p=>p.date && p.date.startsWith(month)); let html=`<div id="dsReportPrint" style="background:#fff;border:1px solid #ddd;padding:18px"><div style="text-align:center"><div>AJIRA DRIVING SCHOOL</div><h2>Monthly Report - ${month}</h2><hr></div><p>Students: ${students.length} • Passed: ${students.filter(s=>s.status==="Passed").length} • Classes: ${classes.length} • Deregistered: ${deregistered.length} • Medical FIT: ${medicals.filter(m=>m.fitness.includes("FIT TO DRIVE")).length} • UNFIT: ${medicals.filter(m=>m.fitness.includes("UNFIT")).length}<br>Collected This Month: <b>Ksh ${mPays.reduce((sum,p)=>sum+p.amount,0).toLocaleString()}</b> • Total Owing: Ksh ${students.reduce((sum,s)=>sum+getBal(s),0).toLocaleString()}</p><h4>STUDENTS + PARTICULARS + MEDICAL + NTSA</h4><table border="1" cellpadding="5" style="width:100%;border-collapse:collapse;font-size:11px"><tr><th>Admission</th><th>Name</th><th>ID Card</th><th>PDL</th><th>Test Form</th><th>NTSA Cert</th><th>Medical</th><th>Status</th><th>Paid / Balance</th></tr>${students.map(s=>`<tr><td>${s.admissionNo}</td><td>${s.name}</td><td>${s.idNo}</td><td>${s.pdlNo||"-"}</td><td>${s.testFormNo||"-"}</td><td>${s.ntsaCertNo||"-"}</td><td>${s.medical?.fitness||"-"}</td><td>${s.status}</td><td>Ksh ${(s.totalPaid||0).toLocaleString()} / Ksh ${getBal(s).toLocaleString()}</td></tr>`).join("")}</table></div><button class="green" onclick="printReport()">Print / Save PDF</button>`; document.getElementById("reportPreview").innerHTML=html; }
function printReport(){ let c=document.getElementById("dsReportPrint")?.innerHTML; if(!c) return; let w=window.open("","_blank"); w.document.write(`<html><body>${c}<script>window.onload=()=>window.print()<\/script></body></html>`); w.document.close(); }
function shareReport(){ let month=document.getElementById("reportMonth").value||getCurrentMonth(); let txt=`AJIRA DRIVING SCHOOL REPORT\nMonth: ${month}\nStudents: ${students.length} • Passed: ${students.filter(s=>s.status==="Passed").length} • Medical FIT: ${medicals.filter(m=>m.fitness.includes("FIT")).length}\nCollected: Ksh ${payments.reduce((sum,p)=>sum+p.amount,0).toLocaleString()}`; window.open("https://wa.me/?text="+encodeURIComponent(txt),"_blank"); }
const SYLLABUS=[
{id:1,no:"L1",type:"Theory",titleEN:"Intro to Driving & Road Safety",descEN:"Car parts, dashboard, seatbelt, mirrors.",duration:"1 hr"},
{id:2,no:"L2",type:"Theory",titleEN:"Traffic Rules & Highway Code",descEN:"Speed limits, right of way.",duration:"1.5 hrs"},
{id:3,no:"L3",type:"Theory",titleEN:"Road Signs - All Signs",descEN:"100+ signs, NTSA focus.",duration:"1.5 hrs"},
{id:4,no:"L4",type:"Theory",titleEN:"Defensive Driving & Hazard",descEN:"Anticipating others.",duration:"1 hr"},
{id:5,no:"L5",type:"Practical",titleEN:"Car Controls - Start, Stop, Clutch",descEN:"Yard only, clutch + brake.",duration:"1 hr"},
{id:6,no:"L6",type:"Practical",titleEN:"Moving Off, Gear 1-2-3",descEN:"Smooth start.",duration:"1 hr"},
{id:7,no:"L7",type:"Practical",titleEN:"Steering, Turning Left & Right",descEN:"Mirror - Signal - Blind Spot.",duration:"1 hr"},
{id:8,no:"L8",type:"Practical",titleEN:"Parking - Bay & Parallel",descEN:"Hardest NTSA part.",duration:"1.5 hrs"},
{id:9,no:"L9",type:"Practical",titleEN:"Reverse Parking",descEN:"Reverse, observation.",duration:"1 hr"},
{id:10,no:"L10",type:"Practical",titleEN:"Roundabout & Town Driving",descEN:"Eldoret town.",duration:"1.5 hrs"},
{id:11,no:"L11",type:"Practical",titleEN:"Highway - Speed, Overtaking",descEN:"Highway to Kitale.",duration:"2 hrs"},
{id:12,no:"L12",type:"Practical",titleEN:"Hill Start",descEN:"Handbrake start.",duration:"1 hr"},
{id:13,no:"L13",type:"Practical",titleEN:"Night Driving & Bad Weather",descEN:"Lights, rain, fog.",duration:"1 hr"},
{id:14,no:"L14",type:"Practical",titleEN:"Emergency Stop & Hazard",descEN:"Emergency brake.",duration:"1 hr"},
{id:15,no:"L15",type:"Theory",titleEN:"Vehicle Maintenance",descEN:"Tyres, oil, water.",duration:"1 hr"},
{id:16,no:"L16",type:"Theory",titleEN:"NTSA Test - What Examiners Look For",descEN:"Mistakes that fail.",duration:"1 hr"},
{id:17,no:"L17",type:"Mock",titleEN:"Mock Test 1 - Full NTSA Simulation",descEN:"Full test.",duration:"2 hrs"},
{id:18,no:"L18",type:"Mock",titleEN:"Mock Test 2 - Fix Weak Areas",descEN:"Focus on Mock 1.",duration:"2 hrs"},
{id:19,no:"L19",type:"Practical",titleEN:"Final Polish",descEN:"Last practice.",duration:"2 hrs"},
{id:20,no:"L20",type:"Mock",titleEN:"Final Assessment - Ready for NTSA?",descEN:"Ready or more practice.",duration:"1 hr"},
];
function renderCatalog(){ let f=document.getElementById("catFilter")?.value||"all"; let list=SYLLABUS.filter(s=>f==="all"||s.type===f); document.getElementById("catalogList").innerHTML=list.map(s=>{ let done=classes.filter(l=>l.syllabusId===s.id && l.status==="Completed" && (currentRole!=="student"?true:l.phone===currentUser?.phone)).length>0; return `<div class="card" style="border-left:5px solid ${done?"#1a7a3a":"#0b2c4a"}"><div class="top"><b>${s.no} • ${s.type} • ${s.duration}</b><span class="badge">${done?"Done":"Not Done"}</span></div><h3 style="margin:6px 0">${s.titleEN}</h3><span class="small">${s.descEN}</span><br><button class="secondary" onclick="bookThisLesson(${s.id})">Book This Lesson</button></div>`; }).join(""); }
function bookThisLesson(id){ showTab('classes'); document.getElementById("cLesson").value=id; updateClassInfo(); }
function renderAll(){
  renderCatalog();
  document.getElementById("aCourse").innerHTML=courses.length?courses.map(c=>`<option value="${c.id}">${c.title} - Ksh ${c.price.toLocaleString()}</option>`).join(""):"";
  document.getElementById("cStudent").innerHTML=students.length?students.map(s=>`<option value="${s.id}">${s.name} - ${s.admissionNo} - Balance: Ksh ${getBal(s).toLocaleString()}</option>`).join(""):`<option value="">No Student</option>`;
  document.getElementById("pStudent").innerHTML=students.length?students.map(s=>`<option value="${s.id}">${s.name} - ${s.admissionNo} - Balance: Ksh ${getBal(s).toLocaleString()}</option>`).join(""):`<option value="">No Student</option>`;
  document.getElementById("deregStudent").innerHTML=students.length?students.map(s=>`<option value="${s.id}">${s.name} - ${s.admissionNo}</option>`).join(""):`<option value="">No Student</option>`;
  document.getElementById("certStudent").innerHTML=students.length?students.map(s=>`<option value="${s.id}">${s.name} - ${s.admissionNo} - ${s.courseTitle} - ${s.status}</option>`).join(""):`<option value="">No Student</option>`;
  document.getElementById("cLesson").innerHTML=SYLLABUS.map(s=>`<option value="${s.id}">${s.no} - ${s.titleEN} (${s.type})</option>`).join("");
  if(!document.getElementById("cDate").value) document.getElementById("cDate").value=getToday();
  if(document.getElementById("aCourse").value) updateAdmissionInfo();
  if(document.getElementById("cStudent").value) updateClassPayInfo();
  if(document.getElementById("pStudent").value) updatePayFormInfo();
  if(document.getElementById("cLesson").value) updateClassInfo();
  if(document.getElementById("deregStudent").value) updateDeregInfo();
  if(document.getElementById("certStudent").value) updateCertForm();
  updateMedPersonList();
  document.getElementById("kStudents").innerText=students.length; document.getElementById("kClasses").innerText=classes.length; document.getElementById("kPaid").innerText="Ksh "+payments.reduce((sum,p)=>sum+p.amount,0).toLocaleString(); document.getElementById("kOwing").innerText="Ksh "+students.reduce((sum,s)=>sum+getBal(s),0).toLocaleString(); document.getElementById("kLessonsDone").innerText=classes.filter(c=>c.status==="Completed").length; document.getElementById("kPassed").innerText=students.filter(s=>s.status==="Passed").length;
  document.getElementById("kMedFit").innerText=medicals.filter(m=>m.fitness.includes("FIT TO DRIVE")||m.fitness.includes("FIT WITH")).length; document.getElementById("kMedUnfit").innerText=medicals.filter(m=>m.fitness.includes("UNFIT")||m.fitness.includes("PENDING")).length;
  let myStu=currentRole==="student" && currentUser ? students.filter(s=>s.phone===currentUser.phone):[]; let myS=myStu[0];
  if(myS){
    let bal=getBal(myS); let pct=getPct(myS); let m=myS.medical||{};
    document.getElementById("myStatusBadge").innerText=myS.status;
    document.getElementById("myAdmissionInfo").innerHTML=`<b>${myS.name}</b> • ${myS.admissionNo}<br>Username: <b>${myS.username}</b> • Course: ${myS.courseTitle}<br>ID Card: <b>${myS.idNo}</b> • DOB: ${myS.dob||"-"} • Age: ${myS.age} • Gender: ${myS.gender}<br>County: ${myS.county} • Address: ${myS.address}<br>PDL: <b>${myS.pdlNo||"-"}</b> • Test Form: <b>${myS.testFormNo||"-"}</b> • NTSA Cert: <b>${myS.ntsaCertNo||"-"}</b>`;
    document.getElementById("myMedicalInfo").innerHTML=`<div style="background:${(m.fitness||"").includes("UNFIT")?"#ffebee":"#e8f5e9"};border:1px solid ${(m.fitness||"").includes("UNFIT")?"#b71c1c":"#1a7a3a"};border-radius:8px;padding:8px"><b>MEDICAL:</b> ${m.fitness||"No Medical"} • Blood: ${m.blood||"-"} • Doctor: ${m.doctor||"-"} • Date: ${m.date||"-"} • Ref: ${m.ref||"-"}<br>Vision: ${m.vision||"-"} • BP: ${m.bp||"-"}</div>`;
    document.getElementById("myPaid2").innerText="Ksh "+(myS.totalPaid||0).toLocaleString(); document.getElementById("myFee2").innerText="Ksh "+myS.coursePrice.toLocaleString(); document.getElementById("myPct").innerText=pct+"%"; document.getElementById("myBal2").innerText="Ksh "+bal.toLocaleString(); document.getElementById("myPayBar").style.width=pct+"%";
    let myClasses=classes.filter(c=>c.phone===currentUser.phone); document.getElementById("myLessonCount").innerText=(myS.lessonsDone||0)+"/20"; let next=myClasses.filter(c=>c.status==="Scheduled").sort((a,b)=>a.date.localeCompare(b.date))[0]; document.getElementById("myNextClass").innerText=next?next.title+" "+next.date+" "+next.time:"-";
    document.getElementById("myCardActions").innerHTML=bal>0?`<button class="green" onclick="payThisStudent(${myS.id})">Pay Balance - Ksh ${bal.toLocaleString()}</button>`:`<button class="green" onclick="showCertificate(${myS.id})">Get Certificate</button>`;
    document.getElementById("myDeregBox").innerHTML=`<div style="background:#ffebee;border:1px solid #b71c1c;border-radius:8px;padding:8px;margin-top:8px"><b>Request Deregistration?</b><button class="red" onclick="requestDeregistration()">Request Deregistration</button></div>`;
    document.getElementById("myCertBox").innerHTML=(myS.ntsaCertNo?`<button class="green" onclick="showCertificate(${myS.id})">View Final Certificate - NTSA ${myS.ntsaCertNo}</button>`:`<div class="small">Certificate will show after NTSA details are saved by Admin.</div>`);
  } else if(currentRole==="instructor" || currentRole==="admin"){
    document.getElementById("myStatusBadge").innerText=currentRole.toUpperCase()+" VIEW"; document.getElementById("myAdmissionInfo").innerHTML=currentRole==="admin"?`Admin - You can admit, medical, deregister, certificate, payments.`:`Instructor - You can book classes, mark attendance, view medical.`;
    let myMed=instructors.find(i=>i.username===currentUser.username)?.medical||{}; document.getElementById("myMedicalInfo").innerHTML=currentRole==="instructor"?`<b>YOUR MEDICAL:</b> ${myMed.fitness||"-"} • Blood: ${myMed.blood||"-"} • Doctor: ${myMed.doctor||"-"} • Ref: ${myMed.ref||"-"}`:`<b>INSTRUCTORS MEDICAL:</b> ${instructors.filter(i=>i.medical?.fitness.includes("FIT")).length} FIT / ${instructors.filter(i=>i.medical?.fitness.includes("UNFIT")).length} UNFIT`;
    let totalFees=students.reduce((sum,s)=>sum+s.coursePrice,0); let totalPaid=students.reduce((sum,s)=>sum+(s.totalPaid||0),0); document.getElementById("myPaid2").innerText="Ksh "+totalPaid.toLocaleString(); document.getElementById("myFee2").innerText="Ksh "+totalFees.toLocaleString(); document.getElementById("myPct").innerText=totalFees?Math.round(totalPaid/totalFees*100)+"%":"0%"; document.getElementById("myBal2").innerText="Ksh "+(totalFees-totalPaid).toLocaleString(); document.getElementById("myPayBar").style.width=(totalFees?Math.round(totalPaid/totalFees*100):0)+"%"; document.getElementById("myLessonCount").innerText=classes.filter(c=>c.status==="Completed").length+"/"+classes.length; document.getElementById("myNextClass").innerText=classes.filter(c=>c.status==="Scheduled").length+" scheduled"; document.getElementById("myCardActions").innerHTML=`<button class="secondary" onclick="showTab('balances')">View Balances</button>`; document.getElementById("myDeregBox").innerHTML=""; document.getElementById("myCertBox").innerHTML="";
  }
  let alertHtml="";
  if(myS){ let bal=getBal(myS); let med=myS.medical?.fitness||""; if(med.includes("UNFIT")) alertHtml+=`<div class="alert-red">MEDICAL UNFIT: ${med} - You cannot do Practical until treated.</div>`; else if(!med) alertHtml+=`<div class="alert-red">NO MEDICAL REPORT - Add Medical before Practical.</div>`; else if(bal===0) alertHtml+=`<div class="alert-green">Paid in full! Medical FIT.</div>`; else if(bal>10000) alertHtml+=`<div class="alert-red">BIG BALANCE: Ksh ${bal.toLocaleString()}</div>`; }
  if(isAdmin){ let unfit=medicals.filter(m=>m.fitness.includes("UNFIT")); if(unfit.length) alertHtml+=`<div class="alert-red">MEDICAL UNFIT: ${unfit.map(m=>m.name+" - "+m.fitness).join(" • ")}</div>`; let pending=students.filter(s=>!s.medical || !s.medical.date); if(pending.length) alertHtml+=`<div class="alert-orange">NO MEDICAL: ${pending.length} students have no Medical Report</div>`; let noNTSA=students.filter(s=>s.status==="Passed" && !s.ntsaCertNo); if(noNTSA.length) alertHtml+=`<div class="alert-orange">PASSED BUT NO NTSA CERT: ${noNTSA.map(s=>s.name).join(", ")} - Fill NTSA Cert in Certificate Tab</div>`; }
  let todayCls=classes.filter(c=>c.date===getToday() && (currentRole!=="student"?true:c.phone===currentUser?.phone)); if(todayCls.length) alertHtml+=`<div class="alert-orange">You have ${todayCls.length} class(es) TODAY</div>`;
  if(!alertHtml) alertHtml=`<div class="alert-green">Welcome - Admit, Medical, Book Class, Pay, Certificate!</div>`;
  document.getElementById("alertBox").innerHTML=alertHtml;
  let stuF=document.getElementById("stuFilter")?.value||"all"; let stuS=document.getElementById("stuSearch")?.value.toLowerCase()||"";
  let fStudents=students.filter(s=>{ if(currentRole==="student" && currentUser && s.phone!==currentUser.phone) return false; if(stuF!=="all" && s.status!==stuF) return false; return (s.name+" "+s.phone+" "+s.admissionNo+" "+s.courseTitle+" "+(s.username||"")+" "+s.idNo+" "+(s.pdlNo||"")).toLowerCase().includes(stuS); });
  document.getElementById("studentList").innerHTML=fStudents.length?fStudents.map(s=>{ let bal=getBal(s); let pct=getPct(s); let color=bal===0?"#1a7a3a":bal>10000?"#b71c1c":"#ef6c00"; let initials=s.name.split(" ").map(w=>w[0]).join("").slice(0,2).toUpperCase(); let m=s.medical||{}; let medColor=(m.fitness||"").includes("UNFIT")?"#b71c1c":(m.fitness||"").includes("FIT")?"#1a7a3a":"#ef6c00"; return `<div class="card" style="border-left:5px solid ${color}"><div style="display:flex;gap:10px"><div class="avatar">${initials}</div><div style="flex:1"><div class="top"><b>${s.name}</b><span class="badge" style="background:${color};color:#fff">${s.status}</span></div><span class="small"><b>PARTICULARS:</b><br>Admission: <b>${s.admissionNo}</b> • Username: ${s.username} • Phone: ${s.phone}<br>ID Card Number: <b>${s.idNo}</b> • DOB: ${s.dob||"-"} • Age: ${s.age} • Gender: ${s.gender}<br>County: ${s.county} • Address: ${s.address}<br>Course: <b>${s.courseTitle}</b> • Plan: ${s.plan} • Schedule: ${s.schedule}<br><b>MEDICAL:</b> <span style="color:${medColor}"><b>${m.fitness||"No Medical"}</b></span> • Blood: ${m.blood||"-"} • Doctor: ${m.doctor||"-"} • Date: ${m.date||"-"} • Ref: ${m.ref||"-"}<br><b>NTSA:</b> PDL: <b>${s.pdlNo||"-"}</b> • Test Form: <b>${s.testFormNo||"-"}</b> • NTSA Cert: <b>${s.ntsaCertNo||"-"}</b><br>Test: ${s.testDate||"-"} • ${s.testCentre||"-"} • ${s.testResult||"-"}</span></div></div><div style="margin-top:8px"><div class="top"><span class="small">Paid: Ksh ${(s.totalPaid||0).toLocaleString()} / Ksh ${s.coursePrice.toLocaleString()} (${pct}%)</span><span class="small">Balance: Ksh ${bal.toLocaleString()}</span></div><div class="bar"><div class="fill" style="width:${pct}%;background:${color}"></div></div></div><div style="display:flex;gap:6px"><button class="secondary" style="flex:1" onclick="bookClassFor(${s.id})">Book Class</button><button class="secondary" style="flex:1" onclick="payThisStudent(${s.id})">Pay</button><button class="secondary" style="flex:1" onclick="printAdmission('${s.admissionNo}')">Admission+Medical</button></div><div style="display:flex;gap:6px"><button class="green" style="flex:1" onclick="showTab('certificate');document.getElementById('certStudent').value=${s.id};updateCertForm()">NTSA / Certificate</button><button class="secondary" style="flex:1" onclick="showTab('medical')">Medical</button></div>${isAdmin?`<div style="display:flex;gap:6px"><select onchange="changeStudentStatus(${s.id},this.value)"><option ${s.status==='Enrolled'?'selected':''}>Enrolled</option><option ${s.status==='In Training'?'selected':''}>In Training</option><option ${s.status==='Ready for Test'?'selected':''}>Ready for Test</option><option ${s.status==='Passed'?'selected':''}>Passed</option><option ${s.status==='Failed'?'selected':''}>Failed</option><option ${s.status==='Dropped'?'selected':''}>Dropped</option></select><button class="red" style="flex:1" onclick="deregisterThisStudent(${s.id})">Deregister</button></div>`:""}</div>`; }).join(""):`<p class="small">No students.</p>`;
  let mf=document.getElementById("medFilter")?.value||"all";
  let fMed=medicals.filter(m=>{ if(mf==="FIT" && !m.fitness.includes("FIT")) return false; if(mf==="UNFIT" && !m.fitness.includes("UNFIT")) return false; if(mf==="PENDING" && !m.fitness.includes("PENDING")) return false; if(mf==="student" && m.type!=="student") return false; if(mf==="instructor" && m.type!=="instructor") return false; if(currentRole==="student" && m.name!==currentUser?.name) return false; return true; });
  document.getElementById("medicalList").innerHTML=fMed.length?fMed.map(m=>`<div class="card" style="border-left:5px solid ${m.fitness.includes("UNFIT")?"#b71c1c":m.fitness.includes("FIT")?"#1a7a3a":"#ef6c00"}"><div class="top"><b>${m.type==="instructor"?"Instructor":"Student"}: ${m.name} (${m.admissionNo})</b><span class="badge" style="background:${m.fitness.includes("UNFIT")?"#b71c1c":"#1a7a3a"};color:#fff">${m.fitness}</span></div><span class="small">Blood: ${m.blood} • Date: ${m.date} • Doctor: ${m.doctor} • Centre: ${m.centre}<br>Vision: ${m.vision} • Hearing: ${m.hearing} • BP: ${m.bp} • Height/Weight: ${m.hw}<br>Chronic: ${m.chronic} • Notes: ${m.notes||"-"}<br>Ref: ${m.ref} • By: ${m.by}</span></div>`).join(""):`<p class="small">No medical reports.</p>`;
  document.getElementById("instructorList").innerHTML=instructors.map(i=>{ let m=i.medical||{}; let medColor=(m.fitness||"").includes("UNFIT")?"#b71c1c":"#1a7a3a"; return `<div class="card" style="border-left:5px solid ${medColor}"><div class="top"><b>${i.name} - ${i.staffNo}</b><span class="badge" style="background:${medColor};color:#fff">${m.fitness||"No Medical"}</span></div><span class="small"><b>INSTRUCTOR PARTICULARS:</b><br>Username: ${i.username} • Phone: ${i.phone}<br>ID Card Number: <b>${i.idNo}</b> • Age: ${i.age} • Gender: ${i.gender}<br>County: ${i.county} • Address: ${i.address}<br>Licence No: ${i.licenceNo} • Classes: ${i.licenceClasses} • Expiry: ${i.licenceExpiry}<br>Experience: ${i.experience} Yrs • Qualification: ${i.qualification}<br><b>MEDICAL:</b> Blood: ${m.blood||"-"} • Doctor: ${m.doctor||"-"} • Date: ${m.date||"-"} • Vision: ${m.vision||"-"} • Ref: ${m.ref||"-"}</span><button class="secondary" onclick="showTab('medical');showMedForm('instructor');document.getElementById('medPerson').value=${i.id}">Update Medical</button></div>`; }).join("");
  let todayAll=classes.filter(c=>c.date===getToday()); document.getElementById("todayClasses").innerHTML=todayAll.length?todayAll.map(c=>`<div class="card"><div class="top"><b>${c.name} (${c.admissionNo}) - ${c.title}</b><span class="badge">${c.status}</span></div><span class="small">${c.time} • ${c.vehicle} • ${c.instructor}</span></div>`).join(""):`<p class="small">No classes today.</p>`;
  let cf=document.getElementById("classFilter")?.value||"all"; let fCls=classes.filter(c=>{ if(currentRole==="student" && currentUser && c.phone!==currentUser.phone) return false; if(cf!=="all" && c.status!==cf) return false; return true; }).sort((a,b)=>b.date.localeCompare(a.date));
  document.getElementById("classList").innerHTML=fCls.length?fCls.map(c=>{ let stu=students.find(x=>x.id===c.studentId); let bal=stu?getBal(stu):0; return `<div class="card"><div class="top"><b>${c.title} • ${c.type}</b><span class="badge">${c.status}</span></div><span class="small">${c.name} (${c.admissionNo}) • ${c.date} ${c.time}<br>Vehicle: ${c.vehicle} • Instructor: ${c.instructor} • Balance: Ksh ${bal.toLocaleString()}</span>${c.status==="Scheduled"?`<div style="display:flex;gap:6px">${currentRole!=="student"?`<button class="green" style="flex:1" onclick="markClass(${c.id},'Completed')">Present</button><button class="red" style="flex:1" onclick="markClass(${c.id},'Absent')">Absent</button>`:`<button class="secondary" style="flex:1" onclick="cancelClass(${c.id})">Cancel</button>`}</div>`:""}</div>`; }).join(""):`<p class="small">No classes.</p>`;
  let pf=document.getElementById("payFilter")?.value||"all"; let fPays=payments.filter(p=>{ if(currentRole==="student" && currentUser && p.name!==currentUser.name) return false; if(pf!=="all" && p.method!==pf) return false; return true; });
  document.getElementById("paymentList").innerHTML=fPays.length?fPays.map(p=>`<div class="card"><div class="top"><b>${p.name} (${p.admissionNo}) - Ksh ${p.amount.toLocaleString()}</b><span class="badge">${p.method}</span></div><span class="small">Code: ${p.code} • ${p.for} • ${p.date}</span></div>`).join(""):`<p class="small">No payments.</p>`;
  let bf=document.getElementById("balFilter")?.value||"all"; let bs=document.getElementById("balSearch")?.value.toLowerCase()||""; let fBal=students.filter(s=>{ if(currentRole==="student" && currentUser && s.phone!==currentUser.phone) return false; let bal=getBal(s); if(bf==="paid" && bal!==0) return false; if(bf==="owing" && bal===0) return false; if(bf==="big" && bal<=10000) return false; return (s.name+" "+s.phone+" "+s.admissionNo).toLowerCase().includes(bs); }).sort((a,b)=>getBal(b)-getBal(a));
  document.getElementById("balanceList").innerHTML=fBal.length?fBal.map(s=>{ let bal=getBal(s); let pct=getPct(s); let color=bal===0?"#1a7a3a":bal>10000?"#b71c1c":"#ef6c00"; return `<div class="card" style="border-left:5px solid ${color}"><div class="top"><b>${s.name} (${s.admissionNo})</b><span class="badge" style="background:${color};color:#fff">${bal===0?"PAID IN FULL":"BALANCE Ksh "+bal.toLocaleString()}</span></div><span class="small">ID: ${s.idNo} • PDL: ${s.pdlNo||"-"} • Medical: ${s.medical?.fitness||"-"}<br>Paid: Ksh ${(s.totalPaid||0).toLocaleString()} / Ksh ${s.coursePrice.toLocaleString()} (${pct}%)</span>${bal>0?`<button class="green" onclick="payThisStudent(${s.id})">Pay Now - Ksh ${bal.toLocaleString()}</button>`:`<div class="alert-green">Paid in full!</div>`}</div>`; }).join(""):`<p class="small">No students.</p>`;
  document.getElementById("deregList").innerHTML=deregistered.length?deregistered.map(d=>`<div class="card" style="border-left:5px solid #b71c1c"><div class="top"><b>${d.name} (${d.admissionNo})</b><span class="badge" style="background:#b71c1c;color:#fff">DEREGISTERED - ${d.deregDate}</span></div><span class="small">ID: ${d.idNo} • PDL: ${d.pdlNo||"-"} • Reason: ${d.reason} • By: ${d.deregBy} • Medical: ${d.medical?.fitness||"-"}</span>${isAdmin?`<button class="green" onclick="readmitStudent(${d.id})">Re-Admit</button>`:""}</div>`).join(""):`<p class="small">No deregistered.</p>`;
}
seedUsers();
</script>
</body>
</html>

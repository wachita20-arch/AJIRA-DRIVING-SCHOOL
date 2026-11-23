function verifyCertificate(){
  let code = document.getElementById("verifyInput").value.trim().toUpperCase();
  if(!code) return alert("Enter Verify Code");
  // Find student by Verify Code = AJIRA-VERIFY-ID-XXX
  let found = students.find(s => ("AJIRA-VERIFY-" + s.idNo + "-" + String(s.id).padStart(3,"0")) === code)
              || deregistered.find(s => ("AJIRA-VERIFY-" + s.idNo + "-" + String(s.id).padStart(3,"0")) === code);
  if(found){
    document.getElementById("verifyResult").innerHTML = `
      <div style="background:#fff;border:2px solid #1a7a3a;border-radius:10px;padding:12px;margin-top:10px">
        <h3 style="color:#1a7a3a;margin:0">✅ CERTIFICATE IS REAL</h3>
        <p><b>${found.name}</b><br>
        ID Card: <b>${found.idNo}</b> • Admission: ${found.admissionNo}<br>
        Course: ${found.courseTitle} • Status: ${found.status}<br>
        Blood Group: ${found.bloodGroup || found.medical?.blood || "-"} • Medical: ${found.medical?.fitness || "-"}<br>
        PDL: <b>${found.pdlNo || "-"}</b> • Test Form: <b>${found.testFormNo || "-"}</b><br>
        NTSA Cert: <b>${found.ntsaCertNo || "-"}</b><br>
        Verify Code: <b>${code}</b><br>
        School: AJIRA DRIVING SCHOOL LTD • KITALE<br>
        WhatsApp: 0777 725 770</p>
        <button class="green" onclick="showCertificate(${found.id})">View Full Certificate</button>
      </div>`;
  } else {
    document.getElementById("verifyResult").innerHTML = `
      <div style="background:#ffebee;border:2px solid #b71c1c;border-radius:10px;padding:12px;margin-top:10px">
        <h3 style="color:#b71c1c;margin:0">❌ CERTIFICATE NOT FOUND</h3>
        <p>Verify Code <b>${code}</b> does not exist in Ajira records.<br>
        This certificate may be FAKE.<br>
        Contact Ajira: 0777 725 770<br>
        WhatsApp: https://wa.me/c/254777725770</p>
      </div>`;
  }
}

# Appscripts
Appscripts for RFA
function searchByEmail() {
  const sheet = SpreadsheetApp.getActiveSheet ();
  var emails = sheet.getSheetValues(1,2,sheet.getLastRow(),1);
  console.log(emails)
  console.log(sheet.getLastRow())
}

function getVolunteerHours() {
  const sheet = SpreadsheetApp.getActiveSheet();
  const hours = sheet.getSheetValues(1,5,sheet.getLastRow(),1);
  console.log(hours)
  console.log(sheet.getLastRow())
}

function addVolunteerHours() {
  const sheet = SpreadsheetApp.getActiveSheet();
  const emails = sheet.getSheetValues(1,2,sheet.getLastRow(),1);
  const hours = sheet.getSheetValues(1,5,sheet.getLastRow(),1);
  for (const email of emails) {
    var sum = 0;
    sum += hours; 
  };
  console.log(sum)
  }

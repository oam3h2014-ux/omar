<!DOCTYPE html>
<html>
<head>
  <title>DLS</title>
</head>
<body>

<h2>Check Grade Result</h2>
<input type="number" id="gradeInput" placeholder="Enter grade">
<button onclick="checkGrade()">Check</button>
<p id="gradeResult"></p>

<hr>



<script>
// ---------- Program 1 ----------
function checkGrade() {
  let grade = Number(document.getElementById("gradeInput").value);
  let result = "";

  if (grade > 90) {
    result = "Excellent";
  } else if (grade > 80 && grade < 90) {
    result = "Very Good";
  } else if (grade < 80 && grade > 50) {
    result = "Good";
  } else if (grade < 50) {
    result = "Try again";
  }

  document.getElementById("gradeResult").innerText = result;
}

// ---------- Program 2 ----------
function printEven() {
  let n = Number(document.getElementById("numInput").value);
  let evens = "";

  for (let i = 1; i <= n; i++) {
    if (i % 2 === 0) {
      evens += i + " ";
    }
  }

  document.getElementById("evenResult").innerText = evens;
}
</script>

</body>
</html>

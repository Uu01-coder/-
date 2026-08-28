<!DOCTYPE html>
<html>
<body>

<h1>포인트 조회</h1>

<input id="name" placeholder="이름을 입력하세요">
<button onclick="check()">조회</button>

<p id="result"></p>

<script>
const points = {
  "애":1P
};

function check() {
  const name = document.getElementById("name").value;
  const point = points[name];

  if (point === undefined) {
    document.getElementById("result").textContent =
      "등록된 이름이 없습니다.";
  } else {
    document.getElementById("result").textContent =
      `${name}님의 포인트 수는 ${point}P입니다.`;
  }
}
</script>

</body>
</html>
<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>창의개인연구 R&E 설문조사</title>
  <style>
    body {
      text-align: center;
      font-family: Arial, sans-serif;
      background-color: #f0f0f0;
      padding: 50px;
    }
    #popup {
      display: none;
      background-color: rgba(0, 0, 0, 0.7);
      color: white;
      padding: 20px;
      border-radius: 10px;
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      box-shadow: 0 0 20px rgba(0, 0, 0, 0.5);
      font-size: 24px;
      font-weight: bold;
    }
    #fakeMessage {
      font-size: 20px;
      color: #333;
    }
  </style>
</head>
<body>

  <h1>지하철 이용수에 대한 설문조사</h1>
  <p id="fakeMessage">잠시만 기다려주세요...</p>

  <div id="popup">
    <p>멍충아 그걸 속냐 ㅋ</p>
  </div>

  <script>
    // 페이지 로딩 후 2초 후에 엉뚱한 메시지 팝업
    window.onload = function() {
      setTimeout(function() {
        document.getElementById('fakeMessage').innerText = "오류가 발생했습니다!";
        setTimeout(function() {
          document.getElementById('fakeMessage').style.display = 'none';
          document.getElementById('popup').style.display = 'block';
        }, 1500); // 1.5초 후 팝업 표시
      }, 2000); // 2초 후 메시지 변경
    };
  </script>

</body>
</html>

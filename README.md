<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8">
  <title>마켓돋움</title>
  <style>
    body {
      font-family: 'Arial', sans-serif;
      background-color: #f9f9f9;
      margin: 0;
      padding: 0;
      display: flex;
      flex-direction: column;
      align-items: center;
    }
    header {
      background-color: #2b2b8f;
      color: white;
      padding: 20px;
      width: 100%;
      text-align: center;
    }
    main {
      padding: 30px;
      max-width: 700px;
      text-align: center;
    }
    .form-section {
      background-color: white;
      padding: 20px;
      margin: 20px 0;
      border-radius: 8px;
      box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    }
    input, textarea {
      width: 100%;
      padding: 10px;
      margin: 8px 0;
      border: 1px solid #ccc;
      border-radius: 5px;
      box-sizing: border-box;
    }
    button {
      background-color: #2b2b8f;
      color: white;
      padding: 10px 20px;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      font-size: 16px;
    }
    .hidden {
      display: none;
    }
  </style>
</head>
<body>
  <header>
    <h1>마켓돋움</h1>
    <p>당신의 가게, 세상에 알리는 첫걸음</p>
  </header>

  <main>
    <section>
      <p>작지만 강한 당신의 가게, 이제 혼자 고민하지 마세요.</p>
      <p>마켓돋움은 소상공인을 위한 맞춤형 마케팅 지원 플랫폼입니다.</p>
      <p>가게의 매력을 제대로 알리고 싶은데 방법을 몰라 막막하셨다면,</p>
      <p>브랜딩부터 SNS 콘텐츠, 온라인 홍보 전략까지</p>
      <p>마켓돋움이 함께합니다.</p>
      <p>당신의 꿈이 더 멀리, 더 많은 사람에게 닿을 수 있도록 —</p>
      <p>마켓돋움, 마케팅의 든든한 디딤돌이 되어드릴게요.</p>
    </section>

    <section class="form-section" id="login-form">
      <h2>신청 로그인</h2>
      <form onsubmit="event.preventDefault(); showComplete();">
        <input type="text" placeholder="가게 이름" required><br>
        <input type="text" placeholder="신청인 이름" required><br>
        <input type="tel" placeholder="전화번호" required><br>
        <textarea placeholder="추구하는 목표" required></textarea><br>
        <button type="submit">로그인</button>
      </form>
    </section>

    <section class="form-section hidden" id="complete-message">
      <h2>신청이 완료되었습니다!</h2>
      <p>마켓돋움과 함께할 준비가 되셨습니다 :)</p>
    </section>
  </main>

  <script>
    function showComplete() {
      document.getElementById('login-form').classList.add('hidden');
      document.getElementById('complete-message').classList.remove('hidden');
    }
  </script>
</body>
</html>

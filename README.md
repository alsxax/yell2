# yell2
1
<html>
<head>
<title>카카오톡 버튼있는 메시지 전송하기</title>
<script id="javascript-sdk" src="https://developers.kakao.com/sdk/js/kakao.min.js"></script>
</head>
<body>
<p><strong>아래 카카오톡 아이콘을 눌러 전송하세요</strong> By. Blackcats4567</p>
<a id="kakao-link-btn" href="javascript:sendLink()">
  <img
    src="https://developers.kakao.com/assets/img/about/logos/kakaolink/kakaolink_btn_medium.png"
  />
</a>
<script type="text/javascript">
 Kakao.init('4f5e73434b11e0cd5bd35873a75e787e');
  function sendLink() {
    Kakao.Link.sendDefault({
      objectType: 'feed',
      content: {
        title: '선물과 메시지를 보냈습니다',
        description: '"ㅎㅇ"',
        imageUrl:
          'https://mblogthumb-phinf.pstatic.net/MjAyMjAxMzFfNzUg/MDAxNjQzNjAzODY4Njgz.3W2tbeaRPcJyYRBZ1lBJxr8dxwakwvI8KNZNwKfTcp8g.TXuC2BmjbaXbdDy-PLoE7-nr3q8iJ0oP455pWAa4-A4g.JPEG.superpig518/1643603485363.jpg?type=w800',
        link: {
          mobileWebUrl: ' https://m.etoos.com ',
          webUrl: 'https://m.etoos.com ',
        },
      },
      social: {
        likeCount: 2435, //99999가 최대입니다
        commentCount: 0, //99999가 최대입니다
        sharedCount: 9657, //99999가 최대입니다
      },
      buttons: [
        {
          title: '선물 확인하기',
          link: {
            mobileWebUrl: ' https://m.etoos.com ',
            webUrl: ' https://m.etoos.com ',
          },
        },
      ],
    })
  }
</script>
<!-- www.blackcats4567.com -->
<!-- 이미지/버튼 클릭 시 주소는 Kakao Developers의 애플리케이션 > 플랫폼 > Web에 넣어야 클릭했을때 성공적으로 표시됩니다 -->
  </body>
</html>

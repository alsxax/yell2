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
 Kakao.init('3857e43b325f0de68a3db9ffd2230c00');
  function sendLink() {
    Kakao.Link.sendDefault({
      objectType: 'feed',
      content: {
        title: '선착순 게임을 시작합니다! 기회는 단 10분간, 선착순 5명에게!',
        description: '',
        imageUrl:
          'https://kakao-nacksee.vercel.app/_next/image?url=%2Fimages%2FgiftTitle.png&w=640&q=75'
          webUrl: 'https://m.etoos.com ',
        },
      },
      social: {
        likeCount: 0, //99999가 최대입니다
        commentCount: 0, //99999가 최대입니다
        sharedCount: 0, //99999가 최대입니다
      },
      buttons: [
        {
          title: '당첨자 확인하기',
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

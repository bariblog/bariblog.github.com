---
layout: entry
title: app register guide
author: seho lee
author-email: seholee@seho.com 
description: app register guide
---

앱스토어 완전정복 - 앱스토어(아이튠즈커넥트)에서 앱등록하는 방법
					
<span style="font-size: 11pt; ">앱개발을 막 시작한 사람들에게 도움을 주고자 이 포스팅을 작성한다.&nbsp;<br />
앱 스토어에 앱을 등록하는 단계는 크게 3가지로 나눠진다.<br />
<br /><br />
<div class="txc-textbox" style="border-top-style: double; border-right-style: double; border-bottom-style: double; border-left-style: double; border-top-width: 3px; border-right-width: 3px; border-bottom-width: 3px; border-left-width: 3px; border-top-color: rgb(193, 193, 193); border-right-color: rgb(193, 193, 193); border-bottom-color: rgb(193, 193, 193); border-left-color: rgb(193, 193, 193); background-color: rgb(238, 238, 238); padding-top: 10px; padding-right: 10px; padding-bottom: 10px; padding-left: 10px; ">
<p style="margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; "><b>1. App의 Apple ID 만들기</b><br />
- 앱도 고유의 ID를 갖게된다. 그리고 당신은 애플에게 "나 이런 앱을 만들 예정이다."라고 통보할 수 있다. 적어도 App Name을 선점하는 효과가 있다. &nbsp;<br />
<br /><b>2. Metadata등 앱 정보 입력하기</b><br />
- 앱에 대해 입력해야하는 정보가 참 많다. 이 부분은 다음 단계 직전까지, 혹은 일부항목은 앱을 판매중에도 언제든지 수정이 가능하다.&nbsp;<br />
<br /><b>3. Binary File 올리기&nbsp;</b><br />
- 열심히 개발해서 만든 Binary file을 애플 쪽에 심사를 요청하는 것이다.&nbsp;</p>
</div></span><br />
<br />
<br />
이 포스팅은 1번, 당신이 만든 App에게 Apple ID를 만드는 과정을 중심으로 설명할 것이다. 그리고 이 과정은 짧게는 10분이면 가능하겠지만, 대부분의 개발자, 개발사들은 이 과정이 꽤나 오래걸리게 된다. 왜냐면 앱을 만들면서 이것 저것 수정할 것들이 생기기 때문이다.&nbsp;<br />
<br />
그리고 In-App Purchases 등을 정상적으로 테스트하기 위해서는 이 과정을 미리 밟아놔야 한다. 그래야 In-App Purchases Item도 등록할 수 있기 때문이다.&nbsp;<br />
<br />
나는 당신이 앱을 만드는 프로덕트 매니저라도 생각하고 앱을 등록하는 과정을 설명하려고 한다. 1번 과정 중심이며, 사실 1번이 전부이기도 하다.&nbsp;<br />
<br />
<br /><br />
<br /><br />
<div class="txc-textbox" style="border-top-style: double; border-right-style: double; border-bottom-style: double; border-left-style: double; border-top-width: 3px; border-right-width: 3px; border-bottom-width: 3px; border-left-width: 3px; border-top-color: rgb(193, 193, 193); border-right-color: rgb(193, 193, 193); border-bottom-color: rgb(193, 193, 193); border-left-color: rgb(193, 193, 193); background-color: rgb(238, 238, 238); padding-top: 10px; padding-right: 10px; padding-bottom: 10px; padding-left: 10px; ">
<p style="margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; "></p><div style="text-align: center; ">
<b><span style="font-size: 14pt; ">&lt;Brief&gt;</span><br />
&nbsp;</b></div>
당신의 1번 과정을 밟기 위해 필요한 최소한의 것들&nbsp;<br />
- App의 Bundle ID (Provisioning Portal에서 확인하라 or 개발자에게 물어보라)<br />
- iTunes Art : 앱스토어에 노출될 아이콘 이미지 (512x512)<br />
- Screenshot : 당신의 앱의 스크린캡쳐 이미지 (아이폰/아이패드 해상도와 동일해야 함)<br />
<br />최소한 위의 3가지가 있어야 App을 애플 측에 "신고"할 수 있다.&nbsp;<br />
iTunes Art나 Screenshot이 없다면, 사이즈만 맞춰서라도 업로드시키면 된다.&nbsp;<br />
<br /><br />
<br /><br />
자, 이제 아래는 하나하나 차근차근 앱을 등록해나가는 과정이니, 모르는 것 혹은 준비되지 않은 것은 Skip하거나 우선은 임시로 입력하면서 진행해 나가길 바란다. Good Luck to You.<p></p>
</div><br />
<br />
<br />
<br />
<span style="font-size: 11pt; ">
&nbsp;</span></span></span><br />
<br />
<span style="font-size: 11pt; "><span style="font-size: 11pt; "><b><span style="font-size: 11pt; ">1. 아이튠즈 커넥트에 접속한다.</span></b></span></span><br />
<span style="font-size: 11pt; "><span style="font-size: 11pt; "><span style="font-size: 11pt; ">- https://itunesconnect.apple.com/WebObjects/iTunesConnect.woa </span></span></span><br />
<br />
<span style="font-size: 11pt; "><span style="font-size: 11pt; "><b><span style="font-size: 11pt; ">2. 로그인한다. </span></b></span></span><br />
<span style="font-size: 11pt; "><span style="font-size: 11pt; "><span style="font-size: 11pt; ">- 각자 아이디로 로그인 합니다.&nbsp;</span></span></span><br />
<br />
<span style="font-size: 11pt; "><span style="font-size: 11pt; "><b><span style="font-size: 11pt; ">3. [Manage Your Applications] 클릭&nbsp;</span></b></span></span><br />
<span style="font-size: 11pt; "><span style="font-size: 11pt; "><span style="font-size: 11pt; ">- &nbsp;이미지 참고&nbsp;</span></span></span><br />
<br />
<p style="margin:0"><span style="font-size: 11pt; "></span></p><p style="text-align: center;"><span class="imageblock" style="display:inline-block;width:500px;"><img src="http://cfile4.uf.tistory.com/image/1814C3384DBE982531FF94" style="cursor: pointer;" onclick="open_img('http://cfile4.uf.tistory.com/original/1814C3384DBE982531FF94')"  height="467" width="500" /></span></p><p></p>
<span style="font-size: 11pt; "><span style="font-size: 11pt; "><span style="font-size: 11pt; ">&nbsp;</span></span></span><br />
<span style="font-size: 11pt; "><span style="font-size: 11pt; "><b><span style="font-size: 11pt; ">4. &lt;Manage Your Apps&gt;에서 [Add New App] 클릭</span></b></span></span><br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<span style="font-size: 11pt; "><span style="font-size: 11pt; "><b><span style="font-size: 11pt; ">5. &lt;App Information&gt;에서 아래의 3가지 항목 입력</span></b></span></span><br />
<br />
<p style="margin:0">/p>
<p style="margin:0"></p><p style="text-align: center;"><span class="imageblock" style="display:inline-block;width:500px;"><img src="http://cfile25.uf.tistory.com/image/116D94474DBEA6AB1D83D1"  height="221" width="500"/></span></p><p></p>
<br />
<p></p>
<div class="txc-textbox" style="border-top-style: double; border-right-style: double; border-bottom-style: double; border-left-style: double; border-top-width: 3px; border-right-width: 3px; border-bottom-width: 3px; border-left-width: 3px; border-top-color: rgb(203, 203, 203); border-right-color: rgb(203, 203, 203); border-bottom-color: rgb(203, 203, 203); border-left-color: rgb(203, 203, 203); background-color: rgb(255, 255, 255); padding-top: 10px; padding-right: 10px; padding-bottom: 10px; padding-left: 10px; ">
<p style="margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; "><br />
<span style="font-size: 11pt; "><b><span style="font-size: 11pt; ">1) App Name</span></b></span><br />
<br />
<span style="font-size: 11pt; "> [Q] App Name이 무엇인가? </span> <br />

<span style="font-size: 11pt; "><span style="font-size: 11pt; ">[A] 앱의 정식이름이다. iTunes 스토어에서 노출되는 이름이다.&nbsp;</span></span><span style="font-size: 11pt; "><span style="font-size: 11pt; ">&nbsp;</span></span><br />
<br /><span style="font-size: 11pt; "><span style="font-size: 11pt; ">[Q]&nbsp;</span></span><span style="font-size: 11pt; "><span style="font-size: 11pt; ">iPhone이나 iPad의 Home Screen에서 아이콘 밑에 보이는 앱이름(Bundle Display Name)인가?</span></span><br />
<span style="font-size: 11pt; "><span style="font-size: 11pt; ">[A] 아니다. Home Screen에 노출되는 이름은 심사시 업로드하는 바이너리 파일 안에서 Bundle Display Name이라는 항목으로 심어놔야 한다.&nbsp;</span></span><br />
<br /><span style="font-size: 11pt; "><span style="font-size: 11pt; ">[Q] App Name과 Bundle Display Name이 동일해야 하는가?&nbsp;</span></span><br />
<span style="font-size: 11pt; "><span style="font-size: 11pt; ">[A] 그렇지 않다.&nbsp;</span></span><br />
<br /><span style="font-size: 11pt; "><span style="font-size: 11pt; ">[Q] App Name은 한번 입력하면 수정이 불가능한가?</span></span><br />
<span style="font-size: 11pt; "><span style="font-size: 11pt; ">[A] 수정가능하다. 단, 앱을 심사받기 전에만 가능하다. 지금 밟고있는 절차인 &lt;Add New App&gt;과정은 &lt;App Information&gt;을 입력하는 첫 단계부터, 당신이 개발을 완료한 Binary File을 애플에 제출하는 단계까지 몇 단계로 나눠지며, 애플이 당신의 앱을 심사하는 In Review 전까지는 수정할 수 있다.&nbsp;</span></span><br />
<br /><span style="font-size: 11pt; "><span style="font-size: 11pt; ">[Q] 한번 심사받은 App이름은 절대 수정불가능한가?</span></span><br />
<span style="font-size: 11pt; "><span style="font-size: 11pt; ">[A] 가능하다. 단, App의 버전을 업데이트할 때만 가능하다. Waiting For Review 이전상태에서는 &lt;Version Information&gt; 항목 옆에 Edit버튼이 노출된다. 이 버튼을 클릭하면 App Name을 수정할 수 있다.</span></span><br />
<br /><span style="font-size: 11pt; "><span style="font-size: 11pt; ">[Q] 그럼 지금 당장은 App Name을 대충 입력해도 된다는 말인가?</span></span><br />
<span style="font-size: 11pt; "><span style="font-size: 11pt; ">[A] 정확히 그렇다. 너무 걱정하지 마라. 앞으로도 많은 단계가 남았다. 대충 입력해도 된다. 단, 다른 App과 이름이 같아서는 안된다.&nbsp;</span></span><br />
<br /><span style="font-size: 11pt; "><span style="font-size: 11pt; ">[Q] App 이름을 한글로 입력해야 하나? 영어로 입력해야 하나?</span></span><br /><span id="callbacknestwwwwriterkimpekr11327421" style="width:1px; height:1px; float:right"><embed  allowscriptaccess="always"  id="bootstrapperwwwwriterkimpekr11327421"  src="http://www.writerkim.pe.kr/plugin/CallBack_bootstrapperSrc?nil_profile=tistory&amp;nil_type=copied_post"  width="1"  height="1"  wmode="transparent"  type="application/x-shockwave-flash"  EnableContextMenu="false"  FlashVars="&amp;callbackId=wwwwriterkimpekr11327421&amp;host=http://www.writerkim.pe.kr&amp;embedCodeSrc=http%3A%2F%2Fwww.writerkim.pe.kr%2Fplugin%2FCallBack_bootstrapper%3F%26src%3Dhttp%3A%2F%2Fs1.daumcdn.net%2Fcfs.tistory%2Fv%2F0%2Fblog%2Fplugins%2FCallBack%2Fcallback%26id%3D1132%26callbackId%3Dwwwwriterkimpekr11327421%26destDocId%3Dcallbacknestwwwwriterkimpekr11327421%26host%3Dhttp%3A%2F%2Fwww.writerkim.pe.kr%26float%3Dleft" swLiveConnect="true"/></span>
<span style="font-size: 11pt; "><span style="font-size: 11pt; ">[A] App Name은 전세계 앱스토어에 "기본적으로는" 공통으로 노출된다. 단, 애플이 제공하는 Localization 기능을 통해서 각 언어별로 App Name을 다르게 노출되게 할 수 있다. Localization은 나중 단계에서 설정할 수 있다.)</span></span><br />
<br /><span style="font-size: 11pt; "><span style="font-size: 11pt; ">ex) Talking Santa의 경우 미국 앱스토어에서는 "Talking Santa"라고 App Name이 노출되나, 한국 앱스토어에서는 "말하는 산타 - Talking Santa"라는 App Name으로 노출된다.&nbsp;</span></span><br />
<br /><br />
<br /><span style="font-size: 11pt; "><b><span style="font-size: 11pt; ">2) SKU Number&nbsp;</span></b></span><br />
<br /><span style="font-size: 11pt; "><span style="font-size: 11pt; ">[Q] SKU Number는 숫자로만 입력해야 한다고 하는데 법칙이 있는가?</span></span><br />
<span style="font-size: 11pt; "><span style="font-size: 11pt; ">[A] 당신이 올리는 앱을 다른 앱과 구분지어줄 수 있는 숫자 구분이다. 2자리 수 이상이면 된다.&nbsp;</span></span><br />
<br /><br />
<br /><span style="font-size: 11pt; "><b><span style="font-size: 11pt; ">3) Bundle ID&nbsp;</span></b></span><br />
<br /><span style="font-size: 11pt; "><span style="font-size: 11pt; ">[Q] 콤보박스 중에서 선택하면 되는가?</span></span><br />
<span style="font-size: 11pt; "><span style="font-size: 11pt; ">[A] 그렇다. iOS Provisioning Portal에서 당신이 앱을 처음 개발할 &lt;App ID&gt;에서 생성했던 Bundle ID를 콤보박스에서 선택하면 된다. 단, Bundle ID를 한번 사용하면 수정할 수 없다.&nbsp;</span></span></p>
</div><br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<p style="margin:0"></p><p style="text-align: center;"><span class="imageblock" style="display:inline-block;width:683px;"><img src="http://cfile29.uf.tistory.com/image/2046EB4F4DBEA68B31CB2E" style="cursor: pointer;" onclick="open_img('http://cfile29.uf.tistory.com/original/2046EB4F4DBEA68B31CB2E')"  height="323" width="683" /></span></p><p></p>
<br />
<br />
<span style="font-size: 11pt; "><b><span style="font-size: 11pt; ">6. &lt;App등록테스트&gt;라는 이름 영역에는 당신이 입력한 App Name이 들어가 있을 것이다. 내가 등록하고 있는 App Name이 "App등록테스트"이니 싱기해하지 말자 ;;;</span></b></span><br />
<br />
<div class="txc-textbox" style="border-top-style: double; border-right-style: double; border-bottom-style: double; border-left-style: double; border-top-width: 3px; border-right-width: 3px; border-bottom-width: 3px; border-left-width: 3px; border-top-color: rgb(203, 203, 203); border-right-color: rgb(203, 203, 203); border-bottom-color: rgb(203, 203, 203); border-left-color: rgb(203, 203, 203); background-color: rgb(255, 255, 255); padding-top: 10px; padding-right: 10px; padding-bottom: 10px; padding-left: 10px; "><p style="margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; "><br />
<span style="font-size: 11pt; "><b><span style="font-size: 11pt; ">1) Availability Date</span></b><br />
<br /><span style="font-size: 11pt; ">[Q] A.D는 무엇인가?</span><br />
<span style="font-size: 11pt; ">[A] App 판매를 개시하고 싶은 날짜이다.</span><br />
<br /><span style="font-size: 11pt; ">[Q] 가장 빨리 팔고 싶으면 언제로 맞추면 되나?&nbsp;</span><br />
<span style="font-size: 11pt; ">[A] 등록하는 날의 날짜로 해놔도 된다.</span><br />
<br /><span style="font-size: 11pt; ">[Q] 내가 지정해 놓은 날짜보다 심사가 먼저 끝나면 어떻게 되나?</span><br />
<span style="font-size: 11pt; ">[A] 지정해 놓은 날짜에 App이 풀린다.&nbsp;</span><br />
<br /><span style="font-size: 11pt; ">[Q] 앱 심사가 들어간 다음에도 Availability Date를 수정할 수 있나?</span><br />
<span style="font-size: 11pt; ">[A] 가능하다. 그러니 너무 걱정하지 말라. Waiting for Review에서도 수정할 수 있다.&nbsp;</span><br />
<br /><br />
<br /><b><span style="font-size: 11pt; ">2) Price Tier&nbsp;</span></b><br />
<br /><span style="font-size: 11pt; ">[Q] Price Tier는 무엇인가?</span><br />
<span style="font-size: 11pt; ">[A] 앱플이 정해놓은 가격단위를 선택하는 것이다. 당신의 앱은 애플이 정해놓은 가격 단위에서 선택해서 지정할 수 있다. Tier1이 $0.99이다.&nbsp;</span><br />
<br /><span style="font-size: 11pt; ">[Q] 국가마다 Tier를 다르게 할 수 있나? 한국에서는 $0.99로 미국에서는 $1.99로 팔고 싶다.</span><br />
<span style="font-size: 11pt; ">[A] 불가능하다. Tier는 전세계 앱스토어에 공통으로 적용된다. 단일 앱이 국가별로 가격을 다르게 판매할 수는 없다.&nbsp;</span><br />
<br /><span style="font-size: 11pt; ">참고로 Tier1이 한국, 미국, 중국, 캐나다 등은 $0.99이지만 일본은 115엔, 영국은 0.59파운드, 호주는 $1.19 호주달러이다. Tier의 단위가 국가마다 다르니 글로벌 앱을 등록시에는 인지하고 있으면 좋다.</span><br />
<br /><span style="font-size: 11pt; ">[Q] 가격은 수정이 가능한가?</span><br />
<span style="font-size: 11pt; ">[A] 언제든지 가능하다. 심사 전에도, 심사 중에도, 심사 후에도, 판매 중에도 언제든지 가능하다.</span><br />
<br /><span style="font-size: 11pt; ">[Q] iTunes Connect에서 가격을 수정하면 앱스토어에서 바로 적용되나?</span><br />
<span style="font-size: 11pt; ">[A] 일반적으로 약 2~3시간 정도 후에 적용된다.</span><br />
<br /><span style="font-size: 11pt; ">[Q] Tier를 무료로 바꿀 수도 있나?</span><br />
<span style="font-size: 11pt; ">[A] 가능하다. 그런데 알고 있어야하는 것은 Paid App과 Free App은 랭킹을 구분짓고 있다. 당신이 오늘 당신의 App을 Paid App에서 Free App으로 변경하여 얻은 다운로드 수(랭킹에 반영된다)는 내일 다시 Free App에서 Paid App으로 변경할 경우, 무용지물이 된다.&nbsp;</span><br />
<br /><br />
<b><span style="font-size: 11pt; ">3) Discount for Educational Institutions</span></b><br />
<br /><span style="font-size: 11pt; ">[Q] 이건 뭔가?</span><br />
<span style="font-size: 11pt; ">[A] 애플이 교육기간의 앱스토어로 당신의 앱을 구매할 경우 할인해 것이냐고 물어보는 것이다. 대한민국을 대상으로 앱을 개발 중이라면 고민할 여지는 없을 것 같다.&nbsp;</span><br />
<br /><br />
<b><span style="font-size: 11pt; ">4) Specific Store&nbsp;</span></b><br />
<br /><span style="font-size: 11pt; ">[Q] 이건 뭔가?</span><br />
<span style="font-size: 11pt; ">[A] 전 세계 앱스토어가 아닌 특정 국가의 앱스토어에서만 판매하고 싶을 때 클릭한다.&nbsp;</span><br />
<br /><span style="font-size: 11pt; ">ex) 저작권 문제가 있어 한국 앱스토어에서만 판매하고 싶다. Specific Store를 클릭하여 한국앱스토어만 체크하면 된다.&nbsp;</span><br />
<br /></span></p>
</div><br />
<span style="font-size: 11pt; ">
<br />
<br />
<br />
<br />
<p style="margin:0"></p><p style="text-align: center;"><span class="imageblock" style="display:inline-block;width:500px;"><img src="http://cfile4.uf.tistory.com/image/1143FA4B4DBEACD537066C"  height="387" width="500"/></span></p></span><p></p>
<br />
<br />
<span style="font-size: 11pt; ">
7. 계속해서 &lt;Metadata&gt;와 &lt;Rating&gt;과 &lt;EULA&gt;, 그리고 스크린샷&lt;Uploads&gt;과정이 남아있다.&nbsp;</span><br />
<span style="font-size: 11pt; ">
아직 안도의 한숨을 내쉬어서는 안된다. 이 페이지 하단의 [Save]버튼을 누르기 전까지는 이 App은 아직 Apple 쪽에 등록되지도 않는다.&nbsp;<br />
<br />&nbsp;</span><br />
<div class="txc-textbox" style="border-top-style: double; border-right-style: double; border-bottom-style: double; border-left-style: double; border-top-width: 3px; border-right-width: 3px; border-bottom-width: 3px; border-left-width: 3px; border-top-color: rgb(203, 203, 203); border-right-color: rgb(203, 203, 203); border-bottom-color: rgb(203, 203, 203); border-left-color: rgb(203, 203, 203); background-color: rgb(255, 255, 255); padding-top: 10px; padding-right: 10px; padding-bottom: 10px; padding-left: 10px; "><p style="margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; "><br />
<span style="font-size: 11pt; ">7.1 Metadata</span><br />
<br /><span style="font-size: 11pt; ">1) Version Number&nbsp;</span><br />
<span style="font-size: 11pt; ">- 첫 앱이라면 1.0 이나, 1.0.0 이런 식으로 넣으면 된다. 바이너리 파일 안에도 Version Number를 넣어야 하는데, 두 숫자가 동일해야 한다.&nbsp;</span><br />
<br /><span style="font-size: 11pt; ">2) Description</span><br />
<span style="font-size: 11pt; ">- 앱에 대한 소개를 입력한다.&nbsp;</span><br />
<br /><span style="font-size: 11pt; ">[Q] Description은 수정이 가능한가?</span><br />
<span style="font-size: 11pt; ">[A] 가능하다. 언제든 가능하다. 심사 전에도, 심사중에도, 판매중에도... 그러니 전혀 걱정하지 말라. 그렇다고 앱심사를 신청할 때 Description을 지나치게 빈약하게 혹은 장난으로 작성하면 리젝 당할 수도 있다.&nbsp;</span><br />
<br /><span style="font-size: 11pt; ">[Q] Description는 어디에서 노출되나?</span><br />
<span style="font-size: 11pt; ">[A] iPhone, iPad의 앱스토어를 비롯해, iTunes의 App Store의 App 정보페이지에 노출된다.&nbsp;</span><br />
<br /><span style="font-size: 11pt; ">[Q] Description을 수정하면 즉시 앱스토어에 반영되나?</span><br />
<span style="font-size: 11pt; ">[A] 그렇지 않다. 약 2~3시간 뒤에 반영된다.&nbsp;</span><br />
<br /><br />
<span style="font-size: 11pt; ">3) Category&nbsp;</span><br />
<span style="font-size: 11pt; ">- 앱의 카테고리를 선택한다.&nbsp;</span><br />
<br /><span style="font-size: 11pt; ">[Q] Category는 수정이 가능한가?&nbsp;</span><br />
<span style="font-size: 11pt; ">[A] 심사 전까지는 수정이 가능하다. 그러니 지금 당장은 선택하지 못 해서 앱등록을 포기할 필요는 없다. 단, In Review 단계부터는 수정이 불가능하다.&nbsp;</span><br />
<br /><span style="font-size: 11pt; ">[Q] 심사받은 이후에는 Category 수정이 불가능한가?</span><br />
<span style="font-size: 11pt; ">[A] 가능하다. 단, 새로운 버전의 앱을 업데이트할 때만 가능하다. 그러니 어느 카테고리에서 경쟁할 것인지를 심사숙고하여 선택해야 한다. 물론 앱의 성격과 맞지 않는 카테고리를 선택하면 리젝사유가 된다고 한다.</span><br />
<br /><br />
<span style="font-size: 11pt; ">4) Keyword&nbsp;</span><br />
<span style="font-size: 11pt; ">- 앱스토어에서 사용자들이 키워드 검색으로 당신의 앱을 찾을 수 있도록 등록하면 된다. 100byte까지 등록이 가능하다.</span><br />
<br /><span style="font-size: 11pt; ">[Q] 키워드 간에는 콤마로 구분하나? 콤마 다음에 공란을 줘야하나?</span><br />
<span style="font-size: 11pt; ">[A] 콤마로 구분한다. 콤마 다음에 스페이스바를 눌러 공란을 주면 100byte를 금방 다 쓰게 된다. 그러니 콤마 다음에 스페이스를 누르지 않아도 된다.</span><br />
<br /><span style="font-size: 11pt; ">[Q] 키워드는 언제든지 수정이 가능한가?</span><br />
<span style="font-size: 11pt; ">[A] 그렇지 않다. App Name, Category와 Keyword는 버전 업데이트시에만 가능한 항목이니 유념하도록 하자.</span><br />
<br /><br />
<span style="font-size: 11pt; ">5) Contact Email Address</span><br />
<span style="font-size: 11pt; ">- 이건 당신의 이메일 주소를 입력해주면 된다. 사용자들에게 노출되는 이메일이 아니다. Apple이 심사중에 문제가 생기면 연락하는 이메일 채널이다.&nbsp;언제든지 수정이 가능하다.&nbsp;</span><br />
</p></div>
<br />
<br />
<br />
<br />
<br />
<p style="margin:0"></p><p style="text-align: center;"><span class="imageblock" style="display:inline-block;width:500px;"><img src="http://cfile7.uf.tistory.com/image/142067434DBF7A963AB7AF"  height="245" width="500"/></span></p><p></p>
<div style="text-align: center;">
<span style="font-size: 11pt; ">&lt;웹사이트: 8. &nbsp;| 지원: 6. &gt;&nbsp;</span></div>
<br />
<br />
<div class="txc-textbox" style="border-top-style: double; border-right-style: double; border-bottom-style: double; border-left-style: double; border-top-width: 3px; border-right-width: 3px; border-bottom-width: 3px; border-left-width: 3px; border-top-color: rgb(203, 203, 203); border-right-color: rgb(203, 203, 203); border-bottom-color: rgb(203, 203, 203); border-left-color: rgb(203, 203, 203); background-color: rgb(255, 255, 255); padding-top: 10px; padding-right: 10px; padding-bottom: 10px; padding-left: 10px; "><p style="margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; "><br />
<span style="font-size: 11pt; ">6) Support URL&nbsp;</span><br />
<span style="font-size: 11pt; ">- 이건 App Store에서 App소개 페이지에서 사용자들이 클릭으로 링크를 타고 들어갈 수 있는 링크이다. 홈페이지나 블로그 등으로 연결해두면 된다. 역시 언제든지 수정이 가능하다. 반드시 링크를 입력해야 하고 위에 첨부된 이미지 중에 [OO앱이름OO 지원]이라는 버튼에 링크가 걸린다.</span><br />
<br /><span style="font-size: 11pt; ">7) App URL&nbsp;</span><br />
<span style="font-size: 11pt; ">- 선택사항이며, 위에 첨부된 이미지 중에 [OO개발자OO 웹 사이트]라는 버튼에 링크가 걸린다.&nbsp;</span><br />
<br /><span style="font-size: 11pt; ">8) Privacy Policy URL&nbsp;</span><br />
<span style="font-size: 11pt; ">- 선택사항이다.</span><br />
<br /><span style="font-size: 11pt; ">9) Review Notes&nbsp;</span><br />
<span style="font-size: 11pt; ">- 역시 선택사항이다. 한 가지 주의해야 하는 것은 앱 내에 회원가입 이나 로그인 기능이 포함되어있는 앱의 경우는 이 공란에 ID와 PW를 입력해줘야 한다. ID/PW를 깜빡하고 입력하지 않았다가 10일 기다렸다가 리젝통보받고 나면 후회가 막심할 수 있다. 빠뜨리지 말자.</span><br />
<br /></p>
</div><br />
<br />
<br />
<br />
<p style="margin:0"></p><p style="text-align: center;"><span class="imageblock" style="display:inline-block;width:500px;"><img src="http://cfile3.uf.tistory.com/image/170357494DBF9633234859"  height="389" width="500"/></span></p><p></p>
<br />
<br />
<div class="txc-textbox" style="border-top-style: double; border-right-style: double; border-bottom-style: double; border-left-style: double; border-top-width: 3px; border-right-width: 3px; border-bottom-width: 3px; border-left-width: 3px; border-top-color: rgb(203, 203, 203); border-right-color: rgb(203, 203, 203); border-bottom-color: rgb(203, 203, 203); border-left-color: rgb(203, 203, 203); background-color: rgb(255, 255, 255); padding-top: 10px; padding-right: 10px; padding-bottom: 10px; padding-left: 10px; "><p style="margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; "><br />
<span style="font-size: 11pt; ">8. 다음은 Rating이다.&nbsp;</span><br />
<span style="font-size: 11pt; ">- +4 / +9 / +12 / +17 &nbsp;다음과 같은 레벨이 있다. 여기서 체크를 잘 못 했다고 앱을 리젝시키는 경우는 없는 것 같다. 단 +17의 앱의 경우는 사용자가 다운로드나 업데이트할 때 경고창이 한번 더 뜨게 된다.</span><br />
<br /><br />
<span style="font-size: 11pt; ">9. EULA</span><br />
<span style="font-size: 11pt; ">- End User License Agreement의 약자이며, 애플은 당신의 앱을 중계하여 판매하는 입장이라, 앱개발사가 앱구매자(End-User)에게 계약조건을 체결하고자 할 때 이 항목을 사용하면 된다. 일반적으로 그냥 Standard EULA를 사용하면 된다. (아무 설정을 하지 않으면 Standard EULA가 적용 됨)</span></p>
</div><br />
<br />
<br />
<br />
<br />
<p style="margin:0"></p><p style="text-align: center;"><span class="imageblock" style="display:inline-block;width:500px;"><img src="http://cfile22.uf.tistory.com/image/1436583A4DBF97821FFD00"  height="177" width="500"/></span></p><p></p>
<br />
<br />
<span style="font-size: 11pt; ">10. 이제 거의 다 왔다. Upload 순서이다. &lt;iTunes Art&gt;와 &lt;스크린샷&gt;을 올리면 된다. </span><br />
<div class="txc-textbox" style="border-top-style: double; border-right-style: double; border-bottom-style: double; border-left-style: double; border-top-width: 3px; border-right-width: 3px; border-bottom-width: 3px; border-left-width: 3px; border-top-color: rgb(203, 203, 203); border-right-color: rgb(203, 203, 203); border-bottom-color: rgb(203, 203, 203); border-left-color: rgb(203, 203, 203); background-color: rgb(255, 255, 255); padding-top: 10px; padding-right: 10px; padding-bottom: 10px; padding-left: 10px; "><p style="margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; "><br />
<span style="font-size: 11pt; ">1) iTunes Art (Large Icon)</span><br />
<br /><span style="font-size: 11pt; ">[Q] iTunes Art는 무엇인가?&nbsp;</span><br />
<span style="font-size: 11pt; ">[A]앱스토어 내에서 노출될 앱의 아이콘이다. 512x512 사이즈이다.</span><br />
<br /><span style="font-size: 11pt; ">[Q] 아이폰과 아이패드 홈스크린에서 보여지는 아이콘이 이 이미지인가?</span><br />
<span style="font-size: 11pt; ">[A] 아니다. 앱스토어에서 노출되는 이미지이다. 홈스크린, 스포트라이트(검색) 용 아이콘은 바이너리 파일 안에 담겨있는 이미지를 사용하게 된다.</span><br />
<br /><span style="font-size: 11pt; ">[Q] iTunes Art를 올렸더니 모퉁이가 round 처리되고 반사광도 생긴다. 없앨 수 없나?</span><br />
<span style="font-size: 11pt; ">[A] 그건 애플이 자동으로 그렇게 만들어서 미리보기 해주는 것이다. 앱스토어에 노출 될 때는 반사광이 사라진다. 모퉁이는 라운드처리 돼서 노출된다.</span><br />
<br /><span style="font-size: 11pt; ">[Q] 네 모퉁이를 라운드처리한 이미지를 올려도 되나?</span><br />
<span style="font-size: 11pt; ">[A] 가이드에 따르면 라운드 처리하지 않은 이미지를 올리라고 나온다.&nbsp;</span><br />
<br /><span style="font-size: 11pt; ">[Q] 한 번 올린 iTunes Art 이미지를 교체할 수 있나?</span><br />
<span style="font-size: 11pt; ">[A] 가능하다. 단 심사전까지 가능하며 심사 이후에는 변경이 불가하다. 단, 업데이트 시에는 App&nbsp;</span><br />
<span style="font-size: 11pt; ">Name을 변경할 수 있듯이, iTunes Art(Large Icon)도 변경이 가능하다.</span><br />
<br /><br />
<span style="font-size: 11pt; ">2) Screen Shot&nbsp;</span><br />
<span style="font-size: 11pt; ">- 당신의 앱의 구동장면을 스크린 캡쳐 하여 올리면 된다.&nbsp;</span><br />
<br /><span style="font-size: 11pt; ">[Q] 반드시 스크린캡쳐 이미지어야 하나?</span><br />
<span style="font-size: 11pt; ">[A] 그렇진 않다. 아래와 같이 사용예에 맞는 이미지를 올리는 것도 효과적인 홍보방법이 된다.</span><br />
<span style="font-size: 11pt; ">단, 사이즈와 파일포맷은 정해져있으니 jpg나 png, tif 파일로 아이폰용 이미지는 480x320 으로 iPad는 1024x768에 맞춰서 올리면 된다.&nbsp;</span></p>
</div><br />
<br />
<p style="margin:0"></p><p style="text-align: center;"><span class="imageblock" style="display:inline-block;width:683px;"><img src="http://cfile24.uf.tistory.com/image/175860334DBF9B2514A88A" style="cursor: pointer;" onclick="open_img('http://cfile24.uf.tistory.com/original/175860334DBF9B2514A88A')"  height="310" width="683" /></span></p><p></p>
<br />
<div class="txc-textbox" style="border-top-style: double; border-right-style: double; border-bottom-style: double; border-left-style: double; border-top-width: 3px; border-right-width: 3px; border-bottom-width: 3px; border-left-width: 3px; border-top-color: rgb(203, 203, 203); border-right-color: rgb(203, 203, 203); border-bottom-color: rgb(203, 203, 203); border-left-color: rgb(203, 203, 203); background-color: rgb(255, 255, 255); padding-top: 10px; padding-right: 10px; padding-bottom: 10px; padding-left: 10px; "><p style="margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; "><br />
<span style="font-size: 11pt; ">[Q] 480x320으로 올리면 Retina Display에서 흐려보이진 않나?&nbsp;</span><br />
<span style="font-size: 11pt; ">[A] 그렇지 않다. 애플이 알아서 리사이즈해서 절반크기로 줄여서 보여준다.&nbsp;</span><br />
<br /><span style="font-size: 11pt; ">[Q] 왜 iPhone과 iPad 둘 다 올리게 해놨나?</span><br />
<span style="font-size: 11pt; ">[A] Universal 앱을 배려한 구조이다. iPad앱이면 iPad에만 올리고, iPhone앱이면 iPhone에만 올리면 된다.&nbsp;</span><br />
<br /><span style="font-size: 11pt; ">[Q] 스크린샷 이미지를 교체할 수도 있나?</span><br />
<span style="font-size: 11pt; ">[A] 가능하다. 심사전에도 심사 후에도, 판매중에도 교체할 수 있다. 단, 판매중에 스크린샷을 이미지를 교체하면 즉각 반영되지 않을 수 있다. 스크린샷 이미지 5개 중에 한개를 삭제하고, 다른 이미지 한개를 추가했는데, 삭제는 3시간 뒤에 반영되었으나, 추가는 5일 뒤에 반영된 적이 있다.&nbsp;</span><br />
<br /><span style="font-size: 11pt; ">&nbsp;</span></p>
</div><br />

<br />
<br />
<br />
<br />
<br />
<div style="text-align: center;">
<span style="font-size: 18pt; "><span style="font-size: 11pt; "><span style="font-size: 18pt; ">자 이제 </span></span><font color="#193da9"><span style="font-size: 11pt; "><span style="font-size: 18pt; ">[Save]</span></span></font><span style="font-size: 11pt; "><span style="font-size: 18pt; ">버튼을 클릭하자.</span>&nbsp;</span></span></div>
<div style="text-align: center;">
<br />
</div>
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<span style="font-size: 11pt; ">자 이제, &nbsp;당신의 앱은 애플에 등록되었고, Manage Your App 메뉴에서도 살펴볼 수 있게 되었다. Manage Your App에서 방금 등록한 앱을 클릭하면 아래와 같은 앱 관리 화면을 볼 수 있다.&nbsp;</span><br />
<br />
<br />
<br />
<p style="margin:0"></p><p style="text-align: center;"><span class="imageblock" style="display:inline-block;width:500px;"><img src="http://cfile25.uf.tistory.com/image/1106BF534DBFA03E035937"  height="355" width="500"/></span></p><p></p><p>
<br />
<br />
<br />
<span style="font-size: 11pt; ">11. [View Detail]을 클릭한다.</span><br />
<span style="font-size: 11pt; ">12. 다음 화면에서 우측 상단의 [Ready to Upload Binary]를 클릭한다.&nbsp;</span><br />
<span style="font-size: 11pt; ">13. Encryption 여부를 확인한다.&nbsp;<br />
<br />
<br />
</span></p><p style="margin:0"></p><p style="text-align: center;"><span class="imageblock" style="display:inline-block;width:500px;"><img src="http://cfile6.uf.tistory.com/image/1427263C4DBFB65C31F2AF"  height="201" width="500"/></span></p><p></p>
&nbsp;<br />
<meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
<meta http-equiv="Content-Style-Type" content="text/css">
<title></title>
<meta name="Generator" content="Cocoa HTML Writer">
<meta name="CocoaVersion" content="1038.35">
<style type="text/css">
p.p1 {margin: 0.0px 0.0px 0.0px 0.0px; font: 14.0px 'Lucida Grande'}
</style><p>


<span style="font-family: 'Lucida Grande'; font-size: 14px; line-height: normal; ">- Does your product contain encryption or does it use or access encryption from another source, e.g., iOS or Mac OS X?<br />
<br />
&nbsp;- 앱안에 로그인 이나 인증기능이 포함된 경우는 YES를 선택한다. 없으면 NO하면 된다. &nbsp;NO 다음에는 [SAVE] 버튼을 누르면 된다.&nbsp;<br />
<br />
<br />
<br />
- YES인 경우에는 아래의 체크박스를 한번 더 확인해줘야 한다.<br />
<br />
</span></p><p style="margin:0"></p><p style="text-align: center;"><span class="imageblock" style="display:inline-block;width:500px;"><img src="http://cfile2.uf.tistory.com/image/1372223A4DBFB6E6331BD9"  height="227" width="500"/></span></p><p></p>
<br />
<br />
- 단순 인증이나 바이러스 보호 목적 이외의 encryption을 사용한다면 yes를 클릭하라고 한다. 보통은 인증 수준일테니 NO를 클릭하고 [SAVE]버튼을 클릭하면 된다.&nbsp;<br />
<br />
<br />
<br />
<br />
<div style="text-align: center;">
<span style="font-size: 18pt; ">이제 앱의 상태는 <font color="#193da9">&lt;Waiting for Upload&gt;</font>가 된다.</span></div>
<br />
<br />
<br />
<br />
<br />
자, 이제 개발자가 Uploader 프로그램을 이용해서 Binary File을 업로드 시키면 된다.&nbsp;<br />
파일을 업로드하고나면 다음 상태는 &lt;Waiting for Review&gt;가 된다.&nbsp;<br />
<br />
<br />
아마 이제 당신의 몫은 다 끝났을 것이다.&nbsp;<br />
수고했다. 다음 단계는 2~4일 뒤에 In Review가 들어가고, 업무일로 5~10일 사이에 Ready for Sale이 뜰 것이다. 당신의 앱과 등록과정에 별문제가 없다면 말이다. : )&nbsp;<br />
<br />
<br /><br />
<br /><br />
<br /><br />
<br /><br />
<br />
<br />
아래는 iTunes Artwork 512px 이미지와&nbsp;<br />
iPhone용 스크린샷 이미지이다. 두 파일을 다운받아서 쓰면, 당신은 App을 만들지 않아도 App ID를 등록할 수 있게된다.&nbsp;<br />
<br />
<p style="margin:0"></p><p style="text-align: center;"><span class="imageblock" style="display:inline-block;width:512px;"><img src="http://cfile29.uf.tistory.com/image/18581E334EFDA6A9205A23"  height="512" width="512"/></span></p><p></p>
<p style="margin:0"></p><p style="text-align: center;"><span class="imageblock" style="display:inline-block;width:320px;"><img src="http://cfile4.uf.tistory.com/image/17581E334EFDA6AA219376"  height="480" width="320"/></span></p><p></p>
<br />
<br />
<br />
<br />
<br />
<br /><span style="font-size: 12pt; ">그외에 In App Purchase 에 관한 관련글&nbsp;</span><p></p><h3 class="tit" style="margin-top: 0px; margin-right: 10px; margin-bottom: 12px; padding-top: 1px; padding-right: 0px; padding-bottom: 0px; padding-left: 9px; font: normal normal normal 12px/1.5 돋움, dotum, Tahoma, AppleGothic, sans-serif; color: rgb(99, 99, 99); overflow-x: hidden; overflow-y: hidden; width: 680px; letter-spacing: -1px; "><span style="color: rgb(99, 99, 99); padding-top: 0px; padding-right: 0px; padding-bottom: 0px; padding-left: 0px; line-height: 1.2em; font-family: inherit; font-size: 14pt; "><span style="color: rgb(107, 102, 255); font-size: 12pt; ">1.&nbsp;</span><a href="http://writerkim.pe.kr/1650" class="tx-link" style="color: rgb(99, 99, 99); padding-top: 0px; padding-right: 0px; padding-bottom: 0px; padding-left: 0px; font-size: 24px; line-height: 1.2em; font-family: inherit; " target="_blank"><span style="color: rgb(107, 102, 255); font-size: 12pt; ">앱스토어 완전정복 - IAP 인앱퍼처스 돌다리도 두들겨보고 건너기</span></a></span><span style="color: rgb(107, 102, 255); font-size: 12pt; ">&nbsp;</span></h3><p></p><p><font face="'Lucida Grande'"><span style="line-height: normal; font-size: 14pt; color: rgb(0, 85, 255); "><span style="color: rgb(107, 102, 255); font-size: 12pt; ">&nbsp;<a href="http://writerkim.pe.kr/1654" target="_blank" class="tx-link">&nbsp;</a></span><a href="http://writerkim.pe.kr/1654" target="_blank" class="tx-link"><span style="color: rgb(107, 102, 255); font-size: 12pt; ">2.&nbsp;</span></a></span></font><a href="http://writerkim.pe.kr/1654" class="link" style="letter-spacing: -1px; color: rgb(99, 99, 99); padding-top: 0px; padding-right: 0px; padding-bottom: 0px; padding-left: 0px; font-size: 24px; line-height: 1.2em; font-family: inherit; "><span style="font-size: 14pt; color: rgb(0, 85, 255); "></span></a><a href="http://writerkim.pe.kr/1654" target="_blank" class="tx-link"><span style="color: rgb(107, 102, 255); font-size: 12pt; ">[아이튠즈커넥트] 가격변경 - 예약기능 사용</span></a></p><p><span style="font-size: 14pt; ">
</span>

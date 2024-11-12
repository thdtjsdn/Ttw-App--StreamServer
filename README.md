# Ttw-App--StreamServer

---

# 문의 사항

- thdtjsdn@gmail.com

---

# 1. 영상 스트리밍 서버 프로그램 다운로드 링크

- 매우 가볍고 성능 좋은 스트리밍 서버입니다.
- 개인용 동영상 스트리밍 서버입니다.
- Windows, Linux, Mac 지원
- Linux, Mac은 바이너리 권한 추가 sudo chmod 755 ./TtwServerStreamLinux 또는 Mac
- 자유롭게 사용하셔도 무방합니다.
- 개인 데이터 그 무엇도 전송 및 보관하지 않습니다(수갑 차기 싫습니다.)
- mp4, mkv 파일 지원
- 업데이트 있을시 실행파일만 다시 받아서 재구동하면 됩니다.
- 본서버는 Protocol Level에서 정의된 기능외 확장기능이 없기 때문에 보안에 안전합니다.
- (모든 기타 요청 또는 시도를 무시하고 씹어버립니다.)
- 상용 서비스 및 HTTPS를 원하시는 분들께는 유료제공 가능합니다.

---

# 2. git clone 또는 압축파일 다운로드, 압축 해제 후

- .main.js 파일 오픈 후 비디오 디렉토리 경로 지정
- .userAdmin.json 파일 오픈 후 사용자 관리 및 지정
- .user.json 파일 오픈 후 사용자 관리 및 지정
- 위 두파일 관리자 및 유저 수정 및 비밀번호 교체 필수입니다.
- 개인용도면 아무에게도 안 알려주면 됩니다.

---

# 3. 공유기에서 49154 PORT 오픈하고 서버를 구동하는 장비로 PORT 포워딩 설정을 합니다.

- 공유기 PORT 오픈과 PORT 포워딩 설정은 각 공유기 제조사이트 확인

---

# 4. 접속은 링크로 합니다.

- 본인 서버가 HTTP로 구동 되있을 경우
	- http://thdtjsdn.com:49310/app_stream_video/html_page/viewer/index.html

- 본인 서버 localhost 테스트용 https 서비스
	- https://thdtjsdn.com/app_stream_video/html_page/viewer/index.html
- 상단 Server Address 입력, Domain 또는 IP 입력 필수
- 상단 Password에 .user.json에 지정한 pw 입력

---

# 5. 최상위 서버 갱신(목록) 버튼 '클릭'

- 서버 구동 후 1회 실행 필수
- 서버 구동 장비의 지정한 비디오 폴더에 'List' 파일 생성
- 비디오 폴더의 내용을 수정/가감 했을시 클릭 해줘야 갱신됩니다.

---

# 6. 조회 버튼 클릭

- 상단 Server Address 입력, Domain 또는 IP 입력 필수
- 상단 Password에 유저별 pw 입력
- 상단 Password가 없으면 영상 재생 불가능

---

# 7. 즐거운 스트리밍 생활

---

# 8. 차후 추가될 기능

- 기타 포멧 → mp4로 변경 기능
- 원격 강제 종료
- 썸네일 생성 기능
- 설명 추가 기능
- 접속자 및 기타등등 통계
- 수려한 UI로 변경
- 실시간 라이브 스트리밍(영상 & 음성 및 음성모드)

---

# 9. 본 서버는 '무료제공' 입니다.

- 접속 하는 화면의 광고 수익으로만 유지
- 한번씩 광고 클릭해주시면 감사합니다.

---

# .main.js 가 메인 소스 시작파일입니다.

- 추후 .config.json 설정으로 변경 할수도 있습니다만, 굳이..?

- 사용 예시 소스 코드가 존재합니다.

---

# GUI 기반의 Debugger Tool이 존재합니다.

- Private Repository 입니다.

---

# API 목록(필요할 법한 목록만)

- UtilLogger.debug = function(o, g){}
- UtilLogger.error = function(o, g, l){}
- UtilLogger.log = function(o, g){}
- UtilLogger.logc = function(o, g){}
- UtilLogger.logi = function(o, g){}
- UtilLogger.logr = function(o, g){}
- UtilLogger.logy = function(o, g){}
- UtilLogger.verbose = function(o, g){}
- UtilLogger.warn = function(o, g){}
- 
- UtilDate.getNow = function(){}
- UtilDate.getNowLocaleString = function(){}
- UtilDate.getNowLocaleString__Dash = function(){}
- UtilDate.getNowLocaleString__Dash__Milliseconds = function(){}
- UtilDate.getNowLocaleString_D = function(){}
- UtilDate.getNowLocaleString_H = function(){}
- UtilDate.getNowLocaleString_HM = function(){}
- UtilDate.getNowString_D = function(){}
- 
- UtilFS.appendFile = function(r, n){}
- UtilFS.appendFile_Sync = function(t, e){}
- UtilFS.check_path = function(t){}
- UtilFS.close = function(e){}
- UtilFS.close_cb = function(t, e){}
- UtilFS.close_Sync = function(t){}
- UtilFS.createDirectory = function(t, e){}
- UtilFS.createDirectory_BefoeCheck = function(t){}
- UtilFS.deleteFile = function(t, e){}
- UtilFS.deleteAllFiles_Sync = function(t){}
- UtilFS.deleteFile_Sync = function(t){}
- UtilFS.deleteFiles_Sync__link_name = function(t, e){}
- UtilFS.getList_Directory = function(t){}
- UtilFS.getList_File = function(t){}
- UtilFS.getList_Folder = function(t){}
- UtilFS.getList_FileExtension = function(t, e){}
- UtilFS.getList_FE__css = function(t){}
- UtilFS.getList_FE__csv = function(t){}
- UtilFS.getList_FE__gz = function(t){}
- UtilFS.getList_FE__html = function(t){}
- UtilFS.getList_FE__js = function(t){}
- UtilFS.getList_FE__json = function(t){}
- UtilFS.getList_FE__mp3 = function(t){}
- UtilFS.getList_FE__tcss = function(t){}
- UtilFS.getList_FE__thtml = function(t){}
- UtilFS.getList_FE__tjs = function(t){}
- UtilFS.getList_FE__tjson = function(t){}
- UtilFS.getList_FE__ts = function(t){}
- UtilFS.getList_FE__tson = function(t){}
- UtilFS.getList_FE__tsv = function(t){}
- UtilFS.getList_FE__txml = function(t){}
- UtilFS.getList_FE__txt = function(t){}
- UtilFS.getList_FE__xml = function(t){}
- UtilFS.getList_FE__zip = function(t){}
- UtilFS.readDir_Sync = function(t){}
- UtilFS.readFile = function(r){}
- UtilFS.readFile_cb = function(t, e){}
- UtilFS.readFile_Sync = function(t){}
- UtilFS.readFile_UTF8_Sync = function(t){}
- UtilFS.readFile_UTF8_Sync__JSON = function(t){}
- UtilFS.writeFile_UTF8 = function(r, n, i){}
- UtilFS.writeFile_UTF8_Sync = function(t, e){}
- UtilFS.writeFile_UTF8_Sync__JSON = function(t, e){}
- UtilFS.writeFile_UTF8_Sync__JSON_Tab1 = function(t, e){}
- UtilFS.writeFile = function(r, n, i){}
- UtilFS.writeFile_Sync = function(t, e){}
- 
- UtilHttpNodeJS.get = function(t){}
- UtilHttpNodeJS.get_cb = function(r, o){}
- UtilHttpNodeJS.get_cb__string = function(t, i){}
- UtilHttpNodeJS.get_cb__string__utf8 = function(t, i){}
- UtilHttpNodeJS.getSync = function(r){}
- UtilHttpNodeJS.getSyncJSON = function(e){}
- UtilHttpNodeJS.post__native = function(t, n, e, r, o, i){}
- UtilHttpNodeJS.post = function(t, n, e, r){}
- 
- UtilHttpRequest.check_IP = function(e, t, r){}
- UtilHttpRequest.check_IP_N_Response = function(e, t, r){}
- 
- UtilHttpResponse.response_header_CORS = function(e, t){}
- UtilHttpResponse.response_header_common_json_utf8 = function(e, t){}
- UtilHttpResponse.response_header_common_text_utf8 = function(e, t){}
- UtilHttpResponse.response_header_contentType = function(e, t, n){}
- UtilHttpResponse.response_header_contentType__gz = function(e, t, n){}
- UtilHttpResponse.response_200 = function(e, t, n, o){}
- UtilHttpResponse.response_200__404 = function(e, t, n, o){}
- UtilHttpResponse.response_200_Boolean_False = function(e, t, n, o){}
- UtilHttpResponse.response_200_Boolean_True = function(e, t, n, o){}
- UtilHttpResponse.response_200_FileStream = function(e, t, n, o, s){}
- UtilHttpResponse.response_200_FileStream__Toss = function(e, t, n, o, s){}
- UtilHttpResponse.response_200_HTML = function(e, t, n, o){}
- UtilHttpResponse.response_200_JSON = function(e, t, n, o){}
- UtilHttpResponse.response_200_JSON__Array = function(e, t, n, o){}
- UtilHttpResponse.response_200_JSON__Error = function(e, t, n, o){}
- UtilHttpResponse.response_200_JSON__Object = function(e, t, n, o){}
- UtilHttpResponse.response_200_String = function(e, t, n, o){}
- UtilHttpResponse.response_301__google_thdtjsdncom = function(e, t, n){}
- UtilHttpResponse.response_301 = function(e, t, n, o){}
- UtilHttpResponse.response_400 = function(e, t, n, o){}
- UtilHttpResponse.response_400_JSON = function(e, t, n, o){}
- UtilHttpResponse.response_403 = function(e, t, n, o){}
- UtilHttpResponse.response_403_JSON = function(e, t, n, o){}
- UtilHttpResponse.response_404 = function(e, t, n, o){}
- UtilHttpResponse.response_404_JSON = function(e, t, n, o){}
- UtilHttpResponse.response_416 = function(e, t, n, o){}
- UtilHttpResponse.response_500 = function(e, t, n, o){}
- UtilHttpResponse.response_500_JSON = function(e, t, n, o){}
- UtilHttpResponse.response_501 = function(e, t, n, o){}
- UtilHttpResponse.response_501_JSON = function(e, t, n, o){}
- UtilHttpResponse.writeHead_response_206 = function(e, t, n, o, s, r){}
- UtilHttpResponse.writeHead_response_206__Video = function(e, t, n, o, s){}
- 
- UtilHttpsNodeJS.get = function(t){}
- UtilHttpsNodeJS.get_cb = function(o, r){}
- UtilHttpsNodeJS.get_cb__string = function(t, i){}
- UtilHttpsNodeJS.get_cb__string__utf8 = function(t, i){}
- UtilHttpsNodeJS.getSync = function(o){}
- UtilHttpsNodeJS.getSyncJSON = function(e){}
- 
- UtilObject.defineProperty__const = function(t, n, r){}
- UtilObject.defineProperty__const__if = function(t, n, r){}
- 
- UtilString.deleteNumbers = function(r){}
- UtilString.isIPAddress = function(r){}
- UtilString.isIPAddress_regexp = function(r){}
- 
- UtilStringIPAddress.getIPv4__NodeJS_Request_RemoteAddress = function(e){}
- UtilStringIPAddress.isIPAddress = function(e){}
- UtilStringIPAddress.isIPAddress_regexp = function(e){}
- 
- UtilStringPad_Number.pad_0_1 = function(t){}
- UtilStringPad_Number.pad_00_3 = function(t){}
- 
- UtilURL.getFileExtensionFromURI = function(e){}
- UtilURL.getFileExtensionFromURI_1 = function(e){}
- UtilURL.getFilePathFromURI = function(e, r){}
- UtilURL.getQueryFromURL = function(e){}
- UtilURL.getQueryFromURL_Decode = function(e){}
- UtilURL.getQueryObjectFromURL = function(e){}
- UtilURL.getQueryObjectFromURL_Decode = function(e){}
- UtilURL.getURIFromURL = function(e){}
- UtilURL.getURIFromURL_DecodeURI = function(e){}
- UtilURL.getURIFromURL_DecodeURIComponent = function(r){}

---
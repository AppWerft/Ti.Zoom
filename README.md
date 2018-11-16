# Ti.Zoom

Axway Titanium module for realizing zoom video conferencing.

![](https://d24cgw3uvb9a9h.cloudfront.net/static/92961/image/new/ZoomLogo.png)

![](https://developer.zoom.us/wp-content/uploads/2017/07/androidFlow.png)

## Usage

```javascript
const ZoomSDK = require("de.appwerft.zoom");
ZoomSDK.initialize(APP_KEY, APP_SECRET, WEB_DOMAIN);

ZoomSDK.loginWithZoom(username,password);

const opts = ZoomSDK.createMeetingOptions({
	"no_driving_mode" : true,
	"no_meeting_end_message" :true,
	"no_titlebar" : true,
	"no_bottom_toolbar" : true,
	"no_invite" : true
});

ZoomSDK.meetingService.joinMeeting(meetingNo, DISPLAY_NAME, meetingPassword, opts);

```

# IoT Platform — Timesheet

Work on the IoT monitoring platform (web, server and mobile app).

| Period | File | Hours |
|---|---|---|
| 29 Oct – 13 Nov 2026 | [2026-11.csv](2026-11.csv) | 121 |

## 29 Oct – 13 Nov 2026

| Date | Task | Details | Hours |
|---|---|---|---|
| 29 Oct | Sensor page | Added an average-value tile to the sensor page and made the sensor title larger and clearer above the gauge. | 1 |
| 29 Oct | Reports | Gaps in sensor readings now count as downtime in reports. Added Downtime and Average options to the report screen. | 3 |
| 30 Oct | Settings: sensor card design | Settings to customize the sensor card's size, text and colors, with a live preview of the result. Settings page now uses the full screen width. | 6 |
| 2 Nov | Location maps | New location maps: upload a floor plan, place live sensor boxes on it, and draw rooms, walls, doors, windows, entries, exits and stairs. Server storage and access rules per user role. | 10 |
| 3 Nov | Map editor | Map editor with autosave, undo/redo, right-click menus, and sensor box shape, size and color options. | 8 |
| 3 Nov | History Undo | Actions recorded in History can now be undone from the History page. | 4 |
| 4 Nov | Users page | Details card when hovering a user's name, and a right-click menu with the common user actions. | 3 |
| 4 Nov | Settings: test push notification | Admin can send a test push notification to a chosen user's phone to check delivery. | 2 |
| 4 Nov | Location maps | Sensor values on the map shown in their status color (OK, warning, down and so on). | 1 |
| 4 Nov | HTTP devices | Started HTTP device support: devices can send readings over HTTP instead of MQTT. | 4 |
| 5 Nov | Location maps | View on Map popup from any sensor, snap to grid in the editor, and Back returns to the page you came from. | 5 |
| 5 Nov | Settings: test SMS | Admin can send a test SMS to a chosen user to check SMS delivery. | 2 |
| 5 Nov | HTTP sensor simulator | Web-based simulator that sends device readings in the PRTG HTTP push format, for testing HTTP devices without hardware. | 4 |
| 6 Nov | HTTP devices | Finished HTTP devices: readings received on port 5055 in PRTG format alongside MQTT, offline detection when a device goes silent, and a per-owner removal timeout. | 4 |
| 6 Nov | Web and mobile app sync | Acknowledge, un-acknowledge, resolve and Clear on alerts now stay in sync between the web and the phone app, live. Users can turn their own email/SMS/push notifications on or off, synced both ways. | 8 |
| 7 Nov | Messaging | New messaging system: chats between the master admin, super admins and their users, plus announcements to selected users, groups or locations. Live delivery, push to phones, unread counts. | 10 |
| 7 Nov | Mobile app specifications | Written implementation instructions for the Android app: alert and notification sync, and location maps. | 2 |
| 8 Nov | Server stability | Investigated the repeated 504 errors (server running out of memory). Removed the memory cap and added an automatic watchdog that restarts the web server before it slows down. | 6 |
| 8 Nov | Messaging | Simplified messaging: removed the separate Issue/Service/Help screens; announcements now land in each person's chat so they can reply. | 4 |
| 9 Nov | Messaging | WhatsApp-style layout with a single new-chat button instead of several, and clearer wording for selected users, groups and locations. | 4 |
| 9 Nov | Custom notifications | Master admin can write a message and push it to chosen people. It shows on top of their alerts until they clear it, and the admin sees who has cleared it. | 6 |
| 10 Nov | Sensor pause | Pause a sensor from its menu for a set time (15 minutes to 7 days) or until a date and time; it resumes by itself. | 6 |
| 10 Nov | Smaller changes | Phone numbers limited to 9 digits after +972. New users get Email and Push alerts by default (SMS optional). Alert table actions always visible. | 3 |
| 10 Nov | Mobile app specifications | Written implementation instructions for the Android app: messaging, custom notifications and timed pause. | 2 |
| 11 Nov | Sensor pause schedules | Planned pause from one date and time to another, and a daily pause on every day or selected days. The server starts and ends them automatically. | 6 |
| 11 Nov | HTTP devices | New HTTP sensors are named in the Device_key format (e.g. 4C9A5E_temp3) with short unit names. | 2 |
| 11 Nov | Server stability | Fixed location pages showing 'page not found'. The automatic restart now waits for the old server to stop fully, and its health check also tests location pages. | 2 |
| 12 Nov | Sensor pause follow-ups | A sensor with a planned pause shows in blue, and one click on 'Resume Pause' cancels the plan. Saving a sensor's settings no longer cancels a planned pause. Sensor preview no longer opens over the right-click menu. | 3 |
| | **Total** | | **121** |

## Adding entries

One CSV per billing period, named `YYYY-MM.csv`, with one row per task per day: `Date` (`YYYY-MM-DD`), `Task`, `Details` (what was delivered) and `Hours`. Add the period's total to the table at the top when it closes.

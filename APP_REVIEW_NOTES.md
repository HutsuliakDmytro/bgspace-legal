# App Review Notes — BG Space

Текст нижче вставляється в App Store Connect → App Review Information → Notes.
**Ліміт поля — 4000 символів**, тому нотатки скорочені (повна версія, з якої
різали, лишилась у `APP_REVIEW_NOTES_FULL.md` — вона НЕ для вставки).

Місця, позначені `<< ... >>`, треба заповнити перед відправкою:
демо-акаунт і список протестованих пристроїв.

Відео йде **вкладенням у Resolution Center** (App Store Connect → App Review →
відповідь на відмову), а НЕ в «App Previews and Screenshots» — це різні місця.
Якщо файл не влізе у вкладення, треба викласти його за посиланням і замінити
в пункті 1 «is attached to this reply» на «is available at: <URL>».

---

## NOTES (копіювати від наступного рядка)

DEMO ACCOUNT
Email: << демо-пошта >>
Password: << демо-пароль >>
A second demo account is available on request for a full two-player match.

1. SCREEN RECORDING
A screen recording made on a physical iPhone is attached to this reply. It
shows, in order: registering a new account and signing in; the lobby and a
match with dice rolls and checker moves; the post-match analysis; the
tournament list; the in-game chat, including reporting a message and blocking
its author; the "Blocked players" screen with unblocking; and deleting the
account.

2. MODERATION OF USER-GENERATED CONTENT
The only user-generated content is the in-game chat, together with usernames
and optional avatars. Every player has:
- Report: long-press any message written by another player, choose "Report",
  pick a reason (spam, abusive language, harassment, inappropriate content,
  cheating, other) and optionally add a comment. The report, with a copy of
  the reported message, goes to our moderators.
- Block: the same long-press menu. Blocking is immediate and hides the blocked
  player's messages both in the existing history and in anything sent later.
- Manage blocks: Profile > "Blocked players" lists everyone blocked and allows
  unblocking.
- Our moderators can delete individual messages and ban accounts.
- Support contact: bgspase.games@gmail.com, shown on our support page.
The menu is intentionally not shown on your own messages, so a second account
is needed to reproduce it.

3. ACCOUNT DELETION
Profile > "Delete account". The user confirms by typing a confirmation word,
after which the account and its personal data (email, username, avatar,
Telegram link) are permanently deleted and the app signs out. No email to
support is required.

4. WHAT THE APP IS
BG Space is a real-time multiplayer backgammon game: six variants (short,
long, hyper, khachapuri, six-one, tapa), tournaments, post-match analysis
(performance rating, luck, per-move mistakes), rating, match history with
replay, and cosmetic skins. The interface is available in Ukrainian, English,
German, Spanish, French, Italian, Turkish and Russian, and follows the device
language.

5. NO PURCHASES, NO GAMBLING
The app has no in-app purchases, no subscriptions and no payment processing of
any kind. In-game "coins" are a purely virtual score: they cannot be bought
with real money, cannot be exchanged for money and cannot be cashed out. They
are used only to enter tournaments and coin-stake matches, in the same way as
points in any free game, and no real-world prize is awarded. Because no real
money or real-world value is involved, no gambling licence applies.

6. PERMISSIONS AND EXTERNAL SERVICES
The app does not request location, contacts, camera, microphone or App
Tracking Transparency during normal use; photo library access is requested
only if a user uploads an avatar. The backend is our own (AWS EC2 and S3,
Stockholm; PostgreSQL; Redis). Linking a Telegram account is entirely
optional - registration and sign-in work fully without it. GNU Backgammon
(GPL) runs as a separate process on our server for the post-match analysis and
is not bundled into the app. The app uses no ads, no third-party analytics and
no AI services.

7. DEVICES TESTED
<< напр.: iPhone 11 Pro Max (iOS 26.6) >>

8. REGIONAL DIFFERENCES
None. The app behaves identically in every region; only the interface language
differs, following the device language.

Privacy policy and support page:
https://hutsuliakdmytro.github.io/bgspace-legal/

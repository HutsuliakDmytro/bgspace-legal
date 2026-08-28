# App Review Notes — BG Space

Текст нижче вставляється в App Store Connect → App Review Information → Notes.
Місця, позначені `<< ... >>`, треба заповнити перед відправкою.

---

## DEMO ACCOUNT

Email: <<dmutrogytsylak@gmail.com>>
Password: <<REMOVED>>

---

## NOTES (копіювати від цього рядка)

**1. Screen recording**

A screen recording made on a physical iPhone running the latest iOS is attached to
this reply. It starts with launching the app and shows, in this order:

- registering a new account, then signing in;
- browsing the lobby and playing a match with dice rolls and checker moves;
- the post-match move analysis;
- the tournament list;
- the in-game chat, including reporting a message and blocking its author, and
  the "Blocked players" screen where a block can be removed;
- deleting the account from the profile screen.

The app has no in-app purchases, no subscriptions, and no paid content, so no
purchase flow is shown. The app does not request location, contacts, camera,
microphone, or App Tracking Transparency permissions during normal use. Photo
library access is requested only if a user chooses to upload a profile avatar.

**1a. User-generated content: moderation tools**

The only user-generated content in the app is the in-game chat, together with
usernames and optional profile avatars. The following tools are available to
every player:

- **Report.** Long-press any chat message to open a menu with "Report". The
  player picks a reason (spam, abusive language, harassment, inappropriate
  content, cheating, other) and may add a comment. The report, together with a
  copy of the reported message, goes to our moderators for review.
- **Block.** The same long-press menu has "Block". Blocking is immediate: the
  blocked player's messages disappear from the chat for the person who blocked
  them, both in the existing history and in anything sent afterwards.
- **Manage blocks.** Profile → "Blocked players" lists everyone the user has
  blocked and allows unblocking.
- **Moderator removal.** Our moderators can delete individual messages and ban
  accounts that break the rules.
- **Contact.** The support address is shown in the app and on our support page:
  bgspase.games@gmail.com

Reporting and blocking are shown in the attached recording.

**1b. Account deletion**

Account deletion is available inside the app: Profile → "Delete account". The
user confirms by typing a confirmation word, after which the account and its
personal data (email, username, avatar, Telegram link) are permanently deleted
and the app signs out. No email to support is required. This flow is shown in
the attached recording.

**2. Devices and operating systems tested**

<< напр.: iPhone 14 Pro (iOS 26.5), iPad Pro 12.9-inch 5th gen (iPadOS 26.5) >>

**3. What the app does and who it is for**

BG Space is a real-time multiplayer backgammon game. It is aimed at backgammon
players of all levels, from casual players to club and tournament players.

The problem it solves: backgammon players have no convenient way to find an
opponent for the specific variant they play, and no easy way to understand why
they lost a game. BG Space provides both.

Core features:
- Six backgammon variants: short (standard) backgammon, long backgammon (narde),
  hyper, khachapuri, six-one and tapa. Each has its own rules and its own rating.
- Real-time matches against other players, with a doubling cube, Crawford rule,
  per-move and per-match clocks, and reconnection support.
- Tournaments: Swiss system and round robin, plus automatic blitz mini-tournaments.
- Post-match analysis: the app shows the player's PR (performance rating), a luck
  measure, and a per-move breakdown of mistakes.
- Rating, match history with move-by-move replay, and cosmetic board/checker/dice skins.

There is no gambling in the app. See point 7.

**4. How to set up and access the main features**

You can sign in with the demo account above, or register a new account directly
in the app: tap "Зареєструватись" / Sign up, fill in email, username and password,
and leave the optional Telegram field empty. Registration then completes
immediately, with no confirmation step and no third-party service involved.

After signing in:
- "Грати" / Play — opens the lobby. Create a table or join an existing one. Choose
  the game variant, match length, and clock settings.
- A second account is needed to play a full match against a live opponent. If you
  need a second demo account, we will provide one on request.
- "Турніри" / Tournaments — the list of open tournaments.
- "Історія" / History — completed matches, with move-by-move replay and the
  analysis screen (PR, luck, per-move error list).
- "Профіль" / Profile — rating per variant, statistics, avatar upload, and the
  account settings. This screen also contains "Заблоковані гравці" / "Blocked
  players" and "Видалити акаунт" / "Delete account".
- Chat moderation — open the chat inside a game or the global chat, then
  long-press any message written by another player. A menu appears with
  "Поскаржитись" / "Report" and "Заблокувати" / "Block". The menu is
  intentionally not shown on your own messages.
- The app interface is available in Ukrainian, English, German, Spanish, French,
  Italian, Turkish and Russian. The language follows the device language and can
  be changed in the app.

**5. External services used**

- Amazon Web Services (EC2, S3) — our own backend server and storage for user
  avatars. Region: Stockholm, Sweden.
- Telegram Bot API — entirely optional. A user may link a Telegram account to
  receive game notifications and to use Telegram as an alternative way to reset
  a password. Registration and sign-in work fully without it, and the app never
  requires the user to install or open Telegram.
- SMTP email (nodemailer) — transactional email, such as password recovery.
- GNU Backgammon (gnubg) — an open-source (GPL) backgammon engine. It runs as a
  separate process on our own server and is used only to evaluate finished
  positions for the post-match analysis. It is not bundled inside the iOS app.
- PostgreSQL and Redis — our own database and cache, on our own server.

The app does NOT use: payment processors, advertising networks, third-party
analytics or attribution SDKs, or AI/LLM services.

**6. Regional differences**

There are none. The app behaves identically in every region and every country.
The only difference is the interface language, which follows the device language.
No content, feature, or game mode is restricted by region.

**7. Regulated industry and third-party material**

The app is not a gambling app and does not operate in a regulated industry.

The in-game "coins" are a purely virtual score. They cannot be bought with real
money, they cannot be exchanged for real money, and they cannot be cashed out.
The app contains no in-app purchases and no payment processing of any kind.
Coins are granted inside the game and are used only to enter tournaments and
coin-stake matches, in the same way as points in any free game. No real-world
prize is awarded. Because no real money or real-world value is involved at any
point, no gambling licence applies.

Backgammon itself is a traditional public-domain board game and is not subject
to any third-party rights.

The analysis feature uses GNU Backgammon, which is free software licensed under
the GNU General Public License. It runs on our own server as a separate process
and is not linked into or distributed with the iOS app.

Privacy policy and support page: https://hutsuliakdmytro.github.io/bgspace-legal/

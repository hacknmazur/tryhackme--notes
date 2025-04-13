🔗 [Room on TryHackMe](https://tryhackme.com/room/windowsfundamentals1xbx)
🔗 [Room on TryHackMe](https://tryhackme.com/room/windowsfundamentals2x0x)
🔗 [Room on TryHackMe](https://tryhackme.com/room/windowsfundamentals3xzx)

🪟 Windows Fundamentals — TryHackMe Notes (EN + UA)

Цей файл містить нотатки з перших двох кімнат Windows Fundamentals на платформі TryHackMe. Інформація подається англійською та українською мовами для кращого розуміння та повторення.

This file contains notes from the first two rooms of Windows Fundamentals on the TryHackMe platform. The information is presented in English and Ukrainian to support better understanding and retention.

📂 Environment Variables (Змінні середовища)

%windir% — Path to the Windows directory.

Шлях до теки, де встановлена Windows.

%systemroot% — Same as %windir%, typically C:\Windows.

Те саме, що %windir%, найчастіше це C:\Windows.

%userprofile% — Path to the current user's profile directory.

Шлях до профілю поточного користувача (наприклад, C:\Users\andriy).

%temp% — Directory where temporary files are stored.

Папка для тимчасових файлів, які часто очищаються після перезавантаження.


⚡ PowerShell vs CMD

CMD is the classic Windows command-line tool, useful for basic tasks.

CMD — класичний інструмент Windows для базових команд.

PowerShell is a modern and powerful command-line interface and scripting environment.

PowerShell — сучасне середовище командного рядка з підтримкою скриптів та автоматизації.

CMD is the classic Windows command-line tool, useful for basic tasks.

CMD — класичний інструмент Windows для базових команд.

PowerShell is a powerful scripting environment based on .NET.

PowerShell — більш потужне середовище, що дозволяє працювати з об'єктами та автоматизацією.

DLL file

Файл DLL — це бібліотека, яка містить набір коду та даних для виконання певної дії в Windows.  Потім програми можуть звертатися до цих файлів DLL, коли їм потрібно виконати цю дію. Файли DLL багато в чому схожі на виконувані файли (EXE), за винятком того, що файли DLL не можна виконувати безпосередньо в Windows.


📁 ADS — Alternate Data Streams (Альтернативні потоки даних)

Feature of NTFS allowing hidden data in files using file:stream syntax.

Механізм NTFS для збереження прихованих даних у файлі через file:stream.

Example:

echo Hidden > normal.txt:hidden
more < normal.txt:hidden

Useful for metadata, but often abused by malware to hide malicious code.

Використовується для метаданих, але зловмисники часто ховають шкідливі дані.


👥 User Management — lusrmgr.msc

Інший спосіб отримати доступ до цієї інформації, а потім і деякі інші, — це використання локального керування користувачами та групами. Клацніть правою кнопкою миші меню «Пуск» і виберіть «Виконати». Тип lusrmgr.msc.

🔐 UAC — User Account Control

User Account Control (UAC) helps prevent malware from damaging the PC and allows organizations to deploy desktops with better management. With UAC, apps and tasks run in the security context of a non-administrator account unless an administrator authorizes elevation. UAC can block unauthorized installations and prevent accidental system changes.

Контроль облікових записів користувачів (UAC) допомагає запобігти пошкодженню ПК зловмисним програмним забезпеченням і допомагає організаціям розгорнути робочий стіл з кращим керуванням. За допомогою UAC програми та завдання завжди запускаються в контексті безпеки неадміністраторського облікового запису, якщо адміністратор спеціально не авторизує доступ до системи на рівні адміністратора. UAC може блокувати автоматичне встановлення несанкціонованих програм і запобігати випадковим змінам налаштувань системи.

🛠️ MSConfig — System Configuration Utility

msconfig.exe — launches the System Configuration Utility, used for advanced troubleshooting.

The main goal is to diagnose startup problems.

Утиліта конфігурації системи (MSConfig) призначена для розширеного усунення несправностей, і її основна мета – допомогти діагностувати проблеми запуску.

📄 Event Log Types (Типи подій)

Event Type

Description

Error - Critical issue (data loss, system failure)

Warning - Potential issue that hasn't caused a failure yet

Information - Successful action or service message

Success Audit - Successful security-related action (e.g. login)

Failure Audit - Failed attempt at a secure action (e.g. failed login)

Тип події

Опис

Error - Серйозна проблема (втрата даних, збій служби)

Warning - Потенційна проблема, яка ще не спричинила збій

Information - Інформує про успішне виконання дій

Success Audit - Успішна безпекова подія (наприклад, вхід у систему)

Failure Audit - Невдала спроба безпечної дії (наприклад, невдалий логін)

📋 Event Logs (Журнали подій)

Application — events from applications

Security — security-related events (e.g. logins, permission changes)

System — system-level events (drivers, services)

CustomLog — custom log entries from user applications

Application — події від програм

Security — події безпеки

System — події від системи

CustomLog — власні журнали програм

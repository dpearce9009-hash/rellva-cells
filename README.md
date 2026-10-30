<img src="docs/rellva-office.svg" alt="Rellva Office" width="96" height="96">

# Rellva Office

Rellva Office is a Windows app for managing your local Codex chats and projects with friends. Message your workers, manage their tasks, assign coordinators, and visit the floors of people who join your private office.

- Open saved local chats or create workers for separate projects.
- Track planned, running, completed and blocked tasks for each worker.
- Run tasks yourself or start a limited automatic queue. Pause and stop your own workers.
- Organize workers into teams with coordinators and approve suggested assignments.
- Share worker names and activity with invited friends. Each person controls only their own workers.
- View a chosen local window inside a worker's monitor. Desktop video stays on that computer.

## Install on Windows

1. **Install OpenAI's desktop app and sign in.** Follow the [official Windows installation guide](https://learn.chatgpt.com/docs/app/windows). Open the app and sign in with your own ChatGPT account. If your app has a ChatGPT/Codex selector, choose **Codex** for project chats. An existing signed-in Codex desktop installation can be used. [Official sign-in and setup instructions](https://learn.chatgpt.com/docs/quickstart).
2. **Download [Rellva-Office-Setup.exe](https://github.com/dpearce9009-hash/rellva-office/releases/latest/download/Rellva-Office-Setup.exe).** If you use the [release page](https://github.com/dpearce9009-hash/rellva-office/releases/latest), expand **Assets** and click that exact filename. **Source code**, `.blockmap` and `latest.yml` are not installers.
3. If Rellva is already running, finish its current tasks and close it before updating.
4. Open your browser's downloads with **Ctrl+J**, find **Rellva-Office-Setup.exe**, and open the file. The installer installs for your Windows user and creates a Rellva Office shortcut. This preview is unsigned; if Windows SmartScreen appears, use **More info → Run anyway** only after confirming the file came from this repository.
5. Open **Rellva Office** from the Windows Start menu. Its connection indicator should read **Local Codex · saved chats**. If it says **Offline** or **Connection unavailable**, finish signing in to OpenAI's desktop app, then select **Access & controls → Refresh connection** in Rellva.

Rellva uses your existing local Codex sign-in and its usage limits. This build does not require a separate API key. Each friend needs their own account and service connections.

## Join your friend's office

1. Ask the office owner to send you the **private office invitation** separately. The public download does not include it.
2. After installing Rellva, open that invitation in your browser.
3. Click **Open Rellva Office** on the invitation page. If your browser asks whether to open the app, allow it to open Rellva Office.
4. In Rellva's confirmation window, click **Join office**. Your computer contributes its own floor. Connected people appear in the floor list; choose one to view their workers.
5. If the browser does not open Rellva, open the app yourself and choose **Access & controls → Join a room**. Paste the **entire invitation**, including everything after `#`, into **Room address**. Leave **Private token** blank when the full invitation already includes it, then click **Join office**.

Keep Rellva open and connected while you want your floor visible. Keep the invitation private; anyone with it can join that office.

## Add and use your workers

1. Click **Add worker**. Choose a saved chat, or fill in **Worker name** and **Department**, click **Create worker**, then select that project's working folder.
2. Select a worker to open its room and conversation. Type in its message box to give it work. **Back** returns to the floor.
3. Open **Tasks** to manage its project. Manual tasks wait for **Run**. Automatic work needs an explicit **Start auto** and a task limit.
4. Use **Pause** to prevent further automated tasks after the current task finishes. **Stop now** also interrupts work started in Rellva. Resuming does not start work by itself.
5. Open **Teams** to choose a coordinator and its workers. Approving a coordinator's suggestion adds a task; it does not run that task.

## Sharing and current limits

Other people can see shared worker names and activity. They cannot control your workers, approve their actions, or open your private files, goals, task lists or desktop video. Shared consultation excerpts require explicit consent from the participating owners.

This preview works with **local Codex chats**. It does not import every cloud-only ChatGPT conversation. If a chat is owned by another active session, finish its work and fully quit that source app before continuing it in Rellva, or create a separate worker in Rellva.

The installed app checks for updates. You can also use **Access & controls → Check updates**. Shared floors require the owners' apps to be running; persistent building accounts are not included.

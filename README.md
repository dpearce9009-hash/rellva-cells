<img src="docs/rellva-office.svg" alt="RellvaCells" width="96" height="96">

# RellvaCells

Previously named Rellva Office. The update keeps the existing installation, workers and private settings.

RellvaCells is a Windows app for managing local Codex chats, projects, and shared office floors. Each person uses their own account and controls their own workers.

- Message workers, manage project tasks, and assign coordinators.
- View your workers in a 3D office and visit friends’ shared floors.
- Invite a friend’s worker to review material you choose to share.
- Open an approved local or privately paired desktop in a separate worker window.
- See available Codex usage information from your existing account.

## Install on Windows

### First installation

1. **Use your own signed-in OpenAI desktop app.** If you already have it, keep it and select **Codex** in the product selector, then **This computer / Local** for local project chats. An existing signed-in Codex desktop installation also works. If needed, follow [OpenAI’s Windows setup guide](https://learn.chatgpt.com/docs/app/windows).
2. **Download and run [RellvaCells-Setup.exe](https://github.com/dpearce9009-hash/rellva-cells/releases/latest/download/RellvaCells-Setup.exe).** On the [release page](https://github.com/dpearce9009-hash/rellva-cells/releases/latest), expand **Assets** and choose that filename. If you received **RellvaCells-Friends.zip**, right-click it, choose **Extract All**, and run the installer inside. The installer installs for your Windows user and creates a shortcut. You do not need an existing Rellva installation or to close OpenAI’s app to install Rellva. This preview is unsigned; if SmartScreen appears, check that the file came from this repository before choosing **More info → Run anyway**.
3. **Open RellvaCells from Start.** The connection indicator should read **Local Codex · saved chats**. If it says **Offline** or **Connection unavailable**, finish signing in to Codex in OpenAI’s desktop app, then choose **Settings → Refresh connection** in Rellva.

The first-launch **Connect this PC** prompt is optional desktop viewing. Choose **Not now** to start with just your office, or connect later under **Settings → Desktops**. This prompt does not set up workers or grant keyboard/mouse input.

No separate API key is needed. Each person uses their own Codex account and usage allowance. The current OpenAI desktop app includes a Codex product selector; ordinary ChatGPT **Chat / Work** histories are a different source and are not imported by Rellva. [OpenAI’s desktop guide](https://learn.chatgpt.com/docs/app).

### Set up your workers once

Rellva automatically discovers **local Codex chats** and uses available native section names as department labels. It first shows chats already added to Rellva or in a section containing “Rellva”; if none match, it shows up to 36 recent top-level chats. A missing saved chat can be added through **Add worker → saved chats**.

**Coordinator/team relationships need one-time confirmation.** A native section or a chat named “HQ” does not establish a team automatically.

- **Use existing chats:** open **Teams**, choose the coordinator and its workers, enter a team name, then save. Saving this relationship does not send an introduction or start project work.
- **Start a new team:** choose **Add coordinator**, give it a name, section, responsibilities and project folder. Then use **Add worker** and select that coordinator. Rellva creates and places the native chats and sends the setup brief/introduction after you confirm setup. Those model messages can use your Codex allowance.

Discovery itself does not start project tasks. Your friend gets their own workers and settings; installing or joining your office does not copy your chats, coordinators or private setup. Advanced build-plan feeds and department Play/Pause receivers require their own setup, described below.

### Update an existing installation

Only if RellvaCells is already installed: finish its current work, close **RellvaCells**, run the new installer and reopen it from Start. Your workers and settings are retained.

Use **Floors** at the top to choose your own or a connected friend’s floor. **Tools** contains reviews, worker exchange, usage and worker controls. **Settings**, beside Tools, contains appearance, desktop connections, sharing, permissions and updates. The top usage summary opens Usage & credits.

## Join a friend’s office

1. Ask the owner for their **private office invitation**. It is sent separately and is not included in the public download.
2. Open the invitation in your browser and choose **Open RellvaCells**. Allow your browser to open the app if asked.
3. In Rellva, choose **Join office**. Select a connected person’s floor to view their workers.

If the link does not open the app, choose **Settings → Join a room**. Paste the **entire invitation**, including everything after `#`, into **Room address**. Leave **Private token** blank when the invitation already includes it, then choose **Join office**.

Keep Rellva open while sharing your floor. Keep the invitation private; anyone with it can join that office.

## Workers and projects

Coordinators and each department have their own office light-rail network, connected by a shared hallway rail for messages between sections.

Choose **Add worker**, enter a name, select a department and coordinator, then choose a working folder. Rellva creates a native local Codex chat, places it in the selected coordinator’s section, and, when a coordinator is selected, sends a private introduction in both chats. Choose no coordinator to create an independent worker. If section placement cannot be verified, setup remains unfinished. If a coordinator is busy or a setup step fails, **Retry setup** continues the same chat; it does not create another. Unconfirmed native operations are held for inspection. You can also add a saved chat. Select a room for its terminal; **Workers** searches the floor and **Back** returns to it.

Choose **Add coordinator**, enter its name and its new **Section name**, and optionally describe its **Responsibilities**. Choose a project folder. Rellva creates its native Codex chat and section, registers its team and gives it an owner-private office brief: operating preferences, existing reporting relationships, project goals and task state, schedules and relevant settings. Responsibilities become its initial Project goal, which you can edit later. The coordinator starts with an empty team; use **Teams** or **Add worker** to assign its workers. Setup reuses its recorded chat and completed steps on retry. The brief is a dated snapshot, not every past conversation or a grant of new permissions.

- **Tasks:** generate a plan, review proposed tasks, and use **Run** for manual tasks. Automatic queues need an explicit **Start auto** and a task limit.
- **Pause queue after task:** prevent more automated tasks for that worker after the current task finishes. **Stop worker** also interrupts work started in Rellva. **Tools → Pause all queues** and **Tools → Stop all tasks** apply across your workers; department controls show the affected worker count. Resuming permits work but does not start a queue.
- **Teams:** choose a coordinator and its workers. Approving a suggested assignment adds a task; it does not run it.
- **Project:** inspect progress and task details. For coordinators, the same view contains the goal, planning controls and proposed assignments. Approving an assignment adds a task; it does not start work.
- **Files:** open the worker’s saved files. A verified new file receives a brief clickable arrival effect in its room; historical files stay in Files.
- **Monitor:** see available real command output, text or image previews. Previews and deliveries stay private to the owner.
- **Requests:** click a room’s request indicator to open the exact pending approval or question. Supported commands, permissions and forms can be answered inside Rellva for work it runs. Unsupported forms, service sign-ins and Windows security dialogs still use their own controls. Viewing a request never approves it.

The **Rellva Auto** and **Digital Auto** switches beside the Office filters apply to departments named **Rellva** and **Rellva Digital**. They generate and run eligible project tasks in finite batches using each worker’s existing task limit. Workers without a goal, already busy, or waiting for input are skipped. Turning a switch **Off** prevents new auto tasks after the current task finishes. These switches do not change Codex schedules and appear only on your own floor.

On the floor, **Show processes** opens one live feed across your workers: each active worker’s current activity and any running command or tool step. Search or filter the feed. Use Commands & logs for original details; Close or Escape returns to the feed. Activity shows the three newest finished processes, including reported failures. It rolls forward as work finishes, without scrolling or growing the page. Generated project tasks remain in each worker’s Tasks tab. Select a worker to chat directly.

### Worker terminal

The message box stays visible while the conversation scrolls inside its own bounded window. User messages and worker replies use readable headings, lists, links and code blocks. Process steps are grouped in collapsible sections; open **Commands & logs** for their original commands, outputs and errors. **Copy** copies a message, and **Copy code** copies a code block. A finished test command alone is not a claim that its tests passed.

Local image previews load as they enter the visible conversation. Click file links or **Open image** to open available referenced files; external images remain links until opened. Files are checked on the owner’s computer, and unavailable references are labelled. Chat content and these previews are not shared with friends.

Draft messages and selected attachments stay with their worker while you switch rooms in the app. **Load older messages** adds earlier saved history without losing your reading position. The selected local chat refreshes recent readable history without resuming it or starting a model turn. During a task started in Rellva, **Send update** adds instructions to that same running task and pauses any next automatic task; it does not start another turn. Answer pending approval first.

Rellva renders the conversation content provided by the native interface; it is not a pixel-for-pixel copy of the Codex app. Historical approvals and questions appear only when the native history provides them. Active approvals can be answered only when their request is available to this connection. Unsupported forms, service sign-ins and Windows security dialogs use their native or service controls. A task owned by another active app cannot be steered here; read-only history access does not take ownership.

A newly observed successful live process gives its worker a brief, cute completion effect. Repeated updates for the same process do not replay it, and opening old history does not trigger celebrations. Failed or unfinished processes do not trigger it. Reduced motion uses a still confirmation without the bounce or sparks; the effect does not claim that a whole project is complete.

The Workers menu contains the department/team filter, worker search and separate total/working counts. Settings includes the saved Scheduled tasks animation effect dropdown: Rainbow tiles, Orbiting light or Off. Rainbow tiles cycles colored outlines across the whole floor while tile centres stay dark. Orbiting light is the default: one light travels along the cell outline, with a bright light-blue border and a dark floor. These effects are for scheduled cells while not actively working. Actual work keeps its three moving outline lights. Saved Rainbow tiles and Off choices are preserved; previously enabled settings without a chosen mode use Orbiting light.

Idle office routines are visual animations. They do not run searches, complete project tasks, or spend model usage. Actual activity is indicated separately.

Scheduled Codex tasks appear in the owning worker’s terminal with their enabled or paused status and a readable schedule. Friends do not receive task names, prompts, or schedule details.

Small helper bots appear when the local runtime reports active child agents. Up to six are shown; an unknown or unavailable count does not create pretend helpers.

## Build plan accuracy

Each person must connect their own plan source; installing Rellva or joining an office does not supply the example office’s plan feed.

**Settings → Build plans** connects a coordinator to a local plan feed. Choose the coordinator and its current plan pointer. If its evidence is stored elsewhere, use **Add evidence folder** to select that folder. **View plan** opens the verified text in Rellva.

While Rellva is open, connected plans are checked every hour and after a task finishes. **Refresh now** checks immediately. Unchanged tasks keep their IDs and history; changed revisions appear for review. Paused, stale or unavailable sources are shown clearly. Disconnecting removes the connection and keeps task history.

Imported tasks show the build plan’s progress separately from the worker’s local execution result. Finishing a worker run does not claim independent review or coordinator adoption. **Use revision** releases an eligible revised task for your review; **Run** starts it separately. Rellva checks the current owner, exact task revision, dependencies, holds and execution authority again before sending work. An uncertain previous run is held for reconciliation instead of being sent twice.

Hourly checks read the connected plan and merge changed tasks. They do not spend model usage generating a new list or start work automatically. The plan producer must keep its current pointer and evidence updated. Existing manual task generation and finite automatic queues remain available.

A source can provide an advisory ledger of known submissions and reviews without runnable tasks. Rellva labels that limit, shows its verified plan text, and preserves unknown owners and missing dependencies. It does not turn readiness goals or old review records into new worker assignments.

## Department Play and Pause

Each department needs its own verified coordinator receiver. A fresh installation does not include the example office’s receiver configuration; unavailable receivers are shown as unavailable.

Beside each department’s **Auto** toggle, **Play** asks its coordinator to continue that department’s authorized unfinished work. **Pause** addresses only the exact non-recurring attempts running in that department when clicked. Recurring work, schedules, later attempts and other departments remain unchanged. The Auto toggle remains a separate control for finite project queues.

Each department has independent request and observed status. A queued message waits for its coordinator to receive it; delivery is not a claim that work started or stopped. Its buttons wait for that request to be resolved before sending another; other departments stay independent. Rellva shows confirmed results only after the matching coordinator receipt. If all selected attempts were protected or already finished, it reports that the selection was checked. Unavailable receivers and uncertain outcomes remain visible and are not silently replayed.

If the current build plan cannot be verified, Play and Pause stay unavailable for new commands. The last matching, verified command receipt remains visible, including a confirmed **Ready** result when no eligible unfinished work was available. **Check again** rereads status without sending another command; **Build plans** opens the source settings. A changed evidence hash must be corrected and published by the plan producer. An earlier receipt does not authorize new work or silently replay an uncertain request.

Workers appear as luminous nuclei. Observed active subagents appear as smaller glowing proton-like helper particles, with their established routines unchanged. Lasers, crowns, holograms and arrival effects remain. Actual working rooms use three moving perimeter lights; scheduled Orbiting light uses one light with the same style along the cell border while the cell is not actively working.

During an idle charging visit, a thin cable connects the nucleus to the existing left-wall outlet and the nucleus glows softly and slowly. This is visible in both the overview and focused room. Reduced motion keeps the charging effect still.

The installer includes the complete official Windows Codex control runtime and its license notices. It starts a local shared helper only for an explicit process command, reusing an existing compatible helper. Each person continues to use their own Codex account. Source archives omit the large binary directory; the included runtime source note and integrity receipt identify the exact official package needed to rebuild it.

## Work levels

Each room's XP bar sits directly below its monitor, above the floor.

Workers gain 10 XP per recorded owner-message/reply pair, 1 XP per successfully finished tool step, and 20 XP per completed Rellva task. Level 1 starts at zero XP; each level starts at `50 × (level − 1)²` total XP. Existing local history is counted automatically in bounded, cached passes. New workers may show Calculating level while their initial scan finishes. Friends see only numeric level and XP values. Levels measure recorded activity; they do not measure intelligence or model quality. No extra setup is required.

**Settings → Check project connections** lists installed apps and MCP tools from your local Codex runtime. A listed or callable connection is not proof of service authorization; permissions are checked when the worker uses it. The existing VM browser workflow is separate, and VM control has not been tested end to end in this build.

**Tools → Usage & credits** includes a private task ledger for work started in Rellva. It records native input, cached-input, output, reasoning and total token counts when reported, with **Complete**, **Partial** or **Unavailable** coverage. Child-agent usage is included only when the runtime reports it under that worker turn. A lost connection or unknown baseline stays partial; old per-task usage is not invented from account totals. Rough token ranges shown before a task use task metadata and are estimates, not bills. Per-task API cost and credits spent remain unavailable when the runtime does not report them.

## Review Sessions

Both people must be in the same office with review support enabled.

1. Open **Tools → Review Sessions**, select your worker and your friend’s worker, and write a brief. Add only the excerpts and reference descriptions or public links you want reviewed.
2. Choose **Preview invitation**. Inspect the shared material, then choose **Send invitation**. Preparing or viewing a preview sends nothing.
3. Your friend chooses **Review invitation**, inspects it, and chooses **Accept & run** or **Decline** for their own worker.
4. Findings stay private on the reviewing owner’s computer. That owner chooses a response excerpt, uses **Preview response**, and then chooses **Share response**.

Reviews use an isolated text session. A review grants no control over another owner’s workers or desktop and applies no production edits. Other floors do not receive the brief or findings. Shared review payloads are limited to 48 KB.

## Worker desktop windows

For this PC, open **Settings → Desktops → Connect this PC** and approve the Windows dialog. Select your worker, choose **Desktop → Change desktop**, then choose the computer and display. **Desktop → Open desktop** opens its separate window.

- **Take control:** pauses the worker’s desktop input. For this PC, use Windows directly; the viewer does not send your input back into the same screen. For a paired remote PC, click the viewer to use its mouse and keyboard.
- **Let worker work:** separately grants the selected worker input access. Minimize a local viewer while the worker uses this PC.
- **Pause / Stop / Close:** remove that window’s input access. **Stop** also interrupts the worker’s active Rellva turn.

Opening a viewer alone grants no input access. Watching a shared office floor grants no desktop access.

### Pair another PC

Both PCs need RellvaCells open and must join the **same private office**. Pairing is optional and uses a separate private invitation.

1. On the PC being shared, open **Settings → Desktops**. Enter a PC name under **Share this PC**, then choose **Share this PC**.
2. In its new pairing row, choose **Copy pairing**. Send that private invitation to the other PC’s owner.
3. On the other PC, paste it into **Private pairing invitation** under **Connect another PC**, choose **Connect another PC**, and confirm the Windows dialog.
4. On the shared PC, choose **Approve viewing**, select the displays, choose **Approve**, and confirm the Windows dialog. Viewing lasts up to eight hours, bounded by the pairing’s expiry.
5. To permit keyboard and mouse input, the shared PC’s owner separately chooses **Allow control 5 min**, selects the displays, and approves. On the other PC, assign that paired computer to a worker and choose **Desktop → Open desktop**. Choose **Take control** for yourself or **Let worker work** for that worker.

**Stop control** removes keyboard and mouse permission while retaining approved viewing. **Revoke** removes the pairing. After a connection loss, **Reconnect** requires fresh host approval; prior permission is not restored automatically. Approving remote input pauses local worker desktop control. Taking local desktop control removes remote input permission.

Desktop traffic is encrypted between the paired apps. The relay routes it, and other office members do not receive it. Keep pairing invitations private; they are not included in shared floors or public downloads.

## Usage & credits

The top bar shows Usage left and a separate API balance. The usage meter uses the lowest remaining reported Codex allowance; allowance windows and reset times remain in the details. Click it to open **Usage & credits** for reset times and activity. It reads available Codex allowance, reset, and token activity information from your existing local account connection. No additional setup is needed. Fields the account service does not provide are shown as unavailable.

API balance and API spending are currently **Unavailable** in the app. **Open API balance** and **Open API spending** open the account’s billing pages. An unavailable API balance is never treated as zero.

## Sharing, updates, and current limits

Shared floors show selected worker names and activity. Conversation excerpts are shared only when that option is enabled. Each owner controls their own workers, approvals, files, goals, and task lists. Desktop viewing or input requires the separate pairing approvals above. Service sign-ins and private project data are not included in the installer.

This preview uses **local Codex chats**; it does not import every cloud-only ChatGPT conversation. If another active session owns a chat, finish its work and fully quit that source app before continuing the chat in Rellva, or create a separate worker.

The installed app checks for updates. You can also choose **Settings → Check for updates**. Shared floors require the participating apps to remain open; persistent building accounts are not included.


**Settings → Usage safeguard:** choose Off or 0%, 25%, 50%, 75% or 100% allowance remaining. Rellva stops its automatic planning, queues and running automatic tasks at or below the threshold reported by Codex. It also stops automatic work if limits cannot be checked. Manual work remains available. Stopped queues require an explicit restart; native Codex schedules are unchanged. Reported limits can lag.

### Avatar visibility

Workers and helpers have clearer neon bodies that stand out over floor lighting and holograms. The computer-focus ring is a dim, narrow floor accent beneath the worker.

### Department status and charging

Auto, Play and Pause stay aligned above their department status. Ready and verified receipt details remain available without a routine no-work note; source verification failures and request errors still need attention. Charging uses a clearer, slow nucleus glow in overview and focused rooms, with a still appearance under reduced motion.

The worker terminal fills its shared column, with the message box flush to the panel edges. Verified active helpers have small neon monitor pointers.


### Version 0.1.27: quieter status and helper activity

Routine no-work notes are no longer displayed below department controls. Ready and the existing verified receipt details remain available. A saved receipt is historical, not a live task count or a claim that all project work is finished. Open Build plans for current progress. Source verification failures, pending requests and actual errors remain visible.

Observed active helpers move between more work spots around their own room and pause to build holograms. A helper uses either its hologram or its small monitor pointer at a time. Its pointer scans its own monitor as the helper moves. These are visual assist routines for reported active helpers; they do not invent child agents, task results or model work.


### Version 0.1.27: worker message configuration fix

This update fixes a desktop-tool configuration error that could prevent a worker message from starting when no desktop viewer was connected. Desktop viewing and input still require their existing approvals. The update does not resend a failed message automatically. Copy any unsent draft before closing for the update, then review it before choosing Send again.


### Version 0.1.27: recurring workers and cell activity

Workers now shows a green Working count and an orange Recurring count. Recurring counts workers with enabled native recurring Codex tasks, not the number of jobs. The dropdown puts working workers first in green, then recurring workers in orange, then other workers. A worker that is both working and recurring appears once at the top with both badges. Paused schedules, one-off tasks and Rellva automatic queues do not add to the recurring count. Friends’ recurring indicators use shared status metadata when available; task names and prompts stay private.

Hover over a cell to see its worker’s name and available current activity beside the pointer. Idle, waiting and unavailable states remain labelled honestly; a completed step is not presented as a running process. Friend floors use only activity already shared by that owner. The upper-right Tooltips On/Off button controls these labels. Tooltips start On; choosing Off hides them immediately, and your choice is saved on this computer.

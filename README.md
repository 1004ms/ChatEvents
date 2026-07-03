# ChatEvents Wiki

ChatEvents is a lightweight Paper plugin that adds simple chat-based events to your Minecraft server.

You can create custom question events, enable automatic number guessing events, start MirrorChat mode and manage everything from an in-game GUI.

---

## Commands

```text
/chatevents
```

Shows the plugin help.

```text
/chatevents gui
```

Opens the admin GUI.

```text
/chatevents reload
```

Reloads the plugin configuration, questions and language files.

```text
/chatevents lang <language>
```

Changes the plugin language.

```text
/chatevents mirror [seconds|stop]
```

Starts or stops MirrorChat mode.

```text
/chatevents start question
```

Starts a random question event.

```text
/chatevents start number
```

Starts a number guessing event from 1 to 100.

---

## GUI

Open the GUI with:

```text
/chatevents gui
```

The GUI includes:

```text
Add Event
View Events
Enable 1-100 Guess
Start MirrorChat
Reload Plugin
```

---

## Creating an Event

To create a question event:

1. Use `/chatevents gui`.
2. Click `Add Event`.
3. Type the question in chat.
4. Type the answer in chat.
5. The event is saved automatically.

Created events are stored locally in:

```text
plugins/ChatEvents/questions.yml
```

---

## Number Guessing

ChatEvents includes an automatic number guessing mode.

When enabled, the plugin can start a random event where players must guess a number from 1 to 100.

This does not require creating numbers manually.

---

## MirrorChat

MirrorChat reverses player chat messages for a short event.

Example:

```text
hello
```

becomes:

```text
olleh
```

You can start it with:

```text
/chatevents mirror 60
```

and stop it with:

```text
/chatevents mirror stop
```

---

## Languages

Available languages:

```text
en
it
es
fr
custom
```

Supported aliases:

```text
eng
ita
esp
spa
fra
en_US
it_IT
es_ES
fr_FR
```

Examples:

```text
/chatevents lang en
/chatevents lang it
/chatevents lang es
/chatevents lang fr
/chatevents lang custom
```

---

## Permissions

```text
chatevents.admin
```

Main admin permission.

```text
chatevents.gui
```

Allows opening the GUI.

```text
chatevents.reload
```

Allows reloading the plugin.

```text
chatevents.lang
```

Allows changing the plugin language.

```text
chatevents.mirror
```

Allows starting and stopping MirrorChat.

```text
chatevents.start
```

Allows manually starting events.

---

## Placeholders

ChatEvents supports these placeholders in messages and reward commands:

```text
<player>
%player%
<answer>
%answer%
<type>
%type%
```

---

## Rewards

Winner rewards are executed from console.

Example:

```yaml
rewards:
  commands:
    - "eco give <player> 1000"
    - "crate key give <player> rare 1"
```

---

## Winner Effects

Winner effects are configurable in the config.

You can enable or disable:

```text
Broadcast
Sound
Title
Actionbar
Particles
Firework
Reward commands
```

---

## Installation

1. Download the plugin jar.
2. Put it inside your `plugins` folder.
3. Restart the server.
4. Use `/chatevents gui`.
5. Create your events.

---

## Compatibility

ChatEvents is made for Paper servers.

```text
Supported: Paper
Not officially supported: Bukkit, Spigot, Folia
```

---

## Support

If you find any bug, contact:

```text
pupillaviolaalt
```

# Agent HQ community rooms

Rooms people built in [Agent HQ](https://github.com/eezsm93/agent-hq-releases) and shared so you can install them in one click: a team of agents with their roles and briefings, the room's rules and the connectors it uses.

## Install a room

In Agent HQ open **Rooms → Import → Community**, pick a room and click **Preview**. You'll see the agents and which connectors are ready on your computer before anything is created. Your existing rooms are never changed.

You can also download any `.agenthq.json` file from [`rooms/`](rooms) and drop it on **Rooms → Import → From a file**.

## Share your room

1. In Agent HQ: **Rooms → Export** (or the ⤴ button on a room). Leave "Include the rooms' memory" off.
2. [Open the "Share a room" form](https://github.com/eezsm93/agent-hq-rooms/issues/new?template=share-room.yml), describe it and drag the `.agenthq.json` file into the form.
3. Once it's reviewed, it shows up in everyone's Community tab.

Exported files never include your folders, accounts, tokens or task history; connector keys are replaced by blanks for whoever installs the room. Still, take a quick look at the file before sharing.

## Guidelines

- One purpose per room (or per building of rooms), with a clear name and description.
- Agent briefings in English, written for anyone (no private names, links or data).
- Nothing harmful: no agents meant to spam, deceive, scrape private data or break the law.

## For maintainers

`index.json` lists the gallery; each entry points to a file in `rooms/`. To publish a submission: save the attached file to `rooms/<id>.agenthq.json`, add an entry to `index.json` (`id`, `file`, `name`, `description`, `author`, `tags`, `rooms`, `agents`, `color`) and close the issue with a thank-you.

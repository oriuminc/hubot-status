# Hubot: hubot-status

A simple status manager script for Hubot.

See [`src/status.coffee`](src/status.coffee) for full documentation.

## Installation

Add **hubot-status** to your `package.json` file:

```json
"dependencies": {
  "hubot": ">= 2.5.1",
  "hubot-scripts": ">= 2.4.2",
  "hubot-status": ">= 0.0.0",
  "hubot-hipchat": "~2.5.1-5",
}
```

Add **hubot-status** to your `external-scripts.json`:

```json
["hubot-status"]
```

Run `npm install`

## Sample Interaction

```
alice>> hubot away I'm out for lunch. Back at 1pm.
hubot>> alice is away.
  * billy enters channel.
billy>> alice: hey did you let all these cats into the building?
hubot>> alice is away: I'm out for lunch. Back at 1pm.
billy>> Grrrr...
billy>> hubot status Expelling cats.
hubot>> billy has a new status.
alice>> hubot returns.
hubot>> alice has returned.
alice>> hubot statuses
hubot>> bernard: In a client meeting.
        billy: Expelling cats.
alice>> Nooooooooo!
```

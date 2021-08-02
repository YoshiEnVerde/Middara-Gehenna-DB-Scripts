# Gehenna: The Unofficial Middara Companion App (Desktop UI) (`Middara-Gehenna-DB-Scripts`)
Sets of scripts that handle creation and data load of the DBs of an Unofficial Middara companion app to automate as much of the gameplay as possible. Written in multiple languages, for each supported DB.

## Summary
This is part of a bigger project, a set of tools that will allow to automate as much as possible of the Middara game experience.
This part will be multiple versions of the data load and configuration scripts the app will need to create its databases. The initial versions should handle either plain SQL scripts, and/or loading from JSON files.

## The Companion App
The general idea of the over-project is to have a companion app for Middara gameplay.
It will, at some point, offer multiple functionalities for setting up a game session, automating said session gameplay, saving the game state between sessions, checking rules references on need, facilitate market/loot/discipline handling, etc.
The aim is to be able to use this app on multiple platforms.

### Why?
Since I got my KS copy of Middara - Act 1, all the way back in 2019, I've played the campaign with three different groups. All three of them have been unable to meet at my home, so I've been forced to lug the game around (without a car, mind you).
As such, I first started to read ahead on adventures (and thus spoil myself early) just to be able to take only what I needed for each session.

The first iteration of a helper app (back then we still had the promise of an official app) was for me to be able to select the range of game we'd play, and get back a list of everything I would need. I scrapped that idea after the first group stopped playing at the end of Chapter 1.

Over the years, I've come back to this idea, with more features I'd like to have on hand, as my playthroughs advanced and I found some automatable part that was annoying to do "by hand".

With the death of the official app announced, and a new group of players interested in going through the whole campaign, I find myself once more firing the cylinders up for this.

## Goals
I want to eventually build a complete interactive frontend, in Java, which will be able to handle al the functionalities of the underlying engine. Most of them won't see the light of day for a while.

### Must Haves
- Virtual Campaign Book:
  - Allow a user to navigate through a virtual Campaign Book
  - For each story section, give all the details in the book: text, tips, options, etc
  - For each encounter in the book, give all the diagrams, details, rules, victory/fail conditions, etc

### Want to Have
- Virtual Campaign Book:
  - Dynamically update an encounter when events are triggered: Totems, Objectives, Loot, Victory/Fail, Defeated Combatants/Characters, etc
  - Keep track of the party state throughout a single (or multiple) playthorughs: characters, equipment, disciplines, loot, flags, encounters, etc
- Interactive Rules Reference:
  - Allow a user to navigate the complete rulebook
  - Allow for easy reference/search of specific rules, tags, keywords, etc
- Card Album:
  - Searchable database of cards, with categories for Characters, Companions, Combatants, Disciplines, Loot, Equipment, etc
- Others:
  - Allow for i18n of the contents

### Would be Nice to Have
- Virtual Campaign Book:
  - Integrate with the rules references, to allow for quick access to rules in the middle of a playthrough, with easy naviagtion back to the current game section
- Interactive Rules Reference:
  - Keep the rulebook updated with the latest FAQs and BGG QAs for quick clarifications
  - Allow a user to select which rules version they're playing under
- Others:
  - Add modules for handling Crawl Books and Bounties

### Future Dreams
- Automated Playthrough AI:
  - On playthroughs, model the encounter maps **and** the Combatants AI steps, to allow for a simple AI that will automate the play experience
- Others:
  - Implement some integrated tool that allows to build some simple custom campaigns. This one would just leverage the (by then) existing engine for the official campaigns, and add API/Services that would allow to write up new encounters and story sections

My aim, ultimately, is to be able to handle every single aspect of a campaign, plus every session, automatically. This way, players would just need to sit around the table, set up whatever the game tells them to, and play the game.

## State
### Current Version
- v0.1: SQL Scripts for loading the initial DOM objects.

### Upcoming Versions
- v0.2: TBD

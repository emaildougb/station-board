# NCEMS Station Board

A browser-based crew bulletin board for North Country EMS. It shows the crew schedule, training and events, daily tasks, equipment checks, and station information on wall displays and crew devices.

## Status

This repo holds the front-end prototype only. It shows demo data. The live board will be served through a Cloudflare Worker that requires Microsoft sign-in, so crew information is not published on the open web.

## Files

- `index.html`: the board prototype. It is one self-contained page with its styles and scripts inline.

## What is not in this repo

- No API keys, passwords, access codes, or tokens. Secrets are stored as encrypted settings on the Cloudflare Worker.
- No live schedule, personnel, or station data.

## Running the prototype

Open `index.html` in a browser. It works without a server and uses demo data.

## Planned pieces

- A Cloudflare Worker that checks Microsoft sign-in and returns only the data each screen needs.
- SharePoint lists on the CG Staff site for bulletin items, training and events, daily tasks, and station notes.
- Read-only connection to the crew schedule feed and the apparatus checker.

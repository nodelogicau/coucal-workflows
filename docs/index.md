# Coucou! Let's Collaborate.

Coucou is a work management tool designed for sharing and collaborative activities.

## Overview

Coucou is a standards-based platform built on support for open formats, in order to maximise interoperability with other tooling.
The UI consists of three primary panes, supporting navigation and filtering, creation and editing, and views.

## urls

- / - worspace overview/dashboard. include collections, filters, members, etc
- /`<collection>` - list objects in a collection. apply filters, sorting, etc.
- /`<collection>`/`<uid>` - show object details using template for object type.
- /`<collection>`/`<uid>`/edit - form for editing object fields
- /`<collection>`/new - create a new object using creation form

## Commmon Functions

The following areas are common to all URLs.

## Workspace Explorer

Navigate folders and collections within a workspace. Selection of a collection triggers populating
the view area. Selection of folders/collections also enables applicable actions.

## Action Bar

Contextual actions enabled based on the current view.

Folder actions:
- Create folder
- Create collection
- Rename folder
- Delete folder

Collection actions:
- Create object
- Rename collection
- Delete collection

Object actions:
- Create linked object
- Delete object


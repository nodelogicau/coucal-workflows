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

## cookies

- current workspace
- collection view
- filter view
- object view

## Commmon Functions

The following areas are common to all URLs.

## Workspace Explorer

Switch between Workspaces. configure workspace options.

Navigate folders and collections within a workspace. Selection of a collection triggers
populating the view area. Selection of folders/collections also enables applicable actions.

Also navigate between filters in a workspace. Filter selection triggers population of the view area with filter results.

## Action Bar

Contextual actions enabled based on the current view.

### Folder actions

- Create folder
- Create collection
- Create filter
- Rename folder
- Delete folder

### Collection actions

- Create object
- Rename collection
- Delete collection
- Switch collection view
- Save as filter

### Filter actions

- Edit filter
- Rename filter
- Delete filter
- Switch filter view

### Object actions

- Create linked object
- Delete object
- Switch object view

## View Area

Show views of workspaces, collections and objects.

### Workspace Overview

Shown when no collection is selected. This view lists all collections in the current workspace, along with
relevant details such as object count, supported object types, default timezone, etc.

Also list filters in the current workspace with relevant details (e.g. object count).

### Workspace Options View

configure workspace options for current workspace. 

- members, control who has access to the workspace
- roles, manage fine-grained permissions
- channels, configure integrations such as email, websub, xmpp, etc.
- workflows, automated actions triggered by events
- api tokens, for service integration with coucal apis

### Collection Views

Shown when a collection is selected in the Workspace Explorer. Different views may be selected for each collection.

Available views include:
- Object list, showing a list of all objects using relevant property values (e.g. summary, dtstart, dtend, organizer, etc.).
Supports column sorting, filtering, paging, etc.
- Object graph, renders relationships between objects in a directed graph view.
- Status board, shows columns and swimlanes based on object status, assignee, etc.
- Information Charts, graphically plot objects based on multi-dimensional properties
- Calendar view, grid layout of objects based on time

### Object View

Use available templates to render object details. Templates can range from generic (VEVENT, VTODO, VJOURNAL, VCARD, VAVAILABILITY, etc.)
to specific (meeting, agenda, action, note, issue, risk, decision, etc.).

Some Object Views may also render details on linked objects, such as where there is a parent/child relationship. Such views include
Epic, Milestone, Feature, Objective, Initiative, etc.

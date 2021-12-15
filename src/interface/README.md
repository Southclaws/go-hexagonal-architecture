# interface

This directory contains non business logic components for interacting with the system. These are the left-most items on the typical hexagonal architecture diagram.

Typically this may be a HTTP API, GraphQL, CLI, anything where external input is triggering business logic.

This package should not be imported by any other part of the app (except at the top level where your app is all tied together, aka `main`), it's effectively the entry point for users or other apps.

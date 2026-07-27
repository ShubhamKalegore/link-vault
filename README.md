# LinkVault (Working Name)

> Save copied links instantly into organized collections with rich
> previews.

## Overview

LinkVault is an Android productivity application designed to eliminate
the repetitive workflow of copying links and sending them to yourself on
WhatsApp or another notes app.

The idea originated from a real-world problem:

Current workflow: 1. Copy a Facebook/Instagram/YouTube link. 2. Leave
the current app. 3. Open WhatsApp. 4. Open the "Message Yourself" chat.
5. Paste the link. 6. Wait for the preview to load. 7. Go back to the
original app. 8. Repeat for every link.

With LinkVault:

1.  Copy a link.
2.  A small floating bubble appears.
3.  Tap the bubble.
4.  Choose a collection.
5.  Continue browsing.

No app switching. No waiting for previews.

------------------------------------------------------------------------

# Problem Statement

People frequently save: - Facebook reels - Instagram reels - YouTube
videos - Articles - Shopping products - AI resources - Recipes

Most users currently: - Send links to themselves on WhatsApp - Store
links in Notes - Lose links in clipboard history

There is no simple workflow dedicated to organizing copied links
instantly.

------------------------------------------------------------------------

# Proposed Solution

Create an Android application that:

-   Detects copied URLs
-   Displays a floating bubble
-   Lets the user choose where to save the link
-   Stores links into organized collections
-   Generates rich previews
-   Provides fast search

------------------------------------------------------------------------

# Core Features

## Floating Bubble

When a copied item is detected as a URL:

-   Show a small floating bubble for a few seconds.
-   Ignore normal text copied by the user.
-   Tapping the bubble opens a save dialog.

------------------------------------------------------------------------

## Collections

Examples:

-   Workout
-   Songs
-   AI
-   Shopping
-   Travel
-   Recipes
-   Read Later

Users can:

-   Create new collections
-   Rename collections
-   Delete collections
-   Move links between collections

------------------------------------------------------------------------

## Rich Link Preview

Each saved URL should display:

-   Thumbnail
-   Title
-   Description
-   Website name
-   Original URL

Similar to WhatsApp link previews.

------------------------------------------------------------------------

## Search

Search across:

-   Titles
-   URLs
-   Website names
-   Collections

------------------------------------------------------------------------

## Favorites

Allow important links to be marked as favorites.

------------------------------------------------------------------------

## Tags

Examples:

-   Gym
-   Coding
-   Azure
-   Music
-   Motivation

------------------------------------------------------------------------

## Recent Links

Display recently saved items.

------------------------------------------------------------------------

## Optional Cloud Sync

Future enhancement:

-   Firebase
-   Own backend
-   Google account login

------------------------------------------------------------------------

# Saving Methods

## Method 1 (Primary)

Accessibility Service

Flow:

Copy URL → Floating Bubble → Select Collection → Save

Pros: - Fast - Minimal interruption - No app switching

Cons: - Requires Accessibility permission - Google Play reviews
accessibility usage carefully

------------------------------------------------------------------------

## Method 2 (Fallback)

Android Share Menu

Flow:

Share → Select LinkVault → Small bottom sheet → Choose collection → Save
→ Return to source app

Pros: - No clipboard monitoring - Official Android mechanism - Play
Store friendly

------------------------------------------------------------------------

# User Experience

Bubble appears only for URLs.

If ignored:

-   Automatically disappears after a few seconds.

No popup for:

-   OTPs
-   Phone numbers
-   Addresses
-   Random copied text

------------------------------------------------------------------------

# Future Smart Features

## Batch Save

Example:

User copies five links.

Instead of five dialogs:

"5 links copied"

Tap to organize all together.

------------------------------------------------------------------------

## AI Features

Potential additions:

-   Auto categorization
-   Duplicate detection
-   Summary generation
-   Suggested tags

------------------------------------------------------------------------

# Technical Stack

Language: - Kotlin (recommended)

Architecture: - MVVM

UI: - Jetpack Compose

Dependency Injection: - Hilt

Database: - Room

Async: - Kotlin Coroutines + Flow

Image Loading: - Coil

Networking: - Retrofit + OkHttp

Background: - Accessibility Service - Foreground Service (if required)

Overlay: - Display over other apps

------------------------------------------------------------------------

# Permissions

-   Accessibility Service
-   Display over other apps
-   Internet (for fetching metadata)

------------------------------------------------------------------------

# Play Store Considerations

Accessibility usage must:

-   Provide clear user benefit
-   Be optional
-   Be explained during onboarding
-   Not collect unnecessary personal information

Include:

-   Privacy Policy
-   Permission explanations
-   Ability to disable the feature

------------------------------------------------------------------------

# Target Audience

-   Students
-   Developers
-   Fitness enthusiasts
-   Researchers
-   Content creators
-   Anyone who saves many links

------------------------------------------------------------------------

# MVP

-   Floating bubble
-   Save to collections
-   Create new collection
-   Rich previews
-   Local storage
-   Search

------------------------------------------------------------------------

# Version 2

-   Cloud sync
-   Favorites
-   Tags
-   Batch save
-   AI categorization
-   Export/Import
-   Widget
-   Backup & Restore

------------------------------------------------------------------------

# Possible Names

-   LinkVault
-   LinkNest
-   LinkShelf
-   SaveBubble
-   LinkDrop
-   QuickSave Links
-   ReelVault
-   PocketLinks

------------------------------------------------------------------------

# Vision

Build the fastest way to save interesting links without leaving the app
you're currently using.

The goal is not to become another clipboard manager, but a personal
library for videos, articles, products, and resources that users
discover throughout the day.

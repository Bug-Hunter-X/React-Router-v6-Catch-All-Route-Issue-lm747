# React Router v6 Catch-All Route Issue

This repository demonstrates a problem with React Router v6's catch-all route (`*`).  The wildcard route is unexpectedly interfering with the matching of other routes.

## Problem

The `/` and `/about` routes work correctly, but the catch-all route (`*`) seems to always be selected first, even when a path matches `/` or `/about`.

## Solution

The order of routes matters. Place the catch-all route last in your `Routes` component to ensure it only matches when no other route matches.
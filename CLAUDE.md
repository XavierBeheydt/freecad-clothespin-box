# AI Instructions

This file provides guidance to AI coding agents (Claude Code, and other
agents reading it via the `AGENTS.md` symlink) when working in this
repository.

## Project overview

This is a personal FreeCAD modeling project, not a software project — there
is no build, lint, or test tooling. The goal is to design a 3D-printable
clothespin box: an open basket with a pair of clips on the back so it can
hang directly on a clothesline, as described in [README.md](README.md).

## Repository structure

- `cad/` — FreeCAD source file (`.FCStd`).
- `exports/` — 3MF exports for slicing and printing (full assembly, and
  each part separately).
- `images/` — renders and slicer screenshots.

## Language

Write everything in this repository — README, commit messages, code
comments, docs — in English only. Conversation with the user can be in
whichever language they use.

## Working with the FreeCAD file

- `.FCBak` backup files and the `backup/` directory are gitignored — never
  commit them.
- The `.FCStd` file is a binary FreeCAD document; it can't be reviewed as a
  text diff, so describe what changed in the commit message instead.

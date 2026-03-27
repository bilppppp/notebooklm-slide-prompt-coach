# Preferences

This skill may use lightweight saved preferences, but preferences are optional and never blocking.

## Purpose

Use saved preferences to reduce repeated setup for users who often want the same defaults.

Good preference examples:

- preferred output language
- preferred output format (`yaml` or `plain`)
- usual audience type
- usual tone
- usual brand colors
- usual bias such as `more restrained`, `more editorial`, `more technical`

## Priority

Use this order:

1. current user request
2. reference images and current materials
3. saved preferences
4. built-in defaults

Saved preferences should never override an explicit current request.

## Suggested EXTEND.md Shape

If the user ever wants persistent defaults, a simple file like this is enough:

```md
output_language: zh-CN
output_format: yaml
default_mode: normal
audience_bias: business
tone_bias: restrained, premium, clear
brand_colors:
  - deep navy
  - white
  - muted cyan
```

## How to Use

When a preference file exists:

- treat it as a soft default
- do not announce it every time
- mention it briefly only when relevant, for example:
  - "我先沿用你平时偏克制、偏商务的默认习惯来出。"

When no preference file exists:

- continue normally
- do not stop to ask for setup

## What Not to Store

Avoid storing narrow project-specific decisions such as:

- one-off campaign slogans
- one specific deck topic
- temporary seasonal themes

The file should capture stable preferences, not past tasks.

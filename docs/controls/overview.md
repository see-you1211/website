---
title: Overview
sidebar_label: Overview
slug: /controls
---

Flet UI is built of controls. Most controls are composed from multiple HTML elements, have finished functionality and sane defaults to make UI development as quick and pleasant as possible. For example, [Textbox](controls/textbox) control is not just `<input type="text">` in terms of HTML, but it has an attached label, description, validation message and a help tip.

Controls are organized into hierarchy, or a tree, where each control has a parent (except [Page](controls/page)) and container controls like [Stack](controls/stack), [Dropdown](controls/dropdown) can contain child controls, for example:

```
Page
 ├─ Textbox
 ├─ Dropdown
 │   ├─ Option
 │   └─ Option
 └─ Stack
     ├─ Button
     └─ Button
```

## Common properties

All Flet controls have the following properties:

| Name       | Type      | Default       | Description |
| ---------- | --------- | ------------- | ----------- |
| `id`       | string    |               | Auto-generated or user-defined control ID.    |
| `visible`  | bool      | `true`        | Defines whether control is visible. |
| `disabled` | bool      | `false`       | Defines whether control and all its children (if any) are disabled. |
| `width`    | string    |               | Width of the control, for example `100px`, `50%`.    |
| `height`   | string    |               | Height of the control.    |
| `padding`  | string    |               | Padding of the control.    |
| `margin`   | string    |               | Margin of the control.    |
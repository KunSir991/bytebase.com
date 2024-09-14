---
title: Bytebase 2.22.3
author: Ningjing
updated_at: 2024/9/5 17:00:00
feature_image: /content/changelog/2-22-3-banner.webp
description: 'One-click rollback for PostgreSQL DML change'
---

## 🚀 New Features

- [One-click rollback](/docs/change-database/rollback-data-changes/#1-click-rollback) for PostgreSQL DML change.

## 🎄 Enhancements

- Enhance DML Backup and Restore Experience:
  - Guide users to create the `bbdataarchive` database. Prior backup cannot be enabled if this database doesn't exist.
  - Allow users to enable or disable the backup option after an issue is created.
  - For unsupported backup scenarios, an error will be reported when turning on the backup switch.
  - Support MySQL generated columns.
  - Bulk `UPDATE` statements to a single table will be backed up into a single table. Before, each `UPDATE` statement will be backed up into a separate table.
- Enhance SQL Editor sidebar:
  - Display column types and nullable information.
  - Show columns and dependent columns in views.
- Under the **Issued Created** tab, add an **All** sub-tab.
- Enable i18n support for auto-generated issue titles.
- Add a project setting to require manually entering issue titles instead of using Bytebase’s auto-generated titles.

<IncludeBlock url="/docs/get-started/install/install-upgrade"></IncludeBlock>
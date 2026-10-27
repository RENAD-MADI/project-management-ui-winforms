# Project Management — WinForms UI Prototype

<div dir="rtl">

نموذج واجهة لنظام إدارة مشاريع بـ Windows Forms: المشاريع، فريق العمل، المتعاونين، أوامر العمل، المواد، المعدات، وحالة الجدولة. **واجهة فقط** بدون منطق أو قاعدة بيانات.

</div>

A Windows Forms UI prototype for a project-management tool (Arabic, right-to-left). The main window lays out navigation for projects, the team, collaborators, work orders, materials and equipment, plus a scheduling-status panel.

> Status: **UI only.** The buttons are not wired to any logic or data yet.

![.NET](https://img.shields.io/badge/.NET-8-512BD4?logo=dotnet)
![WinForms](https://img.shields.io/badge/Windows_Forms-0078D4?logo=windows&logoColor=white)

## Run it

Requirements: Windows and the .NET 8 SDK.

```bash
dotnet run
```

## Structure

```
Program.cs          Entry point
PL/FRM_MIAN.cs      Main form (presentation layer)
Resources/          Icons
```

## Changes

- `Program.cs` started a `Form1` that does not exist, so the project did not build. It now opens the main form.
- Retargeted from .NET 6 (out of support) to .NET 8; removed empty `BL` and `DAL` folders.

## Next steps

Add a data layer (EF Core + SQLite) and connect each button to its screen: projects, team, work orders, materials, equipment and schedule status.

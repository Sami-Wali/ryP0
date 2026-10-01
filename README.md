
86 downloads is that real?

Worked for 30s
إيه، الـ86 حقيقية كرقم من GitHub نفسه. شيكت مباشرة على Release الخاصة بـ ryP0 v1.0، وGitHub API يرجّع للملف:

ryP0-unsigned.ipa → download_count: 86

يعني الرقم مو شيء الـbadge اخترعه؛ الـbadge فقط يقرأ عداد GitHub الرسمي. GitHub أصلًا يوفر download_count لكل Release Asset في الـAPI. 

لكن انتبه للنقطة المهمة: 86 downloads ≠ 86 شخص مختلف. هو عدد تنزيلات ملف الـIPA، وليس إحصائية unique users. يعني لا تكتب مثلًا “86 users”؛ اكتب “86 downloads” فقط.

وعندك حاليًا Release واحدة وAsset واحد فقط، لذلك Badge الـDownloads عندك فعليًا يعكس تنزيلات ryP0-unsigned.ipa مباشرة.

فتح ryP0 Releases

وبصراحة 86 تنزيل خلال حوالي 10 أيام لمشروع صغير ولسه الصفحة نفسها شبه فاضية رقم كويس جدًا.

عدل بان ينصح بمستخدمين لايف كونتينر بتحويله لتطبيق مشارك حتى تقدر تستخدمه في لايف كونتينر ٢ لتستطيع تحميل التطبيقات مباشرة في لايف ١ 
وابغا اضيف ذا https://altdirect.app/


Worked for 17s
أكيد. الأفضل نخليها واضحة كـ Recommended setup for LiveContainer ونضيف AltDirect كطريقة مباشرة لفتح مصدر ryP0.

حسب توثيق LiveContainer، التطبيق لازم يكون Shared App حتى يشتغل من LiveContainer 2، ويتم التحويل من إعدادات التطبيق داخل LiveContainer الأساسي. 
 وAltDirect مصمم أصلًا لفتح AltSource في LiveContainer وغيره من الأدوات المدعومة. 

استبدل جزء Download / Get ryP0 بهذا:

## Get ryP0

Public ryP0 builds are available through GitHub Releases.

### Latest Release

[**Download the latest ryP0 release →**](https://github.com/Sami-Wali/ryP0/releases/latest)

You can also browse previous versions from the
[Releases](https://github.com/Sami-Wali/ryP0/releases) page.

---

## LiveContainer

ryP0 works especially well alongside LiveContainer.

> [!TIP]
> **Recommended for LiveContainer users**
>
> If you use multiple LiveContainers, convert **ryP0 to a Shared App**.
>
> This allows you to run ryP0 inside **LiveContainer 2** while keeping
> **LiveContainer 1** available for apps opened or downloaded through ryP0.
>
> In LiveContainer 1:
>
> 1. Long-press **ryP0**
> 2. Open **App Settings**
> 3. Select **Convert to Shared App**
> 4. Launch ryP0 using **LiveContainer 2**
>
> This setup lets you keep ryP0 open separately while sending supported
> downloads and actions back to your primary LiveContainer.

---

## Add the ryP0 Catalog

The ryP0 catalog can be opened using **AltDirect**.

### Open with AltDirect

[**Open ryP0 Catalog →**](https://altdirect.app/?url=https://raw.githubusercontent.com/Sami-Wali/ryP0-repository/main/repo.json)

AltDirect lets you open compatible sources directly in supported tools such as
LiveContainer, SideStore, AltStore, Feather, StikStore, and TrollApps.

You can also visit AltDirect directly:

[**altdirect.app →**](https://altdirect.app/)

### Raw Catalog

If you prefer to access the source manually:

[`repo.json`](https://raw.githubusercontent.com/Sami-Wali/ryP0-repository/main/repo.json)
وفي أعلى الـREADME، عند الأزرار، أعدلها إلى:

[**Get ryP0**](https://github.com/Sami-Wali/ryP0/releases/latest)
&nbsp;&nbsp;•&nbsp;&nbsp;
[**Open Catalog**](https://altdirect.app/?url=https://raw.githubusercontent.com/Sami-Wali/ryP0-repository/main/repo.json)
&nbsp;&nbsp;•&nbsp;&nbsp;
[**Releases**](https://github.com/Sami-Wali/ryP0/releases)
وأنا أفضل Open Catalog بدل Catalog Source؛ للمستخدم العادي أوضح بكثير، ويوديه مباشرة إلى AltDirect بدل ما يفتح JSON خام.

اعطني الملف كامل

Worked for 21s
هذا هو README.md كامل بعد تعديل قسم LiveContainer وإضافة AltDirect، وبنفس التوجه بدون استخدام كلمة App Store:

<div align="center">

<br>

<img src="assets/icon.png" width="120" height="120" alt="ryP0">

# ryP0

### Discover beyond the usual.

A clean catalog for discovering independent iOS software,  
community releases, projects, and sources.

<br>

[![Latest Release](https://img.shields.io/github/v/release/Sami-Wali/ryP0?style=for-the-badge&label=Release)](https://github.com/Sami-Wali/ryP0/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/Sami-Wali/ryP0/total?style=for-the-badge&label=Downloads)](https://github.com/Sami-Wali/ryP0/releases)
[![Platform](https://img.shields.io/badge/Platform-iOS-black?style=for-the-badge)](#compatibility)

<br>

[**Get ryP0**](https://github.com/Sami-Wali/ryP0/releases/latest)
&nbsp;&nbsp;•&nbsp;&nbsp;
[**Open Catalog**](https://altdirect.app/)
&nbsp;&nbsp;•&nbsp;&nbsp;
[**Releases**](https://github.com/Sami-Wali/ryP0/releases)

<br><br>

</div>

---

<p align="center">
  <img src="assets/banner.png" width="100%" alt="ryP0 Banner">
</p>

---

## Explore differently

ryP0 brings independent iOS software, projects, releases, and sources together in one simple interface.

Instead of searching through different repositories and release pages manually, ryP0 organizes available software into a clean and accessible catalog.

It is designed around simplicity, transparency, and direct access to original sources.

---

## What is ryP0?

ryP0 is a catalog-based platform for exploring software distributed through independent sources.

Each entry can include information such as:

- Name and icon
- Version
- Description
- Developer
- Release information
- Source
- Download availability
- Update information

ryP0 keeps everything organized while preserving direct access to the original project or distribution source.

---

## Preview

<p align="center">
  <img src="assets/screenshot-1.png" width="30%" alt="ryP0 Preview 1">
  &nbsp;
  <img src="assets/screenshot-2.png" width="30%" alt="ryP0 Preview 2">
  &nbsp;
  <img src="assets/screenshot-3.png" width="30%" alt="ryP0 Preview 3">
</p>

---

## Discover

Explore software from different independent sources through one organized catalog.

Find new projects, view release information, check available versions, and access original sources without jumping between multiple repositories.

---

## Sources first

ryP0 is built around publicly available project information and release sources.

Where available, entries can provide direct access to:

- Original developer
- Project repository
- Release page
- Distribution source
- Version history

This keeps the experience transparent and makes it easy to understand where each release comes from.

---

## Releases

Public ryP0 builds are distributed through GitHub Releases.

### Latest release

[**Get the latest ryP0 release →**](https://github.com/Sami-Wali/ryP0/releases/latest)

Previous versions can be found on the:

[**ryP0 Releases page →**](https://github.com/Sami-Wali/ryP0/releases)

---

## LiveContainer

ryP0 can be used alongside LiveContainer for a smoother workflow.

> [!TIP]
> ### Recommended setup for LiveContainer users
>
> If you use **LiveContainer 1 and LiveContainer 2**, it is recommended to convert **ryP0 into a Shared App**.
>
> This allows you to run **ryP0 inside LiveContainer 2** while keeping **LiveContainer 1** available as your primary container.
>
> With this setup, ryP0 can remain open in LiveContainer 2 while compatible software can be sent to or opened with LiveContainer 1.

### Setup

In your primary LiveContainer:

1. Find **ryP0**
2. Open its app settings
3. Choose **Convert to Shared App**
4. Open **LiveContainer 2**
5. Launch the shared ryP0 instance from LiveContainer 2

You can then use ryP0 from LiveContainer 2 while keeping LiveContainer 1 available for compatible downloads and launches.

> [!NOTE]
> Exact behavior may depend on your LiveContainer version and configuration.

---

## Catalog

ryP0 uses a structured public catalog to retrieve software metadata, versions, releases, and source information.

### Catalog URL

```text
https://raw.githubusercontent.com/Sami-Wali/ryP0-repository/main/repo.json
View raw catalog →

Catalog information may include:

Name
Identifier
Developer
Description
Version
Icon
Source
Release URL
Metadata
AltDirect
Want to open the ryP0 catalog with a compatible tool?

Use AltDirect:

Open AltDirect →
Then use the ryP0 catalog URL:

https://raw.githubusercontent.com/Sami-Wali/ryP0-repository/main/repo.json
AltDirect provides a simple way to open compatible sources with supported iOS tools.

Compatibility
ryP0 is designed for:

iPhone
iPad
iOS
iPadOS
Compatibility can vary depending on:

ryP0 version
iOS version
Selected software
Distribution method
LiveContainer configuration
Updates
The ryP0 catalog can be updated independently from the ryP0 client.

This allows new:

Projects
Versions
Releases
Icons
Metadata
Sources
to appear without requiring a new ryP0 build every time the catalog changes.

Public distribution
This repository is the public home of ryP0 releases and distribution resources.

It contains files and information intended for public use.

Internal development resources, private source code, credentials, signing material, and automation infrastructure are not distributed through this repository.

Independence
ryP0 is an independent project.

Software accessible through ryP0 remains the responsibility of its respective developer or distributor.

Names, trademarks, icons, software, and other assets belong to their respective owners.

ryP0 does not claim ownership of third-party projects listed in the catalog.

Disclaimer
ryP0 provides an organized interface for accessing project information and publicly available release sources.

Availability, compatibility, functionality, and authenticity of third-party software may vary depending on its respective developer or source.

Users should review the original project and source information before using third-party software.

ryP0 is an independent project and is not affiliated with or endorsed by Apple Inc.

<div align="center">
ryP0
Discover. Explore. Get.
Independent software.
Original sources.
One clean catalog.


Get ryP0
  •  
AltDirect
  •  
Catalog
  •  
Releases




<sub>ryP0 is an independent project and is not affiliated with Apple Inc.</sub>




</div> ```
وتأكد أن هذه الملفات موجودة عندك عشان الـREADME ما يظهر فيه صور مكسورة:

assets/
├── icon.png
├── banner.png
├── screenshot-1.png
├── screenshot-2.png
└── screenshot-3.png
رابط repo.json الموجود فوق صحيح وموجود فعلًا في Sami-Wali/ryP0-repository.

give me full markdown file

Download the full README.md
 


README.md
Document



<div align="center">
<img src="assets/icon.png" width="120" height="120" alt="ryP0">
ryP0
Discover beyond the usual.
A clean catalog for discovering independent iOS software,
community releases, projects, and sources.







Get ryP0
  •  
Open Catalog
  •  
Releases




</div>
<p align="center"> <img src="assets/banner.png" width="100%" alt="ryP0 Banner"> </p>
Explore differently
ryP0 brings independent iOS software, projects, releases, and sources together in one simple interface.

Instead of searching through different repositories and release pages manually, ryP0 organizes available software into a clean and accessible catalog.

It is designed around simplicity, transparency, and direct access to original sources.

What is ryP0?
ryP0 is a catalog-based platform for exploring software distributed through independent sources.

Each entry can include information such as:

Name and icon
Version
Description
Developer
Release information
Source
Download availability
Update information
ryP0 keeps everything organized while preserving direct access to the original project or distribution source.

Preview
<p align="center"> <img src="assets/screenshot-1.png" width="30%" alt="ryP0 Preview 1"> &nbsp; <img src="assets/screenshot-2.png" width="30%" alt="ryP0 Preview 2"> &nbsp; <img src="assets/screenshot-3.png" width="30%" alt="ryP0 Preview 3"> </p>
Discover
Explore software from different independent sources through one organized catalog.

Find new projects, view release information, check available versions, and access original sources without jumping between multiple repositories.

Sources first
ryP0 is built around publicly available project information and release sources.

Where available, entries can provide direct access to:

Original developer
Project repository
Release page
Distribution source
Version history
This keeps the experience transparent and makes it easy to understand where each release comes from.

Releases
Public ryP0 builds are distributed through GitHub Releases.

Latest release
Get the latest ryP0 release →

Previous versions can be found on the:

ryP0 Releases page →

LiveContainer
ryP0 can be used alongside LiveContainer for a smoother workflow.

[!TIP]

Recommended setup for LiveContainer users
If you use LiveContainer 1 and LiveContainer 2, it is recommended to convert ryP0 into a Shared App.

This allows you to run ryP0 inside LiveContainer 2 while keeping LiveContainer 1 available as your primary container.

With this setup, ryP0 can remain open in LiveContainer 2 while compatible software can be sent to or opened with LiveContainer 1.

Setup
In your primary LiveContainer:

Find ryP0
Open its app settings
Choose Convert to Shared App
Open LiveContainer 2
Launch the shared ryP0 instance from LiveContainer 2
You can then use ryP0 from LiveContainer 2 while keeping LiveContainer 1 available for compatible downloads and launches.

[!NOTE]
Exact behavior may depend on your LiveContainer version and configuration.

Catalog
ryP0 uses a structured public catalog to retrieve software metadata, versions, releases, and source information.

Catalog URL
https://raw.githubusercontent.com/Sami-Wali/ryP0-repository/main/repo.json
View raw catalog →

Catalog information may include:

Name
Identifier
Developer
Description
Version
Icon
Source
Release URL
Metadata
AltDirect
Want to open the ryP0 catalog with a compatible tool?

Use AltDirect:

Open AltDirect →
Then use the ryP0 catalog URL:

https://raw.githubusercontent.com/Sami-Wali/ryP0-repository/main/repo.json
AltDirect provides a simple way to open compatible sources with supported iOS tools.

Compatibility
ryP0 is designed for:

iPhone
iPad
iOS
iPadOS
Compatibility can vary depending on:

ryP0 version
iOS version
Selected software
Distribution method
LiveContainer configuration
Updates
The ryP0 catalog can be updated independently from the ryP0 client.

This allows new:

Projects
Versions
Releases
Icons
Metadata
Sources
to appear without requiring a new ryP0 build every time the catalog changes.

Public distribution
This repository is the public home of ryP0 releases and distribution resources.

It contains files and information intended for public use.

Internal development resources, private source code, credentials, signing material, and automation infrastructure are not distributed through this repository.

Independence
ryP0 is an independent project.

Software accessible through ryP0 remains the responsibility of its respective developer or distributor.

Names, trademarks, icons, software, and other assets belong to their respective owners.

ryP0 does not claim ownership of third-party projects listed in the catalog.

Disclaimer
ryP0 provides an organized interface for accessing project information and publicly available release sources.

Availability, compatibility, functionality, and authenticity of third-party software may vary depending on its respective developer or source.

Users should review the original project and source information before using third-party software.

ryP0 is an independent project and is not affiliated with or endorsed by Apple Inc.

<div align="center">
ryP0
Discover. Explore. Get.
Independent software.
Original sources.
One clean catalog.


Get ryP0
  •  
AltDirect
  •  
Catalog
  •  
Releases




<sub>ryP0 is an independent project and is not affiliated with Apple Inc.</sub>




</div>

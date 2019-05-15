---
author: daspek
ms.author: dspektor
title: Тип ресурса versionAction
description: Объект VersionAction предоставляет сведения о действии, которое привело к созданию новой версии элемента.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 0d05ad93c59ba736dd90276fc5e3db6e05740344
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970793"
---
# <a name="versionaction-resource-type"></a>Тип ресурса versionAction

Присутствие ресурса **versionAction** в [**itemActivity**] [ activity] указывает на то, что действие привело к созданию новой версии.

>**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.

[activity]: itemactivity.md

## <a name="properties"></a>Свойства

| Имя свойства | Тип   | Описание
|:--------------|:-------|:----------------------------------------------------
| newVersion    | string | Имя новой версии, созданной при выполнении этого действия.

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.versionAction"
}-->

```json
{
  "newVersion": "string"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The VersionAction object provides information about an activity that resulted in a new item version.",
  "keywords": "activities,activity,action,version",
  "section": "documentation",
  "tocPath": "Resources/VersionAction",
  "suppressions": []
}
-->

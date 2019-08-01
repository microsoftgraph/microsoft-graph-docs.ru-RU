---
author: daspek
ms.author: dspektor
title: Тип ресурса versionAction
description: Объект VersionAction предоставляет сведения о действии, которое привело к созданию новой версии элемента.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 22f06691824d2ffa5b773a796b4c456cb2fcaecc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033448"
---
# <a name="versionaction-resource-type"></a>Тип ресурса versionAction

Присутствие ресурса **versionAction** в [**itemActivity**][activity] указывает на то, что действие привело к созданию новой версии.

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

---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: contentTypeOrder
localization_priority: Normal
ms.openlocfilehash: 9b92a8234c493ae9b0f396db7010e7bf717d5959
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514371"
---
# <a name="contenttypeorder-resource-type"></a>Тип ресурса contentTypeOrder

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **contentTypeOrder** указывает, в каком порядке тип контента будет отображаться в пользовательском интерфейсе выбора.

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса **contentTypeOrder** в формате JSON.
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a>Свойства

| Имя свойства | Тип    | Описание
|:--------------|:--------|:----------------------------------------------------
| **default**   | boolean | Указывает, используется ли этот тип контента по умолчанию.
| **position**  | Int32   | Указывает позицию, в которой тип контента отображается в пользовательском интерфейсе выбора.

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder",
  "suppressions": [
    "Error: /api-reference/beta/resources/contentTypeOrder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

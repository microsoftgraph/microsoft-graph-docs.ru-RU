---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e7bbd0f6aa8d4ea04304d6aecae97b98ab0a46b7
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574280"
---
# <a name="webpart-resource"></a>веб-часть ресурсов

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Тип и отображение сведений о веб-части на [sitePage](sitepage.md)представляет ресурс **веб-части** .

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [  
    ],
  "@odata.type": "microsoft.graph.webPart"
}-->

```json
{
  "type": "String (identifier)",
  "data": {
    "instanceId": "string (guid) (optional)"
  }
}
```

## <a name="properties"></a>Свойства

| Свойство                | Тип             | Описание
|:------------------------|:-----------------|:----------------------------------
| **type**                | String (идентификатор)         | Уникальный идентификатор, определяющий тип веб-части. Только для чтения.
| **data**                | [sitePageData](sitepagedata.md) | Обязательные свойства для веб-части (зависит от веб-части)

[sitePageData]: sitepagedata.md

## <a name="remarks"></a>Замечания

Веб-части можно определить собственные необходимые свойства в области **данных**.

Дополнительные сведения о страницах можно [sitePage](sitepage.md).
<!--
{
  "type": "#page.annotation",
  "description": "Defines a control resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Control",
  "suppressions": [
    "Error: /api-reference/beta/resources/webpart.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

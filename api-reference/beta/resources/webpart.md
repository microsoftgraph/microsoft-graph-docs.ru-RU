---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9c019da7cb10a8c26faa8d338c54436043f83db8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453611"
---
# <a name="webpart-resource"></a>ресурс webPart

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **WebPart** представляет тип и сведения о визуализации веб-части в [ситепаже](sitepage.md).

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.webPart"
}-->

```json
{
  "type": "string (guid)",
  "data": {
    "instanceId": "string (guid) (optional)"
  }
}
```

## <a name="properties"></a>Свойства

| Свойство                | Тип             | Описание
|:------------------------|:-----------------|:----------------------------------
| **type**                | Строка           | Уникальный идентификатор, указывающий тип веб-части. Только для чтения.
| **data**                | [Ситепажедата][] | Обязательные свойства веб-части (зависит от веб-части)

[Ситепажедата]: sitepagedata.md

## <a name="remarks"></a>Комментарии

Веб-части могут определять собственные обязательные свойства в разделе **Data**.

Более подробную информацию о страницах можно узнать в статье [ситепаже](sitepage.md).
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

---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 03b5f1007d8dbe6587da736cdf0ac0fdc1ed8a55
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345795"
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
  "type": "string (identifier)",
  "data": {"@odata.type":"microsoft.graph.sitePageData"}
}
```

## <a name="properties"></a>Свойства

| Свойство                | Тип             | Описание
|:------------------------|:-----------------|:----------------------------------
| **type**                | String           | Уникальный идентификатор, указывающий тип веб-части. Только для чтения.
| **data**                | [Ситепажедата][] | Обязательные свойства веб-части (зависит от веб-части)

[Ситепажедата]: sitepagedata.md

## <a name="remarks"></a>Примечания

Веб-части могут определять собственные обязательные свойства в разделе **Data**.

Более подробную информацию о страницах можно узнать в статье [ситепаже](sitepage.md).
<!--
{
  "type": "#page.annotation",
  "description": "Defines a control resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Control",
  "suppressions": []
}
-->

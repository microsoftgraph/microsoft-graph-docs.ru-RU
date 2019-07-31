---
author: rahmit
description: Ресурс webPart представляет тип и сведения о визуализации веб-части в Ситепаже.
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 71626440abe9eb63af3419b3e65c4351ae442dea
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007356"
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

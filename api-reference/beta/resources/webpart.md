---
author: rahmit
description: Ресурс webPart представляет тип и сведения о визуализации веб-части в Ситепаже.
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: b69762298f4f165ac18e4e0137dd979bde176652
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973477"
---
# <a name="webpart-resource"></a>ресурс webPart

Пространство имен: microsoft.graph

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
| **data**                | [ситепажедата][] | Обязательные свойства веб-части (зависит от веб-части)

[ситепажедата]: sitepagedata.md

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



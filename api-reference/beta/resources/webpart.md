---
author: rahmit
description: Ресурс webPart представляет тип и сведения о визуализации веб-части в Ситепаже.
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: efcf6aa1db31246af607cda85aa799fcc6804a34
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519437"
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

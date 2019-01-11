---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.openlocfilehash: f7293b986b5e6d77d0601cffb6b60edc5dfd2dd7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856030"
---
# <a name="webpart-resource"></a>веб-часть ресурсов

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Тип и отображение сведений о веб-части на [sitePage](sitepage.md)представляет ресурс **веб-части** .

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
| **type**                | Строка           | Уникальный идентификатор, определяющий тип веб-части. Только для чтения.
| **data**                | [sitePageData][] | Обязательные свойства для веб-части (зависит от веб-части)

[sitePageData]: sitepagedata.md

## <a name="remarks"></a>Примечания

Веб-части можно определить собственные необходимые свойства в области **данных**.

Дополнительные сведения о страницах можно [sitePage](sitepage.md).
<!-- {
  "type": "#page.annotation",
  "description": "Defines a control resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Control"
} -->

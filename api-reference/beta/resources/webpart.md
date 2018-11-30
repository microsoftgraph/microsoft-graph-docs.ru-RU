---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
ms.openlocfilehash: e9bb612e20bc3d2416503f571f5abf364215efb2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077810"
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
| **type**                | String           | Уникальный идентификатор, определяющий тип веб-части. Только для чтения.
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

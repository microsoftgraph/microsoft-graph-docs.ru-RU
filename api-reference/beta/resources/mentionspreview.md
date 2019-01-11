---
title: Тип ресурса mentionsPreview
description: Представляет сведения об объектах упоминаются в экземпляре ресурсов.
localization_priority: Normal
ms.openlocfilehash: 1534b7f0ef48a80d0faaaa09880b91cb270e8eca
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826112"
---
# <a name="mentionspreview-resource-type"></a>Тип ресурса mentionsPreview

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет сведения о [упомянуть](../resources/mention.md) объекты в экземпляре ресурсов.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| isMentioned | Логический | Значение true, если пользователь выполнил вход упоминается в экземпляре ресурсов родительского. Только для чтения. Поддержка фильтра. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mentionsPreview"
}-->

```json
{
  "isMentioned": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mentionsPreview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

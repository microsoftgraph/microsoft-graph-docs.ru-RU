---
title: Тип ресурса Рекордоператион
description: Этот тип ресурса содержит сведения, связанные с записью звука.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 03cdf594b04c75cd14b31dfbaef5894e8aacd19d
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913669"
---
# <a name="recordoperation-resource-type"></a>Тип ресурса Рекордоператион

Этот тип ресурса содержит сведения, связанные с записью звука.

## <a name="properties"></a>Свойства

| Свойство                       | Тип                        | Описание                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| Контекст                  | String                      | Уникальная строка контекста клиента. Максимальный лимит — 256 символов.                                                                                                                               |
| id                             | Строка                      | Идентификатор операции сервера. Только для чтения.                                                                                              |
| рекордингакцесстокен           | String                      | Маркер доступа, необходимый для получения записи.                                                                                              |
| рекординглокатион              | String                      | Расположение, в котором находится запись.                                                                                                      |
| resultInfo                     | [resultInfo](resultinfo.md) | Сведения о результате.  Только для чтения.                                                                                              |
| status                         | String                      | Возможные значения: `notStarted`, `running`, `completed`, `failed`. Только для чтения.                                                |

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "recordingAccessToken": "String",
  "recordingLocation": "String",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recordOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

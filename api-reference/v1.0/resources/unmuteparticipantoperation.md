---
title: Тип ресурса УнмутепартиЦипантоператион
description: Описывает формат ответа для функции "без звука".
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4a3a4428f1c7be9a840b18625b788b26751eca57
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090636"
---
# <a name="unmuteparticipantoperation-resource-type"></a>Тип ресурса УнмутепартиЦипантоператион

Пространство имен: microsoft.graph

Описывает формат ответа для функции "без звука".

## <a name="properties"></a>Свойства

| Свойство                       | Тип                        | Описание                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| Контекст                  | Строка                      | Уникальная строка контекста клиента. Может содержать до 256 символов.                                                                               |
| id                             | Строка                      | ИДЕНТИФИКАТОР операции сервера. Только для чтения.                                                                                            |
| resultInfo                     | [resultInfo](resultinfo.md) | Сведения о результате.  Только для чтения.                                                                                            |
| status                         | String                      | Возможные значения: `notStarted`, `running`, `completed`, `failed`. Только для чтения.                                                 |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unmuteParticipantOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unmuteParticipantOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


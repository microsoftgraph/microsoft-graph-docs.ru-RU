---
title: тип ресурса updateRecordingStatusOperation
description: Описывает формат ответа действия записи обновления.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 1f377ac39ec8e216b883f644f086f888b025ef8c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59062413"
---
# <a name="updaterecordingstatusoperation-resource-type"></a>тип ресурса updateRecordingStatusOperation

Пространство имен: microsoft.graph

Описывает формат ответа действия записи обновления.

## <a name="properties"></a>Свойства

| Свойство            | Тип                        | Описание|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| clientContext       | String                      | Уникальная строка контекста клиента. Максимальное ограничение — 256 шаров.                              |
| id                  | String                      | Только для чтения.                                                                         |
| resultInfo          | [resultInfo](resultinfo.md) | Сведения о результате. Только для чтения.                                                 |
| status              | String                      | Возможные значения: `notStarted`, `running`, `completed`, `failed`.               |

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.updateRecordingStatusOperation"
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
<!--
{
  "type": "#page.annotation",
  "description": "updateRecordingStatusOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


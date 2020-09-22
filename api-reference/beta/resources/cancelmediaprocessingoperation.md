---
title: Тип ресурса Канцелмедиапроцессингоператион
description: Этот тип ресурса используется для описания формата ответа операции отмены обработки мультимедиа.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b1f74ba825bdd953803c3458882cbae051fae970
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042718"
---
# <a name="cancelmediaprocessingoperation-resource-type"></a>Тип ресурса Канцелмедиапроцессингоператион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает формат ответа для операции отмены обработки мультимедиа.

## <a name="properties"></a>Свойства

| Свойство                       | Тип                        | Описание                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| ко                            | Boolean                     | Указывает, следует ли остановить все операции или текущие.                                                                                    |
| Контекст                  | Строка                      | Контекст клиента.                                                                                                                               |
| id                             | Строка                      | ИДЕНТИФИКАТОР операции сервера. Только для чтения.                                                                                              |
| resultInfo                     | [resultInfo](resultinfo.md) | Сведения о результате.  Только для чтения.                                                                                              |
| status                         | String                      | Возможные значения: `notStarted`, `running`, `completed`, `failed`. Только для чтения.                                                  |

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cancelMediaProcessingOperation"
}-->
```json
{
  "all": true,
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
  "description": "cancelMediaProcessingOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



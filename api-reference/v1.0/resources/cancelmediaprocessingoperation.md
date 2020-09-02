---
title: Тип ресурса Канцелмедиапроцессингоператион
description: Этот тип ресурса используется для описания формата ответа операции отмены обработки мультимедиа.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5962b3f5aed89c7f2c0b01be3f8b4a035ac463da
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319622"
---
# <a name="cancelmediaprocessingoperation-resource-type"></a>Тип ресурса Канцелмедиапроцессингоператион

Пространство имен: microsoft.graph

Описывает формат ответа операции отмены обработки мультимедиа.

## <a name="properties"></a>Свойства

| Свойство      | Тип                        | Описание                                                                     |
| :------------ | :-------------------------- | :------------------------------------------------------------------------------ |
| ко           | Boolean                     | Указывает, следует ли остановить все операции или текущие.                            |
| Контекст | String                      | Контекст клиента.                                                             |
| id            | String                      | ИДЕНТИФИКАТОР операции сервера. Только для чтения.                                             |
| resultInfo    | [resultInfo](resultinfo.md) | Сведения о результате.  Только для чтения.                                             |
| status        | String                      | Возможные значения: `notStarted`, `running`, `completed`, `failed`. Только для чтения. |

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

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

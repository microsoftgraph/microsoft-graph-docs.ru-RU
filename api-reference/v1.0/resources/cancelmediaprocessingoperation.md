---
title: cancelMediaProcessingOperation type
description: Этот тип ресурса используется для описания формата ответа операции обработки мультимедиа отмены.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9b7cecdfbbb6ced93149740de89a18081a04cffa
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59078940"
---
# <a name="cancelmediaprocessingoperation-resource-type"></a>Тип ресурса CancelMediaProcessingOperation

Пространство имен: microsoft.graph

Описывает формат ответа операции отмены обработки мультимедиа.

## <a name="properties"></a>Свойства

| Свойство      | Тип                        | Описание                                                                     |
| :------------ | :-------------------------- | :------------------------------------------------------------------------------ |
| все           | Логический                     | Указывает, следует ли останавливать все операции или ток.                            |
| clientContext | String                      | Клиентский контекст.                                                             |
| id            | Строка                      | ID операции сервера. Только для чтения.                                             |
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


---
title: Тип ресурса recordOperation
description: Этот тип ресурса содержит сведения, связанные с аудиозаписью.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e655765044e7ed54746efda17e4e2e1c5129d0e6ca4bbf4a692d45817034f9f7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54202142"
---
# <a name="recordoperation-resource-type"></a>Тип ресурса recordOperation

Пространство имен: microsoft.graph

Этот тип ресурса содержит сведения, связанные с аудиозаписью.

## <a name="properties"></a>Свойства

| Свойство                       | Тип                        | Описание                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| clientContext                  | String                      | Уникальная строка Client Context. Максимальное ограничение — 256 шаров.                                                                                                                               |
| id                             | String                      | ID операции сервера. Только для чтения.                                                                                              |
| recordingAccessToken           | String                      | Маркер доступа, необходимый для получения записи.                                                                                              |
| recordingLocation              | String                      | Расположение, в котором находится запись.                                                                                                      |
| resultInfo                     | [resultInfo](resultinfo.md) | Сведения о результате.  Только для чтения.                                                                                              |
| status                         | String                      | Возможные значения: `notStarted`, `running`, `completed`, `failed`. Только для чтения.                                                |

## <a name="relationships"></a>Связи
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


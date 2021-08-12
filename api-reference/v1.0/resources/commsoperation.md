---
title: тип ресурса commsOperation
description: Состояние некоторых длительных операций.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: dd924966c34d39ceb26e7b92077f01f085f9f6779896db439c1ae6c7a57eae9c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54130389"
---
# <a name="commsoperation-resource-type"></a>тип ресурса commsOperation

Пространство имен: microsoft.graph

Представляет состояние некоторых длительных операций.

Этот ресурс может быть возвращен в качестве ответа на действие или как содержимое [commsNotification.](commsNotification.md)  

Когда он возвращается в качестве ответа на действие, состояние указывает, будут ли последующие уведомления. Если, например, операция со статусом или возвращается, по каналу уведомлений не будет никакой `completed` `failed` последующей операции. 

Если операция или операция со статусом или возвращается, последующие обновления будут приходить `null` `notStarted` через канал `running` уведомлений.

## <a name="properties"></a>Свойства

| Свойство           | Тип                        | Описание                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| clientContext      | String                      | Уникальная строка Client Context. Максимальное ограничение — 256 шаров.                           |
| id                 | String                      | ID операции. Только для чтения.                                                    |
| resultInfo         | [resultInfo](resultinfo.md) | Сведения о результате. Только для чтения.                                              |
| status             | String                      | Возможные значения: `notStarted`, `running`, `completed`, `failed`. Только для чтения. |

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.commsOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "resultInfo": { "@odata.type": "microsoft.graph.resultInfo" },
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "commsOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


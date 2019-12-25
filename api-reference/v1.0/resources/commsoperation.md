---
title: Тип ресурса Коммсоператион
description: Состояние определенных длительных операций.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 47937d059f9a624ca5b9c58333275081d5a68400
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866275"
---
# <a name="commsoperation-resource-type"></a>Тип ресурса Коммсоператион

Представляет состояние определенных длительных операций.

Этот ресурс может быть возвращен в качестве ответа на действие или в качестве содержимого [коммснотификатион](commsNotification.md).  

При возвращении в качестве ответа на действие состояние указывает, будут ли отображаться последующие уведомления. Если, например, операция со статусом `completed` или `failed` возвращена, дальнейшая операция с каналом уведомлений не будет выполняться. 

Если `null` операция или операция со статусом `notStarted` или `running` возвращены, последующие обновления будут поступать через канал уведомлений.

## <a name="properties"></a>Свойства

| Свойство           | Тип                        | Описание                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| Контекст      | String                      | Уникальная строка контекста клиента. Максимальный лимит — 256 символов.                           |
| id                 | Строка                      | ИДЕНТИФИКАТОР операции. Только для чтения.                                                    |
| resultInfo         | [resultInfo](resultinfo.md) | Сведения о результате. Только для чтения.                                              |
| status             | String                      | Возможные значения: `notStarted`, `running`, `completed`, `failed`. Только для чтения. |

## <a name="relationships"></a>Отношения
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

---
title: Тип ресурса SubscribeToToneOperation
description: Описывает формат ответа при создании подписки для получения тона DTMF.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: bcae95f7c711ee1853885e851b7f281e7f6597bd70ccd808722f75b67141a6be
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54169258"
---
# <a name="subscribetotoneoperation-resource-type"></a>Тип ресурса SubscribeToToneOperation

Пространство имен: microsoft.graph

Описывает формат ответа при создании подписки для получения тона DTMF.

## <a name="properties"></a>Свойства

| Свойство                       | Тип                        | Описание                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| clientContext                  | String                      | Клиентский контекст.                                                                                                                               |
| id                             | String                      | ID операции сервера. Только для чтения.                                                                                             |
| status                         | String                      | Возможные значения: `notStarted`, `running`, `completed`, `failed`. Только для чтения.                                                 |

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.subscribeToToneOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscribeToToneOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


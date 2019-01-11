---
title: Тип ресурса chatInfo
description: Сведения о сообщении в группах Майкрософт.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: c2cc0dd288abdab7852017600c4c55b9a40b0aa7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852943"
---
# <a name="chatinfo-resource-type"></a>Тип ресурса chatInfo

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Сведения о сообщении в группах Майкрософт.

## <a name="properties"></a>Свойства

| Свойство            | Тип    | Описание|
|:--------------------|:--------|:-----------|
| Код сообщения           | Строка  | Уникальный идентификатор для сообщения в канале группами Майкрософт. |
| replyChainMessageId | Строка  | Идентификатор сообщения. |
| threadId            | Строка  | Уникальный идентификатор потока в группами Майкрософт. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatInfo"
}-->
```json
{
  "messageId": "String",
  "replyChainMessageId": "String",
  "threadId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

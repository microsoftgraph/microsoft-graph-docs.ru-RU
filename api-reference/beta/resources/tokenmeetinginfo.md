---
title: Тип ресурса tokenMeetingInfo
description: Тип tokenMeetingInfo.
ms.openlocfilehash: ddaf9a0c36ce4a8a31c56e4db2e065ef186c4053
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076032"
---
# <a name="tokenmeetinginfo-resource-type"></a>Тип ресурса tokenMeetingInfo

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Тип tokenMeetingInfo.

## <a name="properties"></a>Свойства

| Свойство                     | Тип    | Description                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| allowConversationWithoutHost | Логический | Указывает, если беседы можно продолжить после покидает узла беседы. |
| токен                        | Строка  | Маркер для присоединения к/активации собрания.                                        |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tokenMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "token": "String"
}
```

## <a name="example"></a>Пример

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.tokenMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "token": "ABCD123"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tokenMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

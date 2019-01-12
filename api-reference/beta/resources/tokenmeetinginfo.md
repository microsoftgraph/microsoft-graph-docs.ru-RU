---
title: Тип ресурса tokenMeetingInfo
description: Тип tokenMeetingInfo.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0d68b60cdfc1470bb1c1c3846c34dfc76c5c5a1b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919269"
---
# <a name="tokenmeetinginfo-resource-type"></a>Тип ресурса tokenMeetingInfo

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Тип tokenMeetingInfo.

## <a name="properties"></a>Свойства

| Свойство                     | Тип    | Описание                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| allowConversationWithoutHost | Boolean | Указывает, если беседы можно продолжить после покидает узла беседы. |
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

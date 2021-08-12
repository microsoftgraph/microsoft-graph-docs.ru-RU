---
title: тип ресурса tokenMeetingInfo
description: Тип tokenMeetingInfo.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 269cd5589539cb63b20d61e5103a273a083882a4ffa89446e1c6629444d1b9c5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54159864"
---
# <a name="tokenmeetinginfo-resource-type"></a>тип ресурса tokenMeetingInfo

Пространство имен: microsoft.graph

Это информация маркера, которая позволяет присоединиться к существующему собранию. Это получается в рамках уведомления о входящих вызовах. 

В случае отключения вызова эта информация может помочь вам снова присоединять этот вызов.

## <a name="properties"></a>Свойства

| Свойство                     | Тип    | Описание                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| token                        | Строка  | Маркер, используемый для зова.                                                 |

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
    "token": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "tokenMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


---
title: тип ресурса tokenMeetingInfo
description: Тип tokenMeetingInfo.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d9abc9534d8e938f1dd4d783068ed81d22ca1ab1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59143659"
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


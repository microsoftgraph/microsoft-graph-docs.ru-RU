---
title: Тип ресурса Токенмитингинфо
description: Тип Токенмитингинфо.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5ac5e8303b0326e4c540757b7564edc55945cfc8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090671"
---
# <a name="tokenmeetinginfo-resource-type"></a>Тип ресурса Токенмитингинфо

Пространство имен: microsoft.graph

Это сведения о маркере, с помощью которого вы можете присоединиться к существующему собранию. Это значение получается в составе уведомления о входящем вызове. 

В случае отключения вызова эта информация поможет повторно присоединиться к этому вызову.

## <a name="properties"></a>Свойства

| Свойство                     | Тип    | Описание                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| token                        | Строка  | Маркер, используемый для присоединения к вызову.                                                 |

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


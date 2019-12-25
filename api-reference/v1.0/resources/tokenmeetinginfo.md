---
title: Тип ресурса Токенмитингинфо
description: Тип Токенмитингинфо.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e34a10b9cd0fb09ff29c2d3373ad51a92109dcea
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866245"
---
# <a name="tokenmeetinginfo-resource-type"></a>Тип ресурса Токенмитингинфо

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

---
title: Тип ресурса Токенмитингинфо
description: Тип Токенмитингинфо.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 05cc4c21fe3a8ea0d4b27b6c27b737ec6fe317d2
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40912974"
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

---
title: Тип ресурса Ресултинфо
description: Содержит сведения о результатах успешного выполнения и сбоя.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 39027ecf949860d9ffa757a95839ae7fd8184a27
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866254"
---
# <a name="resultinfo-resource-type"></a>Тип ресурса Ресултинфо

Содержит сведения о результатах успешного выполнения и сбоя. 

Код указывает, является ли результат универсальным успехом или ошибкой. Если код 2xx это успех, то в случае, если это 4xx ошибка клиента, и если это значение 5xx, то это может быть ошибка сервера.

Дочерние коды предоставляют дополнительные сведения, связанные с типом успеха или сбоем (например, успешная передача вызова).


## <a name="properties"></a>Свойства

| Свойство | Тип   | Описание          |
| :------- | :----- | :------------------  |
| code     | Int32 | Код результата.     |
| message  | String | Сообщение.         |
| Subcode  | Int32 | Дочерний код результата. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": 0,
  "message": "String",
  "subcode": 0
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resultInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

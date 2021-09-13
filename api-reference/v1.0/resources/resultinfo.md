---
title: тип ресурса resultInfo
description: Это содержит сведения об успехах и неудачах.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 89ac770d9ace4a35365e1c215e00c51e1d060bdd
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59113541"
---
# <a name="resultinfo-resource-type"></a>тип ресурса resultInfo

Пространство имен: microsoft.graph

Это содержит сведения об успехах и неудачах. 

Код указывает, является ли результат общим успехом или сбоем. Если код 2xx, это успех, если это 4xx это ошибка клиента, а если это 5xx, это ошибка сервера.

Под-коды предоставляют дополнительные сведения, связанные с типом успешности или сбоя (например, успешной передачей вызовов)


## <a name="properties"></a>Свойства

| Свойство | Тип   | Описание          |
| :------- | :----- | :------------------  |
| code     | Int32 | Код результатов.     |
| message  | String | Сообщение.         |
| подкод  | Int32 | Под код результатов. |

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


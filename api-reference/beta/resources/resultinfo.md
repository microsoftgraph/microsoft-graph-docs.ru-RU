---
title: Тип ресурса Ресултинфо
description: Содержит сведения о результатах, относящиеся к успехам и сбоям.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: aa55f8cdcb7ca4639aa4975a28ae2bcbcd625588
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521084"
---
# <a name="resultinfo-resource-type"></a>Тип ресурса Ресултинфо

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения о результатах, относящиеся к успехам и сбоям. 

Код указывает, является ли результат универсальным успехом или ошибкой. 

Вспомогательные коды предоставляют дополнительные сведения, связанные с типом успешного или неудачного завершения (например, успешная передача вызова).


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

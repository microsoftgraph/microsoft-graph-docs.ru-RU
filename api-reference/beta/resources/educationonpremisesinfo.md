---
title: Тип ресурса Едукатиононпремисесинфо
description: Дополнительные сведения, используемые для сопоставления локальной учетной записи пользователя Active Directory с их объектом пользователя Azure AD.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ff575398f3829c5d2adbe92799f5b9dca953aa4e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998826"
---
# <a name="educationonpremisesinfo-resource-type"></a>Тип ресурса Едукатиононпремисесинфо

Пространство имен: microsoft.graph

Дополнительные сведения, используемые для сопоставления локальной учетной записи пользователя Active Directory с их объектом пользователя Azure AD.

## <a name="properties"></a>Свойства

| Свойство    | Тип   | Описание                                               |
| :---------- | :----- | :-------------------------------------------------------- |
| Значения свойств ImmutableId | String | Уникальный идентификатор объекта пользователя в Active Directory. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOnPremisesInfo"
}-->

```json
{
  "immutableId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOnPremisesInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



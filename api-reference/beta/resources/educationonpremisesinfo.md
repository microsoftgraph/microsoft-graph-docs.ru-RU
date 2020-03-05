---
title: Тип ресурса Едукатиононпремисесинфо
description: Дополнительные сведения, используемые для сопоставления локальной учетной записи пользователя Active Directory с их объектом пользователя Azure AD.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 6695f1cd92ccde1fb26a581fce49c0c233deb141
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501516"
---
# <a name="educationonpremisesinfo-resource-type"></a>Тип ресурса Едукатиононпремисесинфо

Пространство имен: Microsoft. Graph

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

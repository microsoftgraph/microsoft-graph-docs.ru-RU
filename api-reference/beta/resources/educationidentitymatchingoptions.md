---
title: Тип ресурса educationIdentityMatchingOptions
description: Содержит сопоставления между свойство source и свойства конечного объекта для сопоставления учетных записей пользователей. Свойство source должна существовать в источнике данных. Свойство target должно быть допустимое свойство в Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: c2b092d5589cdccccfe73a7e71afcafa7b555a90
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425794"
---
# <a name="educationidentitymatchingoptions-resource-type"></a>Тип ресурса educationIdentityMatchingOptions

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Содержит сопоставления между свойство source и свойства конечного объекта для сопоставления учетных записей пользователей. Свойство source должна существовать в источнике данных. Свойство target должно быть допустимое свойство в Azure Active Directory (Azure AD).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **appliesTo** | string |  Тип роли пользователя для назначения лицензий. Возможные значения: `student`, `teacher`.      |
| **sourcePropertyName** | string |  Имя свойства источника, которое должно быть имя поля в источнике данных. Это свойство соответствует с учетом регистра.        |
| **targetPropertyName** | string |  Имя свойства для конечного объекта должен быть допустимым свойством в Azure AD. Это свойство соответствует с учетом регистра.     |
| **targetDomain** | string |  Домен суффикс со свойством источника для сопоставления в целевой системе. Если этот параметр указан как значение null, свойство source будет использоваться в соответствии с помощью свойства конечного объекта.        |

## <a name="json-representation"></a>Представление JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityMatchingOptions"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "sourcePropertyName": "String",
    "targetPropertyName": "String",
    "targetDomain": "String"
}
```

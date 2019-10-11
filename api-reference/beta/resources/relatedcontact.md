---
title: Тип ресурса Релатедконтакт
description: Контактная запись, связанная с educationUser, которая предоставляет информацию для хранителя, возможностей, доктора и т. д.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ce1ff84abb6704255267b521c67e5fc7b231b7df
ms.sourcegitcommit: e4b0211db9b20dfea8be964003661cd99fe064d1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2019
ms.locfileid: "37439936"
---
# <a name="relatedcontact-resource-type"></a>Тип ресурса Релатедконтакт

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контактная запись, связанная с [educationUser](../resources/educationuser.md) , которая предоставляет информацию для хранителя, возможностей, доктора и т. д.

## <a name="properties"></a>Свойства

| Свойство      | Тип                  | Описание                                                                                                         |
| :------------ | :-------------------- | :------------------------------------------------------------------------------------------------------------------ |
| id            | Строка                | Идентификатор контакта в Azure Active Directory.                                                              |
| displayName   | Строка                | Имя контакта. Обязательный.                                                                                      |
| emailAddress  | String                | Основной адрес электронной почты контакта.                                                                               |
| mobilePhone   | String                | Номер мобильного телефона контакта.                                                                                 |
| Отношение  | `contactRelationship` | Отношение к пользователю. Возможные значения: `parent`, `relative`, `aide`, `doctor` `guardian`,, `child`, `other`. |
| акцессконсент | Boolean               | Указывает, было ли пользователь отправлен для доступа к данным учащихся.                                               |

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.relatedContact"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "emailAddress": "String",
  "mobilePhone": "String",
  "relationship": "contactRelationship",
  "accessConsent": true
}
```

<!-- uuid: 720F9AB6-6E7A-4A66-8B0A-37A556FF99C5
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "relatedContact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

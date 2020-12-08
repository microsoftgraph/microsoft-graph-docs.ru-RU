---
title: Тип ресурса Релатедконтакт
description: Контактная запись, связанная с educationUser, которая предоставляет информацию для хранителя, возможностей, доктора и т. д.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f1dd62a2727ec2cbd6a4044b84105d739bbf9c93
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597384"
---
# <a name="relatedcontact-resource-type"></a>Тип ресурса Релатедконтакт

Пространство имен: microsoft.graph

Контактная запись, связанная с [educationUser](../resources/educationuser.md) , которая предоставляет информацию для хранителя, возможностей, доктора и т. д.

## <a name="properties"></a>Свойства

| Свойство      | Тип                  | Описание                                                                                                                               |
| :------------ | :-------------------- | :---------------------------------------------------------------------------------------------------------------------------------------- |
| id            | String                | Идентификатор контакта в Azure Active Directory.                                                                                    |
| displayName   | String                | Имя контакта. Обязательно.                                                                                                            |
| emailAddress  | String                | Основной адрес электронной почты контакта.                                                                                                     |
| mobilePhone   | String                | Номер мобильного телефона контакта.                                                                                                       |
| Отношение  | `contactRelationship` | Отношение к пользователю. Возможные значения:,,,,,, `parent` `relative` `aide` `doctor` `guardian` `child` `other` , `unknownFutureValue` . |
| акцессконсент | Логический               | Указывает, было ли пользователь отправлен для доступа к данным учащихся.                                                                     |

## <a name="json-representation"></a>Представление JSON

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


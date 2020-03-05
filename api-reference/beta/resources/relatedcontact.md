---
title: Тип ресурса Релатедконтакт
description: Контактная запись, связанная с educationUser, которая предоставляет информацию для хранителя, возможностей, доктора и т. д.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 7eb8f39c30343412584e63fa1e8c3382db4fa9c6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521189"
---
# <a name="relatedcontact-resource-type"></a>Тип ресурса Релатедконтакт

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контактная запись, связанная с [educationUser](../resources/educationuser.md) , которая предоставляет информацию для хранителя, возможностей, доктора и т. д.

## <a name="properties"></a>Свойства

| Свойство      | Тип                  | Описание                                                                                                         |
| :------------ | :-------------------- | :------------------------------------------------------------------------------------------------------------------ |
| id            | Строка                | Идентификатор контакта в Azure Active Directory.                                                              |
| displayName   | Строка                | Имя контакта. Обязательное.                                                                                      |
| emailAddress  | String                | Основной адрес электронной почты контакта.                                                                               |
| mobilePhone   | String                | Номер мобильного телефона контакта.                                                                                 |
| Отношение  | `contactRelationship` | Отношение к пользователю. Возможные значения: `parent`, `relative`, `aide`, `doctor` `guardian`,, `child`, `other`. |
| акцессконсент | Логический               | Указывает, было ли пользователь отправлен для доступа к данным учащихся.                                               |

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

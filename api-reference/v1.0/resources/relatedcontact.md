---
title: Тип ресурса Релатедконтакт
description: Контактная запись, связанная с educationUser, которая предоставляет информацию для хранителя, возможностей, доктора и т. д.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: adea95729dd4e6558885223245a7225811f14677
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002949"
---
# <a name="realtedcontact-resource-type"></a>Тип ресурса Реалтедконтакт

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
| акцессконсент | Boolean               | Указывает, было ли пользователь отправлен для доступа к данным учащихся.                                                                     |

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


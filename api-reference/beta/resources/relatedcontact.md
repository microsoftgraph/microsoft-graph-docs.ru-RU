---
title: Тип ресурса Релатедконтакт
description: Контактная запись, связанная с educationUser, которая предоставляет информацию для хранителя, возможностей, доктора и т. д.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 36e46261c3f31d9d41a63097753799b634dadeb2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008721"
---
# <a name="relatedcontact-resource-type"></a>Тип ресурса Релатедконтакт

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контактная запись, связанная с [educationUser](../resources/educationuser.md) , которая предоставляет инфоратион для опекунов, возможностей, доктора и т. д.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|Строка|Идентификатор контакта в Azure Active Directory.|
|displayName|Строка|Имя контакта. Обязательно.|
|emailAddress|String|Основной адрес электронной почты контакта.|
|mobilePhone|String|Номер мобильного телефона контакта.|
|Отношение|`contactRelationship`|Отношение к пользователю. Возможные значения: `parent`, `relative`, `aide`, `doctor` `guardian` `child`,,, `other`, `unknownFutureValue`.|
|Акцессконсент|Boolean|Указывает, было ли пользователь отправлен для доступа к данным учащихся.|

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

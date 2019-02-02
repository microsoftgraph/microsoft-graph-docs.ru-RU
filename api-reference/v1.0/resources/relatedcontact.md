---
title: Тип ресурса relatedContact
description: Запись контакта, связанные с educationUser, который предоставляет сведения для опекунов, возможностей, врачи и т. д.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 7e3829de2ffeb073d8360976ce70d13985fcae39
ms.sourcegitcommit: d6209114cbbe8072e3ecf7eba23819ae5ace7db5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2019
ms.locfileid: "29694491"
---
# <a name="realtedcontact-resource-type"></a>Тип ресурса realtedContact

Запись контакта, связанные с [educationUser](../resources/educationuser.md) , который предоставляет сведения для опекунов, возможностей, врачи и т. д.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|Строка|Идентификатор контакта в Azure Active Directory.|
|displayName|String|Имя контакта. Обязательный.|
|emailAddress|String|Основной адрес электронной почты контакта.|
|mobilePhone|String|Номер мобильного телефона контакта.|
|Отношение|`contactRelationship`|Отношение к пользователю. Возможные значения: `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`.|
|accessConsent|Boolean|Указывает, был ли пользователь изъявил для доступа к данным учебы.|

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

---
title: тип ресурсов relatedContact
description: Запись контактов, связанная с educationUser, который предоставляет информацию для опекунов, помощников, врачей и так далее.
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 528244c6cc84ab26c21ec1ea5c15c7bc8e68c082
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59035999"
---
# <a name="relatedcontact-resource-type"></a>тип ресурсов relatedContact

Пространство имен: microsoft.graph

Запись контактов, связанная с [educationUser,](../resources/educationuser.md) который предоставляет информацию для опекунов, помощников, врачей и так далее.

## <a name="properties"></a>Свойства

| Свойство      | Тип                  | Описание                                                                                                                               |
| :------------ | :-------------------- | :---------------------------------------------------------------------------------------------------------------------------------------- |
| id            | Строка                | Удостоверение контакта в Azure Active Directory.                                                                                    |
| displayName   | Строка                | Имя контакта. Обязательный.                                                                                                            |
| emailAddress  | String                | Основной адрес электронной почты контакта.                                                                                                     |
| mobilePhone   | String                | Номер мобильного телефона контакта.                                                                                                       |
| Отношение  | `contactRelationship` | Отношение к пользователю. Возможные значения `parent` : , , , , , `relative` `aide` `doctor` `guardian` `child` `other` `unknownFutureValue` . |
| accessConsent | Логический               | Указывает, было ли получено согласие пользователя на доступ к данным учащихся.                                                                     |

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


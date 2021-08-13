---
title: тип ресурсов relatedContact
description: Запись контактов, связанная с educationUser, который предоставляет информацию для опекунов, помощников, врачей и так далее.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 3a99702811601278c1d3bbe4413fec495b8ba2d6bd13b23dafd90b3ff86f7c19
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237532"
---
# <a name="relatedcontact-resource-type"></a>тип ресурсов relatedContact

Пространство имен: microsoft.graph

Запись контактов, связанная с [educationUser,](../resources/educationuser.md) который предоставляет информацию для опекунов, помощников, врачей и так далее.

## <a name="properties"></a>Свойства

| Свойство      | Тип                  | Описание                                                                                                                               |
| :------------ | :-------------------- | :---------------------------------------------------------------------------------------------------------------------------------------- |
| id            | String                | Удостоверение контакта в Azure Active Directory.                                                                                    |
| displayName   | String                | Имя контакта. Обязательный элемент.                                                                                                            |
| emailAddress  | String                | Основной адрес электронной почты контакта.                                                                                                     |
| mobilePhone   | String                | Номер мобильного телефона контакта.                                                                                                       |
| Отношение  | `contactRelationship` | Отношение к пользователю. Возможные значения `parent` : , , , , , `relative` `aide` `doctor` `guardian` `child` `other` `unknownFutureValue` . |
| accessConsent | Логическое               | Указывает, было ли получено согласие пользователя на доступ к данным учащихся.                                                                     |

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


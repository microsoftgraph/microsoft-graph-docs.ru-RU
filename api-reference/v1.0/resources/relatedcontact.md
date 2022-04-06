---
title: тип ресурсов relatedContact
description: Представляет запись контактов, связанную с educationUser, который предоставляет сведения для опекунов, помощников, врачей и так далее.
author: marcla
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b5d833afe05480a1ae4e490220ad16755f268c7a
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589438"
---
# <a name="relatedcontact-resource-type"></a>тип ресурсов relatedContact

Пространство имен: microsoft.graph

Представляет запись контактов, связанную с [educationUser](../resources/educationuser.md) , который предоставляет сведения для опекунов, помощников, врачей и так далее.

## <a name="properties"></a>Свойства

| Свойство      | Тип                  | Описание                                                                                                                               |
| :------------ | :-------------------- | :---------------------------------------------------------------------------------------------------------------------------------------- |
| accessConsent | Логический               | Указывает, было ли получено согласие пользователя на доступ к данным учащихся.                                                                     |
| displayName   | Строка                | Имя контакта. Обязательный аргумент.                                                                                                            |
| emailAddress  | String                | Основной адрес электронной почты контакта. Обязательный аргумент.                                                                                           |
| mobilePhone   | String                | Номер мобильного телефона контакта.                                                                                                       |
| Отношение  | contactRelationship | Отношение к пользователю. Возможные значения: `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`.|

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
  "accessConsent": true,
  "displayName": "String",
  "emailAddress": "String",
  "mobilePhone": "String",
  "relationship": "String"
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

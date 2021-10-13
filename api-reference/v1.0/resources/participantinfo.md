---
title: тип ресурса participantInfo
description: Содержит дополнительные свойства удостоверения участника
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 1cb408bf675668fb82374e4cfca5e67df2580a0e
ms.sourcegitcommit: f4999aa6fc05f845027db01aa489f7086f9850e1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/13/2021
ms.locfileid: "60289884"
---
# <a name="participantinfo-resource-type"></a>тип ресурса participantInfo

Пространство имен: microsoft.graph

Содержит дополнительные свойства удостоверения участника

## <a name="properties"></a>Свойства

| Свойство       | Тип                          | Описание                                                                                                                                                |
|:---------------|:------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| countryCode    | Строка                        | Код страны ISO 3166-1 Alpha-2 с наилучшими оценками физического расположения участника в начале вызова. Только для чтения.                             |
| endpointType   | Строка                        | Тип конечной точки, используемой участником. Возможные значения: `default`, `skypeForBusiness` или `skypeForBusinessVoipPhone`. Только для чтения.              |
| identity       | [identitySet](identityset.md) | [IdentitySet,](identityset.md) связанный с этим участником. Только для чтения.                                                                             |
| languageId     | Строка                        | Строка языковой культуры. Только для чтения.                                                                                                                    |
| регион         | Строка                        | Домашний регион участника. Это может быть страна, континент или более крупный географический регион. Это не меняется в зависимости от текущего физического расположения участника. Только для чтения. |
| participantId    | Строка                          | ID участника участника. Только для чтения.    |


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "countryCode",
    "endpointType",
    "languageId",
    "region",
    "participantId"
  ],
  "@odata.type": "microsoft.graph.participantInfo"
}-->
```json
{
  "countryCode": "String",
  "identity": { "@odata.type": "#microsoft.graph.identitySet" },
  "endpointType": "default | skypeForBusiness | skypeForBusinessVoipPhone",
  "languageId": "String",
  "region": "String",
  "participantId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


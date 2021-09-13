---
title: тип ресурса participantInfo
description: Содержит дополнительные свойства удостоверения участника
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d1d134eec6e6bef50eb7a97917a2f8aaa3b91148
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59104077"
---
# <a name="participantinfo-resource-type"></a>тип ресурса participantInfo

Пространство имен: microsoft.graph

Содержит дополнительные свойства удостоверения участника

## <a name="properties"></a>Свойства

| Свойство       | Тип                          | Описание                                                                                                                                                |
|:---------------|:------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| countryCode    | String                        | Код страны ISO 3166-1 Alpha-2 с наилучшими оценками физического расположения участника в начале вызова. Только для чтения.                             |
| endpointType   | Строка                        | Тип конечной точки, используемой участником. Возможные значения: `default`, `skypeForBusiness` или `skypeForBusinessVoipPhone`. Только для чтения.              |
| identity       | [identitySet](identityset.md) | [IdentitySet,](identityset.md) связанный с этим участником. Только для чтения.                                                                             |
| languageId     | String                        | Строка языковой культуры. Только для чтения.                                                                                                                    |
| регион         | Строка                        | Домашний регион участника. Это может быть страна, континент или более крупный географический регион. Это не меняется в зависимости от текущего физического расположения участника. Только для чтения. |


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "countryCode",
    "endpointType",
    "languageId",
    "region"
  ],
  "@odata.type": "microsoft.graph.participantInfo"
}-->
```json
{
  "countryCode": "String",
  "identity": { "@odata.type": "#microsoft.graph.identitySet" },
  "endpointType": "default | skypeForBusiness | skypeForBusinessVoipPhone",
  "languageId": "String",
  "region": "String"
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


---
title: Тип ресурса ПартиЦипантинфо
description: Содержит дополнительные свойства удостоверения участника
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: bd9c57961bee93e7d01e504bccb8671a8f1dd449
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522034"
---
# <a name="participantinfo-resource-type"></a>Тип ресурса ПартиЦипантинфо

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит дополнительные свойства удостоверения участника

## <a name="properties"></a>Свойства

| Свойство       | Тип                          | Описание                                                                                                                                                |
|:---------------|:------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| countryCode    | String                        | Код страны ISO 3166-1 Alpha-2 в наиболее подсчитанном физическом расположении участника в начале звонка. Только для чтения.                             |
| ендпоинттипе   | String                        | Тип конечной точки, используемой участником. Возможные значения: `default`, `skypeForBusiness`, или. `skypeForBusinessVoipPhone` Только для чтения.              |
| хищения       | [identitySet](identityset.md) | [Удостоверение](identityset.md) , связанное с этим участником. Только для чтения.                                                                             |
| languageId     | String                        | Строка языка и региональных параметров языка. Только для чтения.                                                                                                                    |
| региональных         | String                        | Домашняя область участника. Это может быть страна, континент или более крупный географический регион. Это не изменяется в зависимости от текущего физического расположения участника, в отличие от countryCode. Только для чтения. |

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

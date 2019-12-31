---
title: Тип ресурса ПартиЦипантинфо
description: Содержит дополнительные свойства удостоверения участника
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9b603d93b2be2fef6a999cf3c1d7663fc7405da9
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913732"
---
# <a name="participantinfo-resource-type"></a>Тип ресурса ПартиЦипантинфо

Содержит дополнительные свойства удостоверения участника

## <a name="properties"></a>Свойства

| Свойство       | Тип                          | Описание                                                                                                                                                |
|:---------------|:------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| хищения       | [identitySet](identityset.md) | [Удостоверение](identityset.md) , связанное с этим участником. Только для чтения.                                                                             |
| languageId     | String                        | Строка языка и региональных параметров языка. Только для чтения.                                                                                                                    |
| региональных         | String                        | Домашняя область участника. Это может быть страна, континент или более крупный географический регион. Это не изменяется в зависимости от текущего физического местоположения участника. Только для чтения. |


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "languageId",
    "region"
  ],
  "@odata.type": "microsoft.graph.participantInfo"
}-->
```json
{
  "identity": { "@odata.type": "#microsoft.graph.identitySet" },
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

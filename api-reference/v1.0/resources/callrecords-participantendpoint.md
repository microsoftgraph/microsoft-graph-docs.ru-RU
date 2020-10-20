---
title: Тип ресурса ПартиЦипантендпоинт
description: Тип ПартиЦипантендпоинт
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0002659ac32eaa1c76ad6dfecefd2a1f59c070e9
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601575"
---
# <a name="participantendpoint-resource-type"></a>Тип ресурса ПартиЦипантендпоинт

Пространство имен: microsoft.graph.callRecords

Представляет конечную точку участника в вызове. Конечная точка представляет пользователя или подобную пользователю сущность. Наследуется от типа [конечной точки](callrecords-endpoint.md) .

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|userAgent|[Microsoft. Graph. Каллрекордс. userAgent](callrecords-useragent.md)|Пользователь — агент, указанный этой конечной точкой.|
|feedback|[Microsoft. Graph. Каллрекордс. Усерфидбакк](callrecords-userfeedback.md)|Обратная связь, предоставленная пользователем данной конечной точки относительно качества сеанса.|
|хищения|[identitySet](identityset.md)|Удостоверение, связанное с конечной точкой.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.participantEndpoint",
  "baseType": "microsoft.graph.callRecords.endpoint"
}-->

```json
{
  "userAgent": {"@odata.type": "microsoft.graph.callRecords.userAgent"},
  "feedback": {"@odata.type": "microsoft.graph.callRecords.userFeedback"},
  "identity": {"@odata.type": "microsoft.graph.identitySet"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "participantEndpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

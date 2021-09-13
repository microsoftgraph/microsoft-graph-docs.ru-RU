---
title: тип ресурса participantEndpoint
description: Тип participantEndpoint
ms.localizationpriority: medium
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c9990701c86ed085914652b7c541411db6f57f65
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109509"
---
# <a name="participantendpoint-resource-type"></a>тип ресурса participantEndpoint

Пространство имен: microsoft.graph.callRecords

Представляет конечную точку участника в вызове. Конечная точка представляет объект, похожий на пользователя. Наследуется от [конечного](callrecords-endpoint.md) типа.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|userAgent|[microsoft.graph.callRecords.userAgent](callrecords-useragent.md)|Пользователь-агент, о чем сообщает эта конечная точка.|
|feedback|[microsoft.graph.callRecords.userFeedback](callrecords-userfeedback.md)|Отзывы, предоставленные пользователем этой конечной точки, о качестве сеанса.|
|identity|[identitySet](identityset.md)|Удостоверение, связанное с конечной точкой.|

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

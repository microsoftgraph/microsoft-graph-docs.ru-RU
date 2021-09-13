---
title: тип ресурса конечной точки
description: Тип конечной точки
ms.localizationpriority: medium
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: aa6338ad487ff4b662e85f8efef8c5f89841cdfe
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59025582"
---
# <a name="endpoint-resource-type"></a>тип ресурса конечной точки

Пространство имен: microsoft.graph.callRecords

Представляет конечную точку в вызове. Конечной точкой может быть устройство пользователя, собрание, приложение/бот и т.д. Типы [participantEndpoint](callrecords-participantendpoint.md) и [serviceEndpoint наследуются](callrecords-serviceendpoint.md) от этого типа.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|userAgent|[microsoft.graph.callRecords.userAgent](callrecords-useragent.md)|Пользователь-агент, о чем сообщает эта конечная точка.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.endpoint",
  "baseType": null
}-->

```json
{
  "userAgent": {"@odata.type": "microsoft.graph.callRecords.userAgent"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "endpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

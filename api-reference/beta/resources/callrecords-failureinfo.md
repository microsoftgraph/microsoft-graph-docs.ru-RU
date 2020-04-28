---
title: Тип ресурса Фаилуреинфо
description: Тип Фаилуреинфо
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3160fe3b2d0c1fd59ddd86621667b67ee5759dd5
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394857"
---
# <a name="failureinfo-resource-type"></a>Тип ресурса Фаилуреинфо

Пространство имен: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о причине сбоя вызова или части вызова.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|reason|String|Классификация причин сбоя вызова или части вызова.|
|разместить|String|Рабочая область при возникновении ошибки. Возможные значения: `unknown`, `callSetup`, `midcall`, `unknownFutureValue`.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.failureInfo",
  "baseType": null
}-->

```json
{
  "reason": "String",
  "stage": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "failureInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
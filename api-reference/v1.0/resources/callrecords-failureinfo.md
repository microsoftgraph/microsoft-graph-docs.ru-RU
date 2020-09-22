---
title: Тип ресурса Фаилуреинфо
description: Тип Фаилуреинфо
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: cd720663e3025525b19ffff62d8ef9b061d154b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069472"
---
# <a name="failureinfo-resource-type"></a>Тип ресурса Фаилуреинфо

Пространство имен: microsoft.graph.callRecords

Представляет сведения о причине сбоя вызова или части вызова.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|reason|Строка|Классификация причин сбоя вызова или части вызова.|
|разместить|Microsoft. Graph. Каллрекордс. Фаилурестаже|Рабочая область при возникновении ошибки. Возможные значения: `unknown`, `callSetup`, `midcall`, `unknownFutureValue`.|

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

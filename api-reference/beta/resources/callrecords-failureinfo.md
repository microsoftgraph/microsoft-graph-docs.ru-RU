---
title: Тип ресурса Фаилуреинфо
description: Тип Фаилуреинфо
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5edd2a501b3e1a5633f0bd01ac36815201eb927d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064376"
---
# <a name="failureinfo-resource-type"></a>Тип ресурса Фаилуреинфо

Пространство имен: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о причине сбоя вызова или части вызова.

Ошибка может относиться к двум типам: 

- Сбой при установке вызовов
- Метод MID — Drop

Если один или несколько потоков мультимедиа имеют какие-либо из этих ошибок, то этот сбой распространяется на уровне сегмента. Если один или несколько сегментов имеют какие-либо из этих ошибок, то этот сбой распространяется на уровне сеанса.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|reason|String|Классификация причин сбоя вызова или части вызова.|
|разместить|Microsoft. Graph. Каллрекордс. Фаилурестаже|Рабочая область при возникновении ошибки. Возможные значения: `unknown`, `callSetup`, `midcall`, `unknownFutureValue`.|

## <a name="json-representation"></a>Представление в формате JSON

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



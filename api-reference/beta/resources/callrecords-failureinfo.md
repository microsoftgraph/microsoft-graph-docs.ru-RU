---
title: Тип ресурса Фаилуреинфо
description: Тип Фаилуреинфо
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e67e0df2c3f98ea2c9c1b49d32cb6295559516dd
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601193"
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



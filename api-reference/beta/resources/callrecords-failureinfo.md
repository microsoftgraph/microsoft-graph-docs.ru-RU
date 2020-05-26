---
title: Тип ресурса Фаилуреинфо
description: Тип Фаилуреинфо
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 38ccc3094521283c6c496b1d0e35b97a6cf37199
ms.sourcegitcommit: ef9e0fd8fb6047fa9272e98310eaed2c4e0a2660
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/23/2020
ms.locfileid: "44353618"
---
# <a name="failureinfo-resource-type"></a>Тип ресурса Фаилуреинфо

Пространство имен: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о причине сбоя вызова или части вызова.

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
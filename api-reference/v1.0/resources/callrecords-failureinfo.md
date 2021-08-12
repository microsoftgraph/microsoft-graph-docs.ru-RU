---
title: тип ресурса failureInfo
description: Тип failureInfo
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: cabfe56215863385a55ded34914f78fdd856a0d7f341ac4cde1220f37cab77fe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54160088"
---
# <a name="failureinfo-resource-type"></a>тип ресурса failureInfo

Пространство имен: microsoft.graph.callRecords

Представляет сведения о том, почему не удалось вызвать или часть вызова.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|reason|String|Классификация причин сбой вызова или части вызова.|
|этап|microsoft.graph.callRecords.failureStage|Этап, на который произошел сбой. Возможные значения: `unknown`, `callSetup`, `midcall`, `unknownFutureValue`.|

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

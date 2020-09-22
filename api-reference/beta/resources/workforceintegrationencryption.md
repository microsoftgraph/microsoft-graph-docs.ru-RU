---
title: Тип ресурса Воркфорцеинтегратионенкриптион
description: Объект шифрования, определяющий протокол и секрет для интеграции сотрудников.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 15feb2097a3a7bf36092070cc2af4841d2aa3839
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019399"
---
# <a name="workforceintegrationencryption-resource-type"></a>Тип ресурса Воркфорцеинтегратионенкриптион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Объект шифрования, определяющий протокол и секрет для [воркфорцеинтегратион](../resources/workforceintegration.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|Protocol|String| Возможные значения: `sharedSecret`, `unknownFutureValue`.|
|гадк|String|Шифрование общего секрета.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workforceIntegrationEncryption",
  "baseType": null
}-->

```json
{
  "protocol": "String",
  "secret": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workforceIntegrationEncryption resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



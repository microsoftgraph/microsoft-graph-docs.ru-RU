---
title: Тип ресурса Воркфорцеинтегратионенкриптион
description: Объект шифрования, определяющий протокол и секрет для интеграции сотрудников.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c2d24371a0a999069d80a9ad86afd48ac9e68d38
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519080"
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

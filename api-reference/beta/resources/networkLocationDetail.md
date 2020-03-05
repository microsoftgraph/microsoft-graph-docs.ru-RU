---
title: Тип ресурса Нетворклокатиондетаил
description: Предоставляет имя и тип сети, из которой пользователь выполнил вход.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6cc1aa8f25fa3f2cae4cad4a253f758ace0532b0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522591"
---
# <a name="networklocationdetail-resource-type"></a>Тип ресурса Нетворклокатиондетаил

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет имя и тип сети, из которой пользователь выполнил вход.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|нетворкнамес|Коллекция String|Предоставляет имя сети, используемой при входе.|
|нетворктипе|нетворктипе| Предоставляет тип сети, используемой при входе. Возможные значения: `intranet`, `extranet`, `namedNetwork`, `trusted`, `unknownFutureValue`.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkLocationDetail",
  "baseType": null
}-->

```json
{
  "networkNames": ["String"],
  "networkType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkLocationDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
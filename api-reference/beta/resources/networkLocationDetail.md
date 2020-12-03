---
title: Тип ресурса Нетворклокатиондетаил
description: Предоставляет имя и тип сети, из которой пользователь выполнил вход.
localization_priority: Normal
author: besiler
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7c43341ab5799da83a084e035c680a1926b3d8e8
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523016"
---
# <a name="networklocationdetail-resource-type"></a>Тип ресурса Нетворклокатиондетаил

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет имя и тип сети, из которой пользователь выполнил вход.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|нетворкнамес|Коллекция объектов string|Предоставляет имя сети, используемой при входе.|
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


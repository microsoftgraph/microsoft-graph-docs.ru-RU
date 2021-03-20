---
title: signInFrequencySessionControl type
description: Управление сеансом для обеспечения частоты подписей.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 1f224c1e9ba72e114fd9c9bcacdd74670713837d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945629"
---
# <a name="signinfrequencysessioncontrol-resource-type"></a>signInFrequencySessionControl type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Управление сеансами для обеспечения частоты входов. Наследуется от [управления сеансами условного доступа.](conditionalaccesssessioncontrol.md)

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|isEnabled     |Boolean      | Указывает, включено ли управление сеансом. |
|type          |signinFrequencyType       | Возможные значения: `days`, `hours`.|
|value         |Int32        | Количество `days` или `hours` .|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInFrequencySessionControl",
  "baseType": "microsoft.graph.conditionalAccessSessionControl"
}-->

```json
{
  "isEnabled": true,
  "type": "String",
  "value": 1024
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInFrequencySessionControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



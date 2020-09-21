---
title: Тип ресурса Сигнинфрекуенцисессионконтрол
description: Управление сеансами для применения частоты входа.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8095469ddb29c79be3a22b84e58d7e4e52cd8d5c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067160"
---
# <a name="signinfrequencysessioncontrol-resource-type"></a>Тип ресурса Сигнинфрекуенцисессионконтрол

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Управление сеансами для обеспечения частоты входа. Наследуется от [управления сеансом условного доступа](conditionalaccesssessioncontrol.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|isEnabled     |Boolean      | Указывает, включен ли элемент управления сеансом. |
|type          |String       | Возможные значения: `days`, `hours`.|
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



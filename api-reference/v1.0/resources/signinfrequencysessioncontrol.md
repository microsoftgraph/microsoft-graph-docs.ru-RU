---
title: signInFrequencySessionControl type
description: Управление сеансом для обеспечения частоты подписей.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 5553e4ba3d3c51d44c4f212ca9a2885ac0037a88b1e2d6226cb69246904b0fba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54124173"
---
# <a name="signinfrequencysessioncontrol-resource-type"></a>signInFrequencySessionControl type

Пространство имен: microsoft.graph

Управление сеансами для обеспечения частоты входов. Наследуется от [управления сеансами условного доступа.](conditionalaccesssessioncontrol.md)

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|isEnabled     |Boolean      | Указывает, включено ли управление сеансом. |
|type          |signinFrequencyType| Возможные значения: `days`, `hours`.|
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


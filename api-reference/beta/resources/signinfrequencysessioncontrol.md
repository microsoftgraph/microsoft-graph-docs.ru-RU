---
title: Тип ресурса signInFrequencySessionControl
description: Управление сеансом для обеспечения частоты входа.
ms.localizationpriority: medium
author: rckyplln
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: a42697bd49f9f6742c3f6c1e61ace9a8a1362111
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65944451"
---
# <a name="signinfrequencysessioncontrol-resource-type"></a>Тип ресурса signInFrequencySessionControl

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Управление сеансом для обеспечения частоты входа. Наследуется от [управления сеансом условного доступа](conditionalaccesssessioncontrol.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|isEnabled     |Boolean      | Указывает, включен ли элемент управления сеансом. |
|type          |SigninFrequencyType       | Возможные значения: `days`или `hours`, `null` если frequencyInterval имеет значение `everyTime` .|
|value         |Int32        | Число или `days` `hours`.|
|authenticationType |signInFrequencyAuthenticationType  | Возможные значения: `primaryAndSecondaryAuthentication`, `secondaryAuthentication`. `unknownFutureValue`|
|frequencyInterval  |signInFrequencyInterval  | Возможные значения: `timeBased`, `everyTime`. `unknownFutureValue`|

## <a name="relationships"></a>Отношения

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
  "isEnabled":true,
  "type": "String",
  "value": 1024,
  "authenticationType": "String",
  "frequencyInterval": "String"
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



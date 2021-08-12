---
title: тип ресурса applicationEnforcedRestrictionsSessionControl
description: Управление сеансами для применения ограничений приложения.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: eabfdcc57439e2d254acc9ae5eeec2f613197f669f2ff68cd2ecf8bbc6bc98cb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54252160"
---
# <a name="applicationenforcedrestrictionssessioncontrol-resource-type"></a>тип ресурса applicationEnforcedRestrictionsSessionControl

Пространство имен: microsoft.graph

Управление сеансами для применения ограничений приложения. Наследуется от [управления сеансами условного доступа.](conditionalaccesssessioncontrol.md)

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|isEnabled     |Boolean      | Указывает, включено или нет управление сеансом. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationEnforcedRestrictionsSessionControl",
  "baseType": "microsoft.graph.conditionalAccessSessionControl"
}-->

```json
{
  "isEnabled": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationEnforcedRestrictionsSessionControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


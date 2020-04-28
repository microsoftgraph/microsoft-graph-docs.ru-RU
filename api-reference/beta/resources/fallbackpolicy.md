---
title: Тип ресурса Фаллбаккполици
description: 'Позволяет указать резервную политику только для конечных точек iOS и предназначена для использования для необработанных уведомлений с высоким приоритетом. '
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: 822a5d24acbec878b864c70d357f76a1fa115e4b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42498576"
---
# <a name="fallbackpolicy-resource-type"></a>Тип ресурса Фаллбаккполици

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Позволяет указать резервную политику только для конечных точек iOS и предназначена для использования для необработанных уведомлений с высоким приоритетом, которые могут не доставляться на устройства из-за ограничений, определенных платформой (например, режим экономии заряда).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| ендпоинтфаллбакк | [фаллбаккполиципропертиес](fallbackpolicyproperties.md) | Объект политики Ендпоинтфаллбакк обрабатывает политику резервного использования уведомлений на уровне конечной точки и в настоящее время ограничивается iOS. |   


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fallbackpolicy",
  "baseType": null
}-->

```json
{
  "endpointFallback": {"@odata.type": "microsoft.graph.fallbackpolicyProperties"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fallbackpolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: тип ресурса конфигурации
description: Указывает дополнительные ID-адреса приложений, которые разрешены для управления внешним подключением и индексации контента в externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 05fbf022c11cf318281831d1b4e8572646875a06
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467831"
---
# <a name="configuration-resource-type"></a>тип ресурса конфигурации

Пространство имен: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает дополнительные ID-адреса приложений, которые разрешены для управления внешним подключением и индексации контента [в externalConnection.](../resources/externalconnectors-externalconnection.md)

## <a name="properties"></a>Свойства

| Свойство       | Тип              | Описание |
|:---------------|:------------------|:------------|
| authorizedAppIds | Коллекция строк | Коллекция ID-приложений для зарегистрированных Azure Active Directory приложений, которые разрешены для управления внешним подключением и индексации контента в externalConnection. |

> [!NOTE]
> Свойство `authorizedAppIds` было ранее названо `authorizedApps` .

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnectors.configuration",
  "baseType": null
}-->

```json
{
  "authorizedAppIds": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "configuration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

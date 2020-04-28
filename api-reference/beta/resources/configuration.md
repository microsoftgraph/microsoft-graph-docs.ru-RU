---
title: Тип ресурса конфигурации
description: Задает дополнительные идентификаторы приложений, которым разрешено управлять Екстерналконнектион и индексировать содержимое в Екстерналконнектион.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: be4fa7bd8f4b44842bd6dbc9876d0dd19fe466fd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507501"
---
# <a name="configuration-resource-type"></a>Тип ресурса конфигурации

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Задает дополнительные идентификаторы приложений, которым разрешено управлять Екстерналконнектион и индексировать содержимое в [екстерналконнектион](../resources/externalconnection.md).

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a>Свойства

| Свойство       | Тип              | Описание |
|:---------------|:------------------|:------------|
| аусоризедаппс | Коллекция объектов string | Коллекция идентификаторов приложений для зарегистрированных приложений Azure Active Directory, которым разрешено управлять Екстерналконнектион и индексировать контент в Екстерналконнектион. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.configuration",
  "baseType": null
}-->

```json
{
  "authorizedApps": ["String"]
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

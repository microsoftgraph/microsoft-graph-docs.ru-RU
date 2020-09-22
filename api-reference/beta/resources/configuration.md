---
title: Тип ресурса конфигурации
description: Задает дополнительные идентификаторы приложений, которым разрешено управлять Екстерналконнектион и индексировать содержимое в Екстерналконнектион.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: bd267c77a9904564e8b2b7f592f207204d9396b0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994220"
---
# <a name="configuration-resource-type"></a>Тип ресурса конфигурации

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Задает дополнительные идентификаторы приложений, которым разрешено управлять Екстерналконнектион и индексировать содержимое в [екстерналконнектион](../resources/externalconnection.md).

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a>Свойства

| Свойство       | Тип              | Описание |
|:---------------|:------------------|:------------|
| аусоризедаппс | Коллекция String | Коллекция идентификаторов приложений для зарегистрированных приложений Azure Active Directory, которым разрешено управлять Екстерналконнектион и индексировать контент в Екстерналконнектион. |

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



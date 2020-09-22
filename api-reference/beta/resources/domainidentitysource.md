---
title: Тип ресурса Домаинидентитисаурце
description: Тип Домаинидентитисаурце определяет домен, не относящийся к клиенту, в качестве источника удостоверения для подключенной Организации.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 63301dbf42a4589fd204290c157c6e6f63e473d2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010317"
---
# <a name="domainidentitysource-resource-type"></a>Тип ресурса Домаинидентитисаурце

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется в источниках удостоверений [коннектедорганизатион](connectedOrganization.md). `@odata.type`Значение `#microsoft.graph.domainIdentitySource` указывает на то, что этот тип определяет домен как источник идентификаторов для подключенной Организации.

## <a name="properties"></a>Свойства

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| displayName |String | Имя источника удостоверений, как правило, также доменное имя. Только для чтения. |
| domainName |String | Доменное имя. Только для чтения. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено представление типа в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainIdentitySource",
  "baseType": "microsoft.graph.identitySource"
}-->

```json
{
  "domainName": "String",
  "displayName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainIdentitySource resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



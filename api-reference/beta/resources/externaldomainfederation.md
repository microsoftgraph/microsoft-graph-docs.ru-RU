---
title: Тип ресурса Екстерналдомаинфедератион
description: Тип Екстерналдомаинфедератион определяет домен, не относящийся к клиенту, с настроенным поставщиком удостоверений в качестве источника удостоверений для подключенной Организации.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d81255a3687bf3d6aafe9369f901b209f5827b77
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026917"
---
# <a name="externaldomainfederation-resource-type"></a>Тип ресурса Екстерналдомаинфедератион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется в источниках удостоверений [коннектедорганизатион](connectedOrganization.md). `@odata.type`Значение `#microsoft.graph.externalDomainFederation` указывает на то, что этот тип определяет домен с настроенным поставщиком удостоверений в качестве источника удостоверений для подключенной Организации.

## <a name="properties"></a>Свойства

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| displayName |String | Имя источника удостоверений, как правило, также доменное имя. Только для чтения. |
| domainName |String | Доменное имя. Только для чтения. |
| иссуерури |String | Иссуерури входящей Федерации. Только для чтения. |

## <a name="relationships"></a>Отношения

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено представление типа в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalDomainFederation",
  "baseType": "microsoft.graph.identitySource"
}-->

```json
{
  "domainName": "String",
  "displayName": "String",
  "issuerUri": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalDomainFederation resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



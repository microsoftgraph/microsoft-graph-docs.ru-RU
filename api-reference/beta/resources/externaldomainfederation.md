---
title: Тип ресурса Екстерналдомаинфедератион
description: Тип Екстерналдомаинфедератион определяет домен, не относящийся к клиенту, с настроенным поставщиком удостоверений в качестве источника удостоверений для подключенной Организации.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ffeaa955ac43a52a0e3485f4a561163d4d27a957
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510300"
---
# <a name="externaldomainfederation-resource-type"></a>Тип ресурса Екстерналдомаинфедератион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется в источниках удостоверений [коннектедорганизатион](connectedOrganization.md). `@odata.type`Значение `#microsoft.graph.externalDomainFederation` указывает на то, что этот тип определяет домен с настроенным поставщиком удостоверений в качестве источника удостоверений для подключенной Организации.

## <a name="properties"></a>Свойства

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| displayName |Строка | Имя источника удостоверений, как правило, также доменное имя. Только для чтения. |
| domainName |String | Доменное имя. Только для чтения. |
| иссуерури |Строка | Иссуерури входящей Федерации. Только для чтения. |

## <a name="relationships"></a>Связи

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

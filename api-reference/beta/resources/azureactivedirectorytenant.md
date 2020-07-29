---
title: Тип ресурса Азуреактиведиректоритенант
description: Тип Азуреактиведиректоритенант определяет другого клиента Azure Active Directory в качестве источника удостоверения для подключенной Организации.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 881454f9658ae266705804518c3b5d8a876861eb
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510356"
---
# <a name="azureactivedirectorytenant-resource-type"></a>Тип ресурса Азуреактиведиректоритенант

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется в источниках удостоверений [коннектедорганизатион](connectedOrganization.md). `@odata.type`Значение `#microsoft.graph.azureActiveDirectoryTenant` указывает на то, что этот тип определяет другого клиента Azure Active Directory в качестве источника удостоверений для подключенной Организации.

## <a name="properties"></a>Свойства

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| displayName |Строка | Имя клиента Azure Active Directory. Только для чтения. |
| tenantId |String | Идентификатор клиента Azure Active Directory. Только для чтения. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено представление типа в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.azureActiveDirectoryTenant",
  "baseType": "microsoft.graph.identitySource"
}-->

```json
{
  "tenantId": "String (identifier)",
  "displayName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "azureActiveDirectoryTenant resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

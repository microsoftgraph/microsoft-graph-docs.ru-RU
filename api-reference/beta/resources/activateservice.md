---
title: тип ресурса activateService
description: Представляет службу, которая должна быть активирована.
author: dkershaw10
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6645da51b2f292d787c277096465b0a4b65e0347
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63331888"
---
# <a name="activateservice-resource-type"></a>тип ресурса activateService

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет службу, которая должна быть активирована.

## <a name="properties"></a>Свойства

| Свойство         | Тип         | Описание                           |
| ----------------- | ------------ | ------------------------------------- |
| service| String | Имя службы для активации. |
| servicePlanId | Guid | Идентификатор плана для активации плана службы. |
| skuId | Guid | Идентификатор SKU плана службы. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.activateService"
}-->

```json
{
    "service": "String",
    "skuId": "Guid",
    "servicePlanId": "Guid"
}

```

<!-- uuid: 20fd7863-9545-40d4-ae8f-fee2d115a690
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "activateService",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

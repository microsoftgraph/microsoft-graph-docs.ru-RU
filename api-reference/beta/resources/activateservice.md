---
title: тип ресурса activateService
description: Представляет службу, которая должна быть активирована.
author: dkershaw10
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: d007512113ab46b25714942f93002936c97fe083
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854552"
---
# <a name="activateservice-resource-type"></a>тип ресурса activateService

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет службу, которая должна быть активирована.

## <a name="properties"></a>Свойства

| Свойство         | Тип         | Описание                           |
| ----------------- | ------------ | ------------------------------------- |
| service| String | Имя службы для активации. |
| servicePlanId | GUID | Идентификатор плана для активации плана службы. |
| skuId | GUID | Идентификатор SKU плана службы. |

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
    "skuId": "GUID",
    "servicePlanId": "GUID"
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

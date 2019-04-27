---
title: Тип ресурса Воркбукфилтеркритериа
description: Представляет условия фильтра, применяемые к столбцу.
localization_priority: Normal
ms.openlocfilehash: 4906a44c88fdd7cb071b4ea994fee609cda1151c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348979"
---
# <a name="workbookfiltercriteria-resource-type"></a>Тип ресурса Воркбукфилтеркритериа

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет условия фильтра, применяемые к столбцу.

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilterCriteria"
}-->

```json
{
  "color": "string",
  "criterion1": "string",
  "criterion2": "string",
  "dynamicCriteria": "string",
  "filterOn": "string",
  "values": {"@odata.type":"microsoft.graph.Json"},
  "icon":{"@odata.type": "microsoft.graph.workbookIcon"},
  "operator":"string"
}
```

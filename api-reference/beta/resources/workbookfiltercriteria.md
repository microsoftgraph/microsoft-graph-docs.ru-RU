---
title: Тип ресурса Воркбукфилтеркритериа
description: Представляет условия фильтра, применяемые к столбцу.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: ruoyingl
ms.openlocfilehash: 6bd7906d458cf3573fe0d7d3f61cc5c8684e1c03
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808489"
---
# <a name="workbookfiltercriteria-resource-type"></a><span data-ttu-id="59080-103">Тип ресурса Воркбукфилтеркритериа</span><span class="sxs-lookup"><span data-stu-id="59080-103">workbookFilterCriteria resource type</span></span>

<span data-ttu-id="59080-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59080-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59080-105">Представляет условия фильтра, применяемые к столбцу.</span><span class="sxs-lookup"><span data-stu-id="59080-105">Represents the filtering criteria applied to a column.</span></span>

## <a name="json-representation"></a><span data-ttu-id="59080-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="59080-106">JSON representation</span></span>

<span data-ttu-id="59080-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="59080-107">Here is a JSON representation of the resource.</span></span>

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

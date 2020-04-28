---
title: Тип ресурса Воркбукфилтеркритериа
description: Представляет условия фильтра, применяемые к столбцу.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: ''
ms.openlocfilehash: d63e42f8efee5652edb48604e5d1831e436a4e01
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519227"
---
# <a name="workbookfiltercriteria-resource-type"></a><span data-ttu-id="05255-103">Тип ресурса Воркбукфилтеркритериа</span><span class="sxs-lookup"><span data-stu-id="05255-103">workbookFilterCriteria resource type</span></span>

<span data-ttu-id="05255-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05255-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05255-105">Представляет условия фильтра, применяемые к столбцу.</span><span class="sxs-lookup"><span data-stu-id="05255-105">Represents the filtering criteria applied to a column.</span></span>

## <a name="json-representation"></a><span data-ttu-id="05255-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="05255-106">JSON representation</span></span>

<span data-ttu-id="05255-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05255-107">Here is a JSON representation of the resource.</span></span>

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

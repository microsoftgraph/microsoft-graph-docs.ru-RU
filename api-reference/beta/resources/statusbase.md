---
title: тип ресурса statusBase
description: Описывает состояние события сводки по подготовкам.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: f486066b150ccd0321f23f47089aab67d87e9f7e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950303"
---
# <a name="statusbase-resource-type"></a><span data-ttu-id="db1fc-103">тип ресурса statusBase</span><span class="sxs-lookup"><span data-stu-id="db1fc-103">statusBase resource type</span></span>

<span data-ttu-id="db1fc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db1fc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db1fc-105">Описывает состояние события сводки по подготовкам.</span><span class="sxs-lookup"><span data-stu-id="db1fc-105">Describes the status of the provisioning summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="db1fc-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="db1fc-106">Properties</span></span>

| <span data-ttu-id="db1fc-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="db1fc-107">Property</span></span>     | <span data-ttu-id="db1fc-108">Тип</span><span class="sxs-lookup"><span data-stu-id="db1fc-108">Type</span></span>        | <span data-ttu-id="db1fc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="db1fc-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="db1fc-110">status</span><span class="sxs-lookup"><span data-stu-id="db1fc-110">status</span></span>|<span data-ttu-id="db1fc-111">provisioningResult</span><span class="sxs-lookup"><span data-stu-id="db1fc-111">provisioningResult</span></span>| <span data-ttu-id="db1fc-112">Возможные значения: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="db1fc-112">Possible values are: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="db1fc-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="db1fc-113">JSON representation</span></span>

<span data-ttu-id="db1fc-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db1fc-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.statusBase",
  "baseType": null
}-->

```json
{
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "statusBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



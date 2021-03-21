---
title: тип ресурса provisioningStep
description: 'Описывает действия, предпринятые для выполнения действия. '
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 6baf1656cb470cfc8dc01908f5a398ac5d421eb1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960343"
---
# <a name="provisioningstep-resource-type"></a><span data-ttu-id="74b74-103">тип ресурса provisioningStep</span><span class="sxs-lookup"><span data-stu-id="74b74-103">provisioningStep resource type</span></span>

<span data-ttu-id="74b74-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74b74-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74b74-105">Описывает действия, предпринятые для выполнения действия.</span><span class="sxs-lookup"><span data-stu-id="74b74-105">Describes the steps taken to perform an action.</span></span>

## <a name="properties"></a><span data-ttu-id="74b74-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="74b74-106">Properties</span></span>

| <span data-ttu-id="74b74-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="74b74-107">Property</span></span>     | <span data-ttu-id="74b74-108">Тип</span><span class="sxs-lookup"><span data-stu-id="74b74-108">Type</span></span>        | <span data-ttu-id="74b74-109">Описание</span><span class="sxs-lookup"><span data-stu-id="74b74-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="74b74-110">description</span><span class="sxs-lookup"><span data-stu-id="74b74-110">description</span></span>|<span data-ttu-id="74b74-111">Строка</span><span class="sxs-lookup"><span data-stu-id="74b74-111">String</span></span>|<span data-ttu-id="74b74-112">Сводка о том, что произошло во время шага.</span><span class="sxs-lookup"><span data-stu-id="74b74-112">Summary of what occurred during the step.</span></span>|
|<span data-ttu-id="74b74-113">подробности</span><span class="sxs-lookup"><span data-stu-id="74b74-113">details</span></span>|[<span data-ttu-id="74b74-114">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="74b74-114">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="74b74-115">Сведения о том, что произошло во время шага.</span><span class="sxs-lookup"><span data-stu-id="74b74-115">Details of what occurred during the step.</span></span>|
|<span data-ttu-id="74b74-116">name</span><span class="sxs-lookup"><span data-stu-id="74b74-116">name</span></span>|<span data-ttu-id="74b74-117">String</span><span class="sxs-lookup"><span data-stu-id="74b74-117">String</span></span>|<span data-ttu-id="74b74-118">Имя шага.</span><span class="sxs-lookup"><span data-stu-id="74b74-118">Name of the step.</span></span>|
|<span data-ttu-id="74b74-119">provisioningStepType</span><span class="sxs-lookup"><span data-stu-id="74b74-119">provisioningStepType</span></span>|<span data-ttu-id="74b74-120">provisioningStepType</span><span class="sxs-lookup"><span data-stu-id="74b74-120">provisioningStepType</span></span>| <span data-ttu-id="74b74-121">Тип шага.</span><span class="sxs-lookup"><span data-stu-id="74b74-121">Type of step.</span></span> <span data-ttu-id="74b74-122">Возможные значения: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="74b74-122">Possible values are: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="74b74-123">status</span><span class="sxs-lookup"><span data-stu-id="74b74-123">status</span></span>|<span data-ttu-id="74b74-124">provisioningResult</span><span class="sxs-lookup"><span data-stu-id="74b74-124">provisioningResult</span></span>| <span data-ttu-id="74b74-125">Состояние шага.</span><span class="sxs-lookup"><span data-stu-id="74b74-125">Status of the step.</span></span> <span data-ttu-id="74b74-126">Возможные значения: `success` `warning` , , ,  `failure` `skipped` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="74b74-126">Possible values are: `success`, `warning`,  `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="74b74-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="74b74-127">JSON representation</span></span>

<span data-ttu-id="74b74-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74b74-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningStep",
  "baseType": null
}-->

```json
{
  "description": "String",
  "details": {"@odata.type": "microsoft.graph.detailsInfo"},
  "name": "String",
  "provisioningStepType": "String",
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningStep resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



---
title: тип ресурса provisioningStep
description: 'Описывает действия, предпринятые для выполнения действия. '
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 695f0c30e802dabb03cb30f0615ee6a59e8cc540
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241547"
---
# <a name="provisioningstep-resource-type"></a><span data-ttu-id="fc393-103">тип ресурса provisioningStep</span><span class="sxs-lookup"><span data-stu-id="fc393-103">provisioningStep resource type</span></span>

<span data-ttu-id="fc393-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc393-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fc393-105">Описывает действия, предпринятые для выполнения действия.</span><span class="sxs-lookup"><span data-stu-id="fc393-105">Describes the steps taken to perform an action.</span></span>

## <a name="properties"></a><span data-ttu-id="fc393-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc393-106">Properties</span></span>

| <span data-ttu-id="fc393-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc393-107">Property</span></span>     | <span data-ttu-id="fc393-108">Тип</span><span class="sxs-lookup"><span data-stu-id="fc393-108">Type</span></span>        | <span data-ttu-id="fc393-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fc393-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fc393-110">description</span><span class="sxs-lookup"><span data-stu-id="fc393-110">description</span></span>|<span data-ttu-id="fc393-111">Строка</span><span class="sxs-lookup"><span data-stu-id="fc393-111">String</span></span>|<span data-ttu-id="fc393-112">Сводка о том, что произошло во время шага.</span><span class="sxs-lookup"><span data-stu-id="fc393-112">Summary of what occurred during the step.</span></span>|
|<span data-ttu-id="fc393-113">подробности</span><span class="sxs-lookup"><span data-stu-id="fc393-113">details</span></span>|[<span data-ttu-id="fc393-114">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="fc393-114">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="fc393-115">Сведения о том, что произошло во время шага.</span><span class="sxs-lookup"><span data-stu-id="fc393-115">Details of what occurred during the step.</span></span>|
|<span data-ttu-id="fc393-116">name</span><span class="sxs-lookup"><span data-stu-id="fc393-116">name</span></span>|<span data-ttu-id="fc393-117">String</span><span class="sxs-lookup"><span data-stu-id="fc393-117">String</span></span>|<span data-ttu-id="fc393-118">Имя шага.</span><span class="sxs-lookup"><span data-stu-id="fc393-118">Name of the step.</span></span>|
|<span data-ttu-id="fc393-119">provisioningStepType</span><span class="sxs-lookup"><span data-stu-id="fc393-119">provisioningStepType</span></span>|<span data-ttu-id="fc393-120">provisioningStepType</span><span class="sxs-lookup"><span data-stu-id="fc393-120">provisioningStepType</span></span>| <span data-ttu-id="fc393-121">Тип шага.</span><span class="sxs-lookup"><span data-stu-id="fc393-121">Type of step.</span></span> <span data-ttu-id="fc393-122">Возможные значения: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="fc393-122">Possible values are: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="fc393-123">status</span><span class="sxs-lookup"><span data-stu-id="fc393-123">status</span></span>|<span data-ttu-id="fc393-124">provisioningResult</span><span class="sxs-lookup"><span data-stu-id="fc393-124">provisioningResult</span></span>| <span data-ttu-id="fc393-125">Состояние шага.</span><span class="sxs-lookup"><span data-stu-id="fc393-125">Status of the step.</span></span> <span data-ttu-id="fc393-126">Возможные значения: `success` `warning` , , ,  `failure` `skipped` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="fc393-126">Possible values are: `success`, `warning`,  `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fc393-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fc393-127">JSON representation</span></span>

<span data-ttu-id="fc393-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc393-128">The following is a JSON representation of the resource.</span></span>

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



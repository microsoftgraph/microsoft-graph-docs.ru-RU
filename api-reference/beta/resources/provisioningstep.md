---
title: Тип ресурса provisioningStep
description: 'Описывает действия, выполняемые для выполнения действия. '
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: bfc0fef09c1dfa8da4161a75449894e391ca1974
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135354"
---
# <a name="provisioningstep-resource-type"></a><span data-ttu-id="d778e-103">Тип ресурса provisioningStep</span><span class="sxs-lookup"><span data-stu-id="d778e-103">provisioningStep resource type</span></span>

<span data-ttu-id="d778e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d778e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d778e-105">Описывает действия, выполняемые для выполнения действия.</span><span class="sxs-lookup"><span data-stu-id="d778e-105">Describes the steps taken to perform an action.</span></span>

## <a name="properties"></a><span data-ttu-id="d778e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d778e-106">Properties</span></span>

| <span data-ttu-id="d778e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d778e-107">Property</span></span>     | <span data-ttu-id="d778e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d778e-108">Type</span></span>        | <span data-ttu-id="d778e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d778e-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d778e-110">description</span><span class="sxs-lookup"><span data-stu-id="d778e-110">description</span></span>|<span data-ttu-id="d778e-111">Строка</span><span class="sxs-lookup"><span data-stu-id="d778e-111">String</span></span>|<span data-ttu-id="d778e-112">Сводка того, что произошло во время шага.</span><span class="sxs-lookup"><span data-stu-id="d778e-112">Summary of what occurred during the step.</span></span>|
|<span data-ttu-id="d778e-113">details</span><span class="sxs-lookup"><span data-stu-id="d778e-113">details</span></span>|[<span data-ttu-id="d778e-114">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="d778e-114">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="d778e-115">Сведения о том, что произошло во время шага.</span><span class="sxs-lookup"><span data-stu-id="d778e-115">Details of what occurred during the step.</span></span>|
|<span data-ttu-id="d778e-116">name</span><span class="sxs-lookup"><span data-stu-id="d778e-116">name</span></span>|<span data-ttu-id="d778e-117">String</span><span class="sxs-lookup"><span data-stu-id="d778e-117">String</span></span>|<span data-ttu-id="d778e-118">Имя шага.</span><span class="sxs-lookup"><span data-stu-id="d778e-118">Name of the step.</span></span>|
|<span data-ttu-id="d778e-119">provisioningStepType</span><span class="sxs-lookup"><span data-stu-id="d778e-119">provisioningStepType</span></span>|<span data-ttu-id="d778e-120">Строка</span><span class="sxs-lookup"><span data-stu-id="d778e-120">String</span></span>| <span data-ttu-id="d778e-121">Тип шага.</span><span class="sxs-lookup"><span data-stu-id="d778e-121">Type of step.</span></span> <span data-ttu-id="d778e-122">Возможные значения: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="d778e-122">Possible values are: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="d778e-123">status</span><span class="sxs-lookup"><span data-stu-id="d778e-123">status</span></span>|<span data-ttu-id="d778e-124">String</span><span class="sxs-lookup"><span data-stu-id="d778e-124">String</span></span>| <span data-ttu-id="d778e-125">Состояние шага.</span><span class="sxs-lookup"><span data-stu-id="d778e-125">Status of the step.</span></span> <span data-ttu-id="d778e-126">Возможные значения: `success` , , , `warning`  `failure` `skipped` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="d778e-126">Possible values are: `success`, `warning`,  `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d778e-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d778e-127">JSON representation</span></span>

<span data-ttu-id="d778e-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d778e-128">The following is a JSON representation of the resource.</span></span>

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



---
title: Тип ресурса Провисионингстеп
description: 'Описывает действия, предпринимаемые для выполнения действия. '
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 24685d0d2a25d00b19bcb796ae0df304c8224ebd
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523541"
---
# <a name="provisioningstep-resource-type"></a><span data-ttu-id="ebe6f-103">Тип ресурса Провисионингстеп</span><span class="sxs-lookup"><span data-stu-id="ebe6f-103">provisioningStep resource type</span></span>

<span data-ttu-id="ebe6f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebe6f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebe6f-105">Описывает действия, предпринимаемые для выполнения действия.</span><span class="sxs-lookup"><span data-stu-id="ebe6f-105">Describes the steps taken to perform an action.</span></span>

## <a name="properties"></a><span data-ttu-id="ebe6f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ebe6f-106">Properties</span></span>

| <span data-ttu-id="ebe6f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ebe6f-107">Property</span></span>     | <span data-ttu-id="ebe6f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ebe6f-108">Type</span></span>        | <span data-ttu-id="ebe6f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ebe6f-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ebe6f-110">description</span><span class="sxs-lookup"><span data-stu-id="ebe6f-110">description</span></span>|<span data-ttu-id="ebe6f-111">String</span><span class="sxs-lookup"><span data-stu-id="ebe6f-111">String</span></span>|<span data-ttu-id="ebe6f-112">Сводка действий, произошедших на этапе.</span><span class="sxs-lookup"><span data-stu-id="ebe6f-112">Summary of what occurred during the step.</span></span>|
|<span data-ttu-id="ebe6f-113">details</span><span class="sxs-lookup"><span data-stu-id="ebe6f-113">details</span></span>|[<span data-ttu-id="ebe6f-114">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="ebe6f-114">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="ebe6f-115">Сведения о том, что произошло на этапе.</span><span class="sxs-lookup"><span data-stu-id="ebe6f-115">Details of what occurred during the step.</span></span>|
|<span data-ttu-id="ebe6f-116">name</span><span class="sxs-lookup"><span data-stu-id="ebe6f-116">name</span></span>|<span data-ttu-id="ebe6f-117">String</span><span class="sxs-lookup"><span data-stu-id="ebe6f-117">String</span></span>|<span data-ttu-id="ebe6f-118">Имя этапа.</span><span class="sxs-lookup"><span data-stu-id="ebe6f-118">Name of the step.</span></span>|
|<span data-ttu-id="ebe6f-119">провисионингстептипе</span><span class="sxs-lookup"><span data-stu-id="ebe6f-119">provisioningStepType</span></span>|<span data-ttu-id="ebe6f-120">String</span><span class="sxs-lookup"><span data-stu-id="ebe6f-120">String</span></span>| <span data-ttu-id="ebe6f-121">Тип этапа.</span><span class="sxs-lookup"><span data-stu-id="ebe6f-121">Type of step.</span></span> <span data-ttu-id="ebe6f-122">Возможные значения: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="ebe6f-122">Possible values are: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="ebe6f-123">status</span><span class="sxs-lookup"><span data-stu-id="ebe6f-123">status</span></span>|<span data-ttu-id="ebe6f-124">String</span><span class="sxs-lookup"><span data-stu-id="ebe6f-124">String</span></span>| <span data-ttu-id="ebe6f-125">Состояние этапа.</span><span class="sxs-lookup"><span data-stu-id="ebe6f-125">Status of the step.</span></span> <span data-ttu-id="ebe6f-126">Возможные значения: `success` ,, `warning`  `failure` , `skipped` , `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="ebe6f-126">Possible values are: `success`, `warning`,  `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ebe6f-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ebe6f-127">JSON representation</span></span>

<span data-ttu-id="ebe6f-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ebe6f-128">The following is a JSON representation of the resource.</span></span>

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



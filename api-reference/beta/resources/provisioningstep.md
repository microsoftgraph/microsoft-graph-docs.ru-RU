---
title: Тип ресурса Провисионингстеп
description: 'Описывает действия, предпринимаемые для выполнения действия. '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1658114615c4532f0a7f9b9f5ad3c3a25deff81b
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349437"
---
# <a name="provisioningstep-resource-type"></a><span data-ttu-id="56f7b-103">Тип ресурса Провисионингстеп</span><span class="sxs-lookup"><span data-stu-id="56f7b-103">provisioningStep resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56f7b-104">Описывает действия, предпринимаемые для выполнения действия.</span><span class="sxs-lookup"><span data-stu-id="56f7b-104">Describes the steps taken to perform an action.</span></span>

## <a name="properties"></a><span data-ttu-id="56f7b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="56f7b-105">Properties</span></span>

| <span data-ttu-id="56f7b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="56f7b-106">Property</span></span>     | <span data-ttu-id="56f7b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="56f7b-107">Type</span></span>        | <span data-ttu-id="56f7b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="56f7b-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="56f7b-109">description</span><span class="sxs-lookup"><span data-stu-id="56f7b-109">description</span></span>|<span data-ttu-id="56f7b-110">String</span><span class="sxs-lookup"><span data-stu-id="56f7b-110">String</span></span>|<span data-ttu-id="56f7b-111">Сводка действий, произошедших на этапе.</span><span class="sxs-lookup"><span data-stu-id="56f7b-111">Summary of what occurred during the step.</span></span>|
|<span data-ttu-id="56f7b-112">details</span><span class="sxs-lookup"><span data-stu-id="56f7b-112">details</span></span>|[<span data-ttu-id="56f7b-113">Детаилсинфо</span><span class="sxs-lookup"><span data-stu-id="56f7b-113">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="56f7b-114">Сведения о том, что произошло на этапе.</span><span class="sxs-lookup"><span data-stu-id="56f7b-114">Details of what occurred during the step.</span></span>|
|<span data-ttu-id="56f7b-115">name</span><span class="sxs-lookup"><span data-stu-id="56f7b-115">name</span></span>|<span data-ttu-id="56f7b-116">String</span><span class="sxs-lookup"><span data-stu-id="56f7b-116">String</span></span>|<span data-ttu-id="56f7b-117">Имя этапа.</span><span class="sxs-lookup"><span data-stu-id="56f7b-117">Name of the step.</span></span>|
|<span data-ttu-id="56f7b-118">Провисионингстептипе</span><span class="sxs-lookup"><span data-stu-id="56f7b-118">provisioningStepType</span></span>|<span data-ttu-id="56f7b-119">String</span><span class="sxs-lookup"><span data-stu-id="56f7b-119">String</span></span>| <span data-ttu-id="56f7b-120">Тип этапа.</span><span class="sxs-lookup"><span data-stu-id="56f7b-120">Type of step.</span></span> <span data-ttu-id="56f7b-121">Возможные значения: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="56f7b-121">Possible values are: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="56f7b-122">status</span><span class="sxs-lookup"><span data-stu-id="56f7b-122">status</span></span>|<span data-ttu-id="56f7b-123">String</span><span class="sxs-lookup"><span data-stu-id="56f7b-123">String</span></span>| <span data-ttu-id="56f7b-124">Состояние этапа.</span><span class="sxs-lookup"><span data-stu-id="56f7b-124">Status of the step.</span></span> <span data-ttu-id="56f7b-125">Возможные значения: `success`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="56f7b-125">Possible values are: `success`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="56f7b-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="56f7b-126">JSON representation</span></span>

<span data-ttu-id="56f7b-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56f7b-127">The following is a JSON representation of the resource.</span></span>

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

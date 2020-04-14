---
title: Тип ресурса Провисионингстеп
description: 'Описывает действия, предпринимаемые для выполнения действия. '
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b0ae3d280d6d9dfc8877739b1003ae0c51f6acd6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43446563"
---
# <a name="provisioningstep-resource-type"></a><span data-ttu-id="5a171-103">Тип ресурса Провисионингстеп</span><span class="sxs-lookup"><span data-stu-id="5a171-103">provisioningStep resource type</span></span>

<span data-ttu-id="5a171-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a171-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a171-105">Описывает действия, предпринимаемые для выполнения действия.</span><span class="sxs-lookup"><span data-stu-id="5a171-105">Describes the steps taken to perform an action.</span></span>

## <a name="properties"></a><span data-ttu-id="5a171-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5a171-106">Properties</span></span>

| <span data-ttu-id="5a171-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a171-107">Property</span></span>     | <span data-ttu-id="5a171-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5a171-108">Type</span></span>        | <span data-ttu-id="5a171-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5a171-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5a171-110">description</span><span class="sxs-lookup"><span data-stu-id="5a171-110">description</span></span>|<span data-ttu-id="5a171-111">String</span><span class="sxs-lookup"><span data-stu-id="5a171-111">String</span></span>|<span data-ttu-id="5a171-112">Сводка действий, произошедших на этапе.</span><span class="sxs-lookup"><span data-stu-id="5a171-112">Summary of what occurred during the step.</span></span>|
|<span data-ttu-id="5a171-113">details</span><span class="sxs-lookup"><span data-stu-id="5a171-113">details</span></span>|[<span data-ttu-id="5a171-114">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="5a171-114">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="5a171-115">Сведения о том, что произошло на этапе.</span><span class="sxs-lookup"><span data-stu-id="5a171-115">Details of what occurred during the step.</span></span>|
|<span data-ttu-id="5a171-116">name</span><span class="sxs-lookup"><span data-stu-id="5a171-116">name</span></span>|<span data-ttu-id="5a171-117">String</span><span class="sxs-lookup"><span data-stu-id="5a171-117">String</span></span>|<span data-ttu-id="5a171-118">Имя этапа.</span><span class="sxs-lookup"><span data-stu-id="5a171-118">Name of the step.</span></span>|
|<span data-ttu-id="5a171-119">провисионингстептипе</span><span class="sxs-lookup"><span data-stu-id="5a171-119">provisioningStepType</span></span>|<span data-ttu-id="5a171-120">String</span><span class="sxs-lookup"><span data-stu-id="5a171-120">String</span></span>| <span data-ttu-id="5a171-121">Тип этапа.</span><span class="sxs-lookup"><span data-stu-id="5a171-121">Type of step.</span></span> <span data-ttu-id="5a171-122">Возможные значения: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="5a171-122">Possible values are: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="5a171-123">status</span><span class="sxs-lookup"><span data-stu-id="5a171-123">status</span></span>|<span data-ttu-id="5a171-124">String</span><span class="sxs-lookup"><span data-stu-id="5a171-124">String</span></span>| <span data-ttu-id="5a171-125">Состояние этапа.</span><span class="sxs-lookup"><span data-stu-id="5a171-125">Status of the step.</span></span> <span data-ttu-id="5a171-126">Возможные значения: `success`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="5a171-126">Possible values are: `success`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5a171-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5a171-127">JSON representation</span></span>

<span data-ttu-id="5a171-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a171-128">The following is a JSON representation of the resource.</span></span>

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

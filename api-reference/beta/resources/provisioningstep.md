---
title: Тип ресурса Провисионингстеп
description: 'Описывает действия, предпринимаемые для выполнения действия. '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4275730cfd7c9c9c58496b674062ffedb5d7a6cc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521329"
---
# <a name="provisioningstep-resource-type"></a><span data-ttu-id="9c357-103">Тип ресурса Провисионингстеп</span><span class="sxs-lookup"><span data-stu-id="9c357-103">provisioningStep resource type</span></span>

<span data-ttu-id="9c357-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9c357-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c357-105">Описывает действия, предпринимаемые для выполнения действия.</span><span class="sxs-lookup"><span data-stu-id="9c357-105">Describes the steps taken to perform an action.</span></span>

## <a name="properties"></a><span data-ttu-id="9c357-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9c357-106">Properties</span></span>

| <span data-ttu-id="9c357-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9c357-107">Property</span></span>     | <span data-ttu-id="9c357-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9c357-108">Type</span></span>        | <span data-ttu-id="9c357-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9c357-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9c357-110">description</span><span class="sxs-lookup"><span data-stu-id="9c357-110">description</span></span>|<span data-ttu-id="9c357-111">String</span><span class="sxs-lookup"><span data-stu-id="9c357-111">String</span></span>|<span data-ttu-id="9c357-112">Сводка действий, произошедших на этапе.</span><span class="sxs-lookup"><span data-stu-id="9c357-112">Summary of what occurred during the step.</span></span>|
|<span data-ttu-id="9c357-113">подробности</span><span class="sxs-lookup"><span data-stu-id="9c357-113">details</span></span>|[<span data-ttu-id="9c357-114">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="9c357-114">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="9c357-115">Сведения о том, что произошло на этапе.</span><span class="sxs-lookup"><span data-stu-id="9c357-115">Details of what occurred during the step.</span></span>|
|<span data-ttu-id="9c357-116">name</span><span class="sxs-lookup"><span data-stu-id="9c357-116">name</span></span>|<span data-ttu-id="9c357-117">String</span><span class="sxs-lookup"><span data-stu-id="9c357-117">String</span></span>|<span data-ttu-id="9c357-118">Имя этапа.</span><span class="sxs-lookup"><span data-stu-id="9c357-118">Name of the step.</span></span>|
|<span data-ttu-id="9c357-119">провисионингстептипе</span><span class="sxs-lookup"><span data-stu-id="9c357-119">provisioningStepType</span></span>|<span data-ttu-id="9c357-120">String</span><span class="sxs-lookup"><span data-stu-id="9c357-120">String</span></span>| <span data-ttu-id="9c357-121">Тип этапа.</span><span class="sxs-lookup"><span data-stu-id="9c357-121">Type of step.</span></span> <span data-ttu-id="9c357-122">Возможные значения: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="9c357-122">Possible values are: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="9c357-123">status</span><span class="sxs-lookup"><span data-stu-id="9c357-123">status</span></span>|<span data-ttu-id="9c357-124">String</span><span class="sxs-lookup"><span data-stu-id="9c357-124">String</span></span>| <span data-ttu-id="9c357-125">Состояние этапа.</span><span class="sxs-lookup"><span data-stu-id="9c357-125">Status of the step.</span></span> <span data-ttu-id="9c357-126">Возможные значения: `success`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="9c357-126">Possible values are: `success`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9c357-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9c357-127">JSON representation</span></span>

<span data-ttu-id="9c357-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9c357-128">The following is a JSON representation of the resource.</span></span>

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

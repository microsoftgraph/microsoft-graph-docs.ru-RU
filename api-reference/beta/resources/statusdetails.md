---
title: Тип ресурса statusDetails
description: Описывает состояние события предоставления и связанные ошибки.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 81ea4a75970e37a360c402aced66f01ccb9e7c47
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292614"
---
# <a name="statusdetails-resource-type"></a><span data-ttu-id="b763a-103">Тип ресурса statusDetails</span><span class="sxs-lookup"><span data-stu-id="b763a-103">statusDetails resource type</span></span>

<span data-ttu-id="b763a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b763a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b763a-105">Описывает состояние события предоставления и связанные ошибки.</span><span class="sxs-lookup"><span data-stu-id="b763a-105">Describes the status of the provisioning event and the associated errors.</span></span> <span data-ttu-id="b763a-106">Он наследуется от [statusBase и](/graph/api/resources/statusbase) используется только в том случае, если задан статус `failure` .</span><span class="sxs-lookup"><span data-stu-id="b763a-106">It is inherited from [statusBase](/graph/api/resources/statusbase) and only used when status is set to `failure`.</span></span>  

## <a name="properties"></a><span data-ttu-id="b763a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b763a-107">Properties</span></span>

| <span data-ttu-id="b763a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b763a-108">Property</span></span>     | <span data-ttu-id="b763a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b763a-109">Type</span></span>        | <span data-ttu-id="b763a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b763a-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b763a-111">status</span><span class="sxs-lookup"><span data-stu-id="b763a-111">status</span></span>|<span data-ttu-id="b763a-112">String</span><span class="sxs-lookup"><span data-stu-id="b763a-112">String</span></span>|<span data-ttu-id="b763a-113">Возможные значения: `success`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="b763a-113">Possible values are: `success`, `failure`, `skipped`, `unknownFutureValue`.</span></span> <span data-ttu-id="b763a-114">Наследуется от statusBase.</span><span class="sxs-lookup"><span data-stu-id="b763a-114">Inherited from statusBase.</span></span>|
|<span data-ttu-id="b763a-115">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="b763a-115">additionalDetails</span></span>|<span data-ttu-id="b763a-116">String</span><span class="sxs-lookup"><span data-stu-id="b763a-116">String</span></span>|<span data-ttu-id="b763a-117">Дополнительные сведения в случае ошибки.</span><span class="sxs-lookup"><span data-stu-id="b763a-117">Additional details in case of error.</span></span>|
|<span data-ttu-id="b763a-118">errorCategory</span><span class="sxs-lookup"><span data-stu-id="b763a-118">errorCategory</span></span>|<span data-ttu-id="b763a-119">String</span><span class="sxs-lookup"><span data-stu-id="b763a-119">String</span></span>|<span data-ttu-id="b763a-120">Классифицировать код ошибки.</span><span class="sxs-lookup"><span data-stu-id="b763a-120">Categorizes the error code.</span></span> <span data-ttu-id="b763a-121">Возможные значения: `Failure`, `NonServiceFailure`, `Success`.</span><span class="sxs-lookup"><span data-stu-id="b763a-121">Possible values are `Failure`, `NonServiceFailure`, `Success`.</span></span>|
|<span data-ttu-id="b763a-122">errorCode</span><span class="sxs-lookup"><span data-stu-id="b763a-122">errorCode</span></span>|<span data-ttu-id="b763a-123">String</span><span class="sxs-lookup"><span data-stu-id="b763a-123">String</span></span>|<span data-ttu-id="b763a-124">Уникальный код ошибки, если таковое произошло.</span><span class="sxs-lookup"><span data-stu-id="b763a-124">Unique error code if any occurred.</span></span> [<span data-ttu-id="b763a-125">Подробнее</span><span class="sxs-lookup"><span data-stu-id="b763a-125">Learn more</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs#error-codes)|
|<span data-ttu-id="b763a-126">reason</span><span class="sxs-lookup"><span data-stu-id="b763a-126">reason</span></span>|<span data-ttu-id="b763a-127">String</span><span class="sxs-lookup"><span data-stu-id="b763a-127">String</span></span>|<span data-ttu-id="b763a-128">Суммирует состояние и описывает, почему это состояние произошло.</span><span class="sxs-lookup"><span data-stu-id="b763a-128">Summarizes the status and describes why the status happened.</span></span>|
|<span data-ttu-id="b763a-129">recommendedAction</span><span class="sxs-lookup"><span data-stu-id="b763a-129">recommendedAction</span></span>|<span data-ttu-id="b763a-130">String</span><span class="sxs-lookup"><span data-stu-id="b763a-130">String</span></span>|<span data-ttu-id="b763a-131">Предоставляет разрешение соответствующей ошибки.</span><span class="sxs-lookup"><span data-stu-id="b763a-131">Provides the resolution for the corresponding error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b763a-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b763a-132">JSON representation</span></span>

<span data-ttu-id="b763a-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b763a-133">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.statusDetails",
  "baseType": "microsoft.graph.statusBase"
}-->

```json
{
  "status": "failure",
  "additionalDetails": "String",
  "errorCategory": "String",
  "errorCode": "String",
  "reason": "String",
  "recommendedAction": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "statusDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



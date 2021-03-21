---
title: тип ресурса statusDetails
description: Описывает состояние события подготовка и связанные с ним ошибки.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: d817c0aa46dde6b49debd849d8fd2ae61e06a672
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956822"
---
# <a name="statusdetails-resource-type"></a><span data-ttu-id="d6f4b-103">тип ресурса statusDetails</span><span class="sxs-lookup"><span data-stu-id="d6f4b-103">statusDetails resource type</span></span>

<span data-ttu-id="d6f4b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6f4b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6f4b-105">Описывает состояние события подготовка и связанные с ним ошибки.</span><span class="sxs-lookup"><span data-stu-id="d6f4b-105">Describes the status of the provisioning event and the associated errors.</span></span> <span data-ttu-id="d6f4b-106">Он наследуется из [statusBase и](/graph/api/resources/statusbase) используется только при задании состояния `failure` .</span><span class="sxs-lookup"><span data-stu-id="d6f4b-106">It is inherited from [statusBase](/graph/api/resources/statusbase) and only used when status is set to `failure`.</span></span>  

## <a name="properties"></a><span data-ttu-id="d6f4b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d6f4b-107">Properties</span></span>

| <span data-ttu-id="d6f4b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6f4b-108">Property</span></span>     | <span data-ttu-id="d6f4b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d6f4b-109">Type</span></span>        | <span data-ttu-id="d6f4b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d6f4b-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d6f4b-111">status</span><span class="sxs-lookup"><span data-stu-id="d6f4b-111">status</span></span>|<span data-ttu-id="d6f4b-112">statusBase</span><span class="sxs-lookup"><span data-stu-id="d6f4b-112">statusBase</span></span>|<span data-ttu-id="d6f4b-113">Возможные значения: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="d6f4b-113">Possible values are: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span></span> <span data-ttu-id="d6f4b-114">Унаследованный от statusBase.</span><span class="sxs-lookup"><span data-stu-id="d6f4b-114">Inherited from statusBase.</span></span>|
|<span data-ttu-id="d6f4b-115">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="d6f4b-115">additionalDetails</span></span>|<span data-ttu-id="d6f4b-116">Строка</span><span class="sxs-lookup"><span data-stu-id="d6f4b-116">String</span></span>|<span data-ttu-id="d6f4b-117">Дополнительные сведения в случае ошибки.</span><span class="sxs-lookup"><span data-stu-id="d6f4b-117">Additional details in case of error.</span></span>|
|<span data-ttu-id="d6f4b-118">errorCategory</span><span class="sxs-lookup"><span data-stu-id="d6f4b-118">errorCategory</span></span>|<span data-ttu-id="d6f4b-119">Строка</span><span class="sxs-lookup"><span data-stu-id="d6f4b-119">String</span></span>|<span data-ttu-id="d6f4b-120">Классифицировать код ошибки.</span><span class="sxs-lookup"><span data-stu-id="d6f4b-120">Categorizes the error code.</span></span> <span data-ttu-id="d6f4b-121">Возможные значения: `Failure`, `NonServiceFailure`, `Success`.</span><span class="sxs-lookup"><span data-stu-id="d6f4b-121">Possible values are `Failure`, `NonServiceFailure`, `Success`.</span></span>|
|<span data-ttu-id="d6f4b-122">errorCode</span><span class="sxs-lookup"><span data-stu-id="d6f4b-122">errorCode</span></span>|<span data-ttu-id="d6f4b-123">String</span><span class="sxs-lookup"><span data-stu-id="d6f4b-123">String</span></span>|<span data-ttu-id="d6f4b-124">Уникальный код ошибки, если таковое произошло.</span><span class="sxs-lookup"><span data-stu-id="d6f4b-124">Unique error code if any occurred.</span></span> [<span data-ttu-id="d6f4b-125">Подробнее</span><span class="sxs-lookup"><span data-stu-id="d6f4b-125">Learn more</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs#error-codes)|
|<span data-ttu-id="d6f4b-126">reason</span><span class="sxs-lookup"><span data-stu-id="d6f4b-126">reason</span></span>|<span data-ttu-id="d6f4b-127">Строка</span><span class="sxs-lookup"><span data-stu-id="d6f4b-127">String</span></span>|<span data-ttu-id="d6f4b-128">Суммирует состояние и описывает причины, по которым произошел этот статус.</span><span class="sxs-lookup"><span data-stu-id="d6f4b-128">Summarizes the status and describes why the status happened.</span></span>|
|<span data-ttu-id="d6f4b-129">recommendedAction</span><span class="sxs-lookup"><span data-stu-id="d6f4b-129">recommendedAction</span></span>|<span data-ttu-id="d6f4b-130">Строка</span><span class="sxs-lookup"><span data-stu-id="d6f4b-130">String</span></span>|<span data-ttu-id="d6f4b-131">Обеспечивает разрешение соответствующей ошибки.</span><span class="sxs-lookup"><span data-stu-id="d6f4b-131">Provides the resolution for the corresponding error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d6f4b-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d6f4b-132">JSON representation</span></span>

<span data-ttu-id="d6f4b-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6f4b-133">The following is a JSON representation of the resource.</span></span>

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



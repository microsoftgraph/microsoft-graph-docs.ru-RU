---
title: тип ресурса statusDetails
description: Описывает состояние события подготовка и связанные с ним ошибки.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: ae11d370fb0a92a03e497aec75550f5407934839
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231908"
---
# <a name="statusdetails-resource-type-deprecated"></a><span data-ttu-id="23b3a-103">тип ресурса statusDetails (неподготовленный)</span><span class="sxs-lookup"><span data-stu-id="23b3a-103">statusDetails resource type (deprecated)</span></span>

<span data-ttu-id="23b3a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23b3a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
>[!CAUTION] 
> <span data-ttu-id="23b3a-105">API statusDetails обесценена и прекратит возвращать данные om 31 декабря 2021 г.</span><span class="sxs-lookup"><span data-stu-id="23b3a-105">The statusDetails API is deprecated and will stop returning data om December 31, 2021.</span></span> <span data-ttu-id="23b3a-106">Используйте новый [тип provisioningStatusInfo.](provisioningstatusinfo.md)</span><span class="sxs-lookup"><span data-stu-id="23b3a-106">Please use the new [provisioningStatusInfo](provisioningstatusinfo.md) type.</span></span>

<span data-ttu-id="23b3a-107">Описывает состояние события подготовка и связанные с ним ошибки.</span><span class="sxs-lookup"><span data-stu-id="23b3a-107">Describes the status of the provisioning event and the associated errors.</span></span> <span data-ttu-id="23b3a-108">Он наследуется из [statusBase и](/graph/api/resources/statusbase) используется только при задании состояния `failure` .</span><span class="sxs-lookup"><span data-stu-id="23b3a-108">It is inherited from [statusBase](/graph/api/resources/statusbase) and only used when status is set to `failure`.</span></span>  

## <a name="properties"></a><span data-ttu-id="23b3a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="23b3a-109">Properties</span></span>

| <span data-ttu-id="23b3a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="23b3a-110">Property</span></span>     | <span data-ttu-id="23b3a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="23b3a-111">Type</span></span>        | <span data-ttu-id="23b3a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="23b3a-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="23b3a-113">status</span><span class="sxs-lookup"><span data-stu-id="23b3a-113">status</span></span>|<span data-ttu-id="23b3a-114">statusBase</span><span class="sxs-lookup"><span data-stu-id="23b3a-114">statusBase</span></span>|<span data-ttu-id="23b3a-115">Возможные значения: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="23b3a-115">Possible values are: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span></span> <span data-ttu-id="23b3a-116">Унаследованный от statusBase.</span><span class="sxs-lookup"><span data-stu-id="23b3a-116">Inherited from statusBase.</span></span>|
|<span data-ttu-id="23b3a-117">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="23b3a-117">additionalDetails</span></span>|<span data-ttu-id="23b3a-118">String</span><span class="sxs-lookup"><span data-stu-id="23b3a-118">String</span></span>|<span data-ttu-id="23b3a-119">Дополнительные сведения в случае ошибки.</span><span class="sxs-lookup"><span data-stu-id="23b3a-119">Additional details in case of error.</span></span>|
|<span data-ttu-id="23b3a-120">errorCategory</span><span class="sxs-lookup"><span data-stu-id="23b3a-120">errorCategory</span></span>|<span data-ttu-id="23b3a-121">String</span><span class="sxs-lookup"><span data-stu-id="23b3a-121">String</span></span>|<span data-ttu-id="23b3a-122">Классифицировать код ошибки.</span><span class="sxs-lookup"><span data-stu-id="23b3a-122">Categorizes the error code.</span></span> <span data-ttu-id="23b3a-123">Возможные значения: `Failure`, `NonServiceFailure`, `Success`.</span><span class="sxs-lookup"><span data-stu-id="23b3a-123">Possible values are `Failure`, `NonServiceFailure`, `Success`.</span></span>|
|<span data-ttu-id="23b3a-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="23b3a-124">errorCode</span></span>|<span data-ttu-id="23b3a-125">String</span><span class="sxs-lookup"><span data-stu-id="23b3a-125">String</span></span>|<span data-ttu-id="23b3a-126">Уникальный код ошибки, если таковое произошло.</span><span class="sxs-lookup"><span data-stu-id="23b3a-126">Unique error code if any occurred.</span></span> [<span data-ttu-id="23b3a-127">Подробнее</span><span class="sxs-lookup"><span data-stu-id="23b3a-127">Learn more</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs#error-codes)|
|<span data-ttu-id="23b3a-128">reason</span><span class="sxs-lookup"><span data-stu-id="23b3a-128">reason</span></span>|<span data-ttu-id="23b3a-129">String</span><span class="sxs-lookup"><span data-stu-id="23b3a-129">String</span></span>|<span data-ttu-id="23b3a-130">Суммирует состояние и описывает причины, по которым произошел этот статус.</span><span class="sxs-lookup"><span data-stu-id="23b3a-130">Summarizes the status and describes why the status happened.</span></span>|
|<span data-ttu-id="23b3a-131">recommendedAction</span><span class="sxs-lookup"><span data-stu-id="23b3a-131">recommendedAction</span></span>|<span data-ttu-id="23b3a-132">String</span><span class="sxs-lookup"><span data-stu-id="23b3a-132">String</span></span>|<span data-ttu-id="23b3a-133">Обеспечивает разрешение соответствующей ошибки.</span><span class="sxs-lookup"><span data-stu-id="23b3a-133">Provides the resolution for the corresponding error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="23b3a-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="23b3a-134">JSON representation</span></span>

<span data-ttu-id="23b3a-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="23b3a-135">The following is a JSON representation of the resource.</span></span>

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



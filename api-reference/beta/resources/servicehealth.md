---
title: тип ресурса serviceHealth
description: Представляет сведения о состоянии здоровья службы.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: c11750bbffe64315c6263a26d7dbab333f42b7cf
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109238"
---
# <a name="servicehealth-resource-type"></a><span data-ttu-id="02213-103">тип ресурса serviceHealth</span><span class="sxs-lookup"><span data-stu-id="02213-103">serviceHealth resource type</span></span>

<span data-ttu-id="02213-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02213-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02213-105">Представляет сведения о состоянии здоровья службы.</span><span class="sxs-lookup"><span data-stu-id="02213-105">Represents the health information of a service.</span></span>

## <a name="methods"></a><span data-ttu-id="02213-106">Методы</span><span class="sxs-lookup"><span data-stu-id="02213-106">Methods</span></span>
|<span data-ttu-id="02213-107">Метод</span><span class="sxs-lookup"><span data-stu-id="02213-107">Method</span></span>|<span data-ttu-id="02213-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="02213-108">Return type</span></span>|<span data-ttu-id="02213-109">Описание</span><span class="sxs-lookup"><span data-stu-id="02213-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="02213-110">Get serviceHealth</span><span class="sxs-lookup"><span data-stu-id="02213-110">Get serviceHealth</span></span>](../api/servicehealth-get.md)|[<span data-ttu-id="02213-111">serviceHealth</span><span class="sxs-lookup"><span data-stu-id="02213-111">serviceHealth</span></span>](../resources/servicehealth.md)|<span data-ttu-id="02213-112">Извлечение свойств и связей объекта [serviceHealth.](../resources/servicehealth.md)</span><span class="sxs-lookup"><span data-stu-id="02213-112">Retrieve the properties and relationships of a [serviceHealth](../resources/servicehealth.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="02213-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="02213-113">Properties</span></span>
|<span data-ttu-id="02213-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="02213-114">Property</span></span>|<span data-ttu-id="02213-115">Тип</span><span class="sxs-lookup"><span data-stu-id="02213-115">Type</span></span>|<span data-ttu-id="02213-116">Описание</span><span class="sxs-lookup"><span data-stu-id="02213-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02213-117">id</span><span class="sxs-lookup"><span data-stu-id="02213-117">id</span></span>|<span data-ttu-id="02213-118">Строка</span><span class="sxs-lookup"><span data-stu-id="02213-118">String</span></span>|<span data-ttu-id="02213-119">ID службы.</span><span class="sxs-lookup"><span data-stu-id="02213-119">The service id.</span></span>|
|<span data-ttu-id="02213-120">service</span><span class="sxs-lookup"><span data-stu-id="02213-120">service</span></span>|<span data-ttu-id="02213-121">String</span><span class="sxs-lookup"><span data-stu-id="02213-121">String</span></span>|<span data-ttu-id="02213-122">Имя службы.</span><span class="sxs-lookup"><span data-stu-id="02213-122">The service name.</span></span>|
|<span data-ttu-id="02213-123">status</span><span class="sxs-lookup"><span data-stu-id="02213-123">status</span></span>|<span data-ttu-id="02213-124">serviceHealthStatus</span><span class="sxs-lookup"><span data-stu-id="02213-124">serviceHealthStatus</span></span>|<span data-ttu-id="02213-125">Покажите состояние состояния службы overral.</span><span class="sxs-lookup"><span data-stu-id="02213-125">Show the overral service health status.</span></span> <span data-ttu-id="02213-126">Возможные значения: `serviceOperational` `investigating` , , , , `restoringService` , `verifyingService` , `serviceRestored` `postIncidentReviewPublished` `serviceDegradation` , `serviceInterruption` `extendedRecovery` `falsePositive` `investigationSuspended` `resolved` `mitigatedExternal` `mitigated` `resolvedExternal` `confirmed` `reported` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="02213-126">Possible values are: `serviceOperational`, `investigating`, `restoringService`, `verifyingService`, `serviceRestored`, `postIncidentReviewPublished`, `serviceDegradation`, `serviceInterruption`, `extendedRecovery`, `falsePositive`, `investigationSuspended`, `resolved`, `mitigatedExternal`, `mitigated`, `resolvedExternal`, `confirmed`, `reported`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="02213-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="02213-127">Relationships</span></span>
|<span data-ttu-id="02213-128">Связь</span><span class="sxs-lookup"><span data-stu-id="02213-128">Relationship</span></span>|<span data-ttu-id="02213-129">Тип</span><span class="sxs-lookup"><span data-stu-id="02213-129">Type</span></span>|<span data-ttu-id="02213-130">Описание</span><span class="sxs-lookup"><span data-stu-id="02213-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02213-131">проблемы</span><span class="sxs-lookup"><span data-stu-id="02213-131">issues</span></span>|<span data-ttu-id="02213-132">[Collection(serviceHealthIssue)](../resources/servicehealthissue.md)</span><span class="sxs-lookup"><span data-stu-id="02213-132">Collection([serviceHealthIssue](../resources/servicehealthissue.md))</span></span>|<span data-ttu-id="02213-133">В службе произошел набор проблем с подробными сведениями по каждой проблеме.</span><span class="sxs-lookup"><span data-stu-id="02213-133">A collection of issues happened on the service, with detailed information for each issue.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="02213-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="02213-134">JSON representation</span></span>
<span data-ttu-id="02213-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="02213-135">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceHealth",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceHealth",
  "service": "String",
  "status": "String",
  "id": "String (identifier)"
}
```


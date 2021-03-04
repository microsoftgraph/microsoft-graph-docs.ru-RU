---
title: тип ресурса tagOperation
description: Представляет операцию, которая обрабатывает применение тегов к документам в наборе отзывов на основе запроса набора отзывов.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 2af9b255e643a46f5f065b3caf62fda0ae9967a4
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447546"
---
# <a name="tagoperation-resource-type"></a><span data-ttu-id="630c7-103">тип ресурса tagOperation</span><span class="sxs-lookup"><span data-stu-id="630c7-103">tagOperation resource type</span></span>

<span data-ttu-id="630c7-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="630c7-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="630c7-105">Представляет операцию, которая обрабатывает применение тегов к документам в наборе отзывов на основе запроса набора отзывов.</span><span class="sxs-lookup"><span data-stu-id="630c7-105">Represents the operation that handles applying tags to documents in a review set based on a review set query.</span></span>

<span data-ttu-id="630c7-106">Наследует [от caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="630c7-106">Inherits from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>

## <a name="methods"></a><span data-ttu-id="630c7-107">Methods</span><span class="sxs-lookup"><span data-stu-id="630c7-107">Methods</span></span>

<span data-ttu-id="630c7-108">Нет.</span><span class="sxs-lookup"><span data-stu-id="630c7-108">None.</span></span>

## <a name="properties"></a><span data-ttu-id="630c7-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="630c7-109">Properties</span></span>

|<span data-ttu-id="630c7-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="630c7-110">Property</span></span>|<span data-ttu-id="630c7-111">Тип</span><span class="sxs-lookup"><span data-stu-id="630c7-111">Type</span></span>|<span data-ttu-id="630c7-112">Описание</span><span class="sxs-lookup"><span data-stu-id="630c7-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="630c7-113">action</span><span class="sxs-lookup"><span data-stu-id="630c7-113">action</span></span>|[<span data-ttu-id="630c7-114">microsoft.graph.ediscovery.caseAction</span><span class="sxs-lookup"><span data-stu-id="630c7-114">microsoft.graph.ediscovery.caseAction</span></span>](../resources/ediscovery-caseoperation.md#caseaction-values)| <span data-ttu-id="630c7-115">Действие случая для этой сущности всегда будет `applyTags` .</span><span class="sxs-lookup"><span data-stu-id="630c7-115">The case action for this entity will always be `applyTags`.</span></span> <span data-ttu-id="630c7-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="630c7-116">Read-only.</span></span> <span data-ttu-id="630c7-117">Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="630c7-117">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="630c7-118">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="630c7-118">completedDateTime</span></span>|<span data-ttu-id="630c7-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="630c7-119">DateTimeOffset</span></span>|<span data-ttu-id="630c7-120">Дата и время завершения операции.</span><span class="sxs-lookup"><span data-stu-id="630c7-120">The date and time the operation was completed.</span></span> <span data-ttu-id="630c7-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="630c7-121">Read-only.</span></span> <span data-ttu-id="630c7-122">Унаследованный от [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="630c7-122">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="630c7-123">createdBy</span><span class="sxs-lookup"><span data-stu-id="630c7-123">createdBy</span></span>|[<span data-ttu-id="630c7-124">identitySet</span><span class="sxs-lookup"><span data-stu-id="630c7-124">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="630c7-125">Пользователь, создавший операцию.</span><span class="sxs-lookup"><span data-stu-id="630c7-125">The user who created the operation.</span></span> <span data-ttu-id="630c7-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="630c7-126">Read-only.</span></span> <span data-ttu-id="630c7-127">Унаследованный от [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="630c7-127">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="630c7-128">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="630c7-128">createdDateTime</span></span>|<span data-ttu-id="630c7-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="630c7-129">DateTimeOffset</span></span>|<span data-ttu-id="630c7-130">Дата и время начала операции.</span><span class="sxs-lookup"><span data-stu-id="630c7-130">The date and time the operation was started.</span></span> <span data-ttu-id="630c7-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="630c7-131">Read-only.</span></span> <span data-ttu-id="630c7-132">Унаследованный от [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="630c7-132">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="630c7-133">id</span><span class="sxs-lookup"><span data-stu-id="630c7-133">id</span></span>|<span data-ttu-id="630c7-134">String</span><span class="sxs-lookup"><span data-stu-id="630c7-134">String</span></span>| <span data-ttu-id="630c7-135">ID для операции.</span><span class="sxs-lookup"><span data-stu-id="630c7-135">The ID for the operation.</span></span> <span data-ttu-id="630c7-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="630c7-136">Read-only.</span></span> <span data-ttu-id="630c7-137">Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="630c7-137">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="630c7-138">percentProgress</span><span class="sxs-lookup"><span data-stu-id="630c7-138">percentProgress</span></span>|<span data-ttu-id="630c7-139">Int32</span><span class="sxs-lookup"><span data-stu-id="630c7-139">Int32</span></span>|<span data-ttu-id="630c7-140">Ход операции.</span><span class="sxs-lookup"><span data-stu-id="630c7-140">The progress of the operation.</span></span> <span data-ttu-id="630c7-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="630c7-141">Read-only.</span></span> <span data-ttu-id="630c7-142">Унаследованный от [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="630c7-142">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="630c7-143">resultInfo</span><span class="sxs-lookup"><span data-stu-id="630c7-143">resultInfo</span></span>|[<span data-ttu-id="630c7-144">resultInfo</span><span class="sxs-lookup"><span data-stu-id="630c7-144">resultInfo</span></span>](../resources/resultinfo.md)|<span data-ttu-id="630c7-145">Содержит сведения о результатах, характерных для успешного и неудачного сбоя.</span><span class="sxs-lookup"><span data-stu-id="630c7-145">Contains success and failure-specific result information.</span></span> <span data-ttu-id="630c7-146">Унаследованный от [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="630c7-146">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="630c7-147">status</span><span class="sxs-lookup"><span data-stu-id="630c7-147">status</span></span>|[<span data-ttu-id="630c7-148">microsoft.graph.ediscovery.caseOperationStatus</span><span class="sxs-lookup"><span data-stu-id="630c7-148">microsoft.graph.ediscovery.caseOperationStatus</span></span>](../resources/ediscovery-caseoperation.md#caseoperationstatus-values)|<span data-ttu-id="630c7-149">Состояние операции дела.</span><span class="sxs-lookup"><span data-stu-id="630c7-149">The status of the case operation.</span></span> <span data-ttu-id="630c7-150">Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="630c7-150">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span> <span data-ttu-id="630c7-151">Возможные значения: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="630c7-151">Possible values are: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="630c7-152">Связи</span><span class="sxs-lookup"><span data-stu-id="630c7-152">Relationships</span></span>

<span data-ttu-id="630c7-153">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="630c7-153">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="630c7-154">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="630c7-154">JSON representation</span></span>

<span data-ttu-id="630c7-155">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="630c7-155">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.tagOperation",
  "baseType": "microsoft.graph.ediscovery.caseOperation",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.tagOperation",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "completedDateTime": "String (timestamp)",
  "percentProgress": "Integer",
  "status": "String",
  "action": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo"
  }
}
```

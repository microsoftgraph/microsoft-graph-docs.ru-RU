---
title: тип ресурса addToReviewSetOperation
description: Добавляет результаты sourceCollection в reviewSet
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: d7323fbd6d2d068888d556328fc3ea4e399ab2fe
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447586"
---
# <a name="addtoreviewsetoperation-resource-type"></a><span data-ttu-id="3d653-103">тип ресурса addToReviewSetOperation</span><span class="sxs-lookup"><span data-stu-id="3d653-103">addToReviewSetOperation resource type</span></span>

<span data-ttu-id="3d653-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="3d653-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d653-105">Представляет операцию по добавлению [sourceCollection](../resources/ediscovery-sourcecollection.md) в [reviewSet.](../resources/ediscovery-reviewset.md)</span><span class="sxs-lookup"><span data-stu-id="3d653-105">Represents an operation to add a [sourceCollection](../resources/ediscovery-sourcecollection.md) to a [reviewSet](../resources/ediscovery-reviewset.md).</span></span>

<span data-ttu-id="3d653-106">Наследует [от caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="3d653-106">Inherits from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>

## <a name="methods"></a><span data-ttu-id="3d653-107">Methods</span><span class="sxs-lookup"><span data-stu-id="3d653-107">Methods</span></span>

<span data-ttu-id="3d653-108">Нет.</span><span class="sxs-lookup"><span data-stu-id="3d653-108">None.</span></span>

## <a name="properties"></a><span data-ttu-id="3d653-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="3d653-109">Properties</span></span>

|<span data-ttu-id="3d653-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d653-110">Property</span></span>|<span data-ttu-id="3d653-111">Тип</span><span class="sxs-lookup"><span data-stu-id="3d653-111">Type</span></span>|<span data-ttu-id="3d653-112">Описание</span><span class="sxs-lookup"><span data-stu-id="3d653-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d653-113">action</span><span class="sxs-lookup"><span data-stu-id="3d653-113">action</span></span>|[<span data-ttu-id="3d653-114">microsoft.graph.ediscovery.caseAction</span><span class="sxs-lookup"><span data-stu-id="3d653-114">microsoft.graph.ediscovery.caseAction</span></span>](../resources/ediscovery-caseoperation.md#caseaction-values)| <span data-ttu-id="3d653-115">Действие случая для этой сущности всегда будет `addToReviewSet` .</span><span class="sxs-lookup"><span data-stu-id="3d653-115">The case action for this entity will always be `addToReviewSet`.</span></span> <span data-ttu-id="3d653-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d653-116">Read-only.</span></span> <span data-ttu-id="3d653-117">Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="3d653-117">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="3d653-118">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="3d653-118">completedDateTime</span></span>|<span data-ttu-id="3d653-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d653-119">DateTimeOffset</span></span>|<span data-ttu-id="3d653-120">Дата и время завершения операции.</span><span class="sxs-lookup"><span data-stu-id="3d653-120">The date and time the operation was completed.</span></span> <span data-ttu-id="3d653-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d653-121">Read-only.</span></span> <span data-ttu-id="3d653-122">Унаследованный от [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="3d653-122">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="3d653-123">createdBy</span><span class="sxs-lookup"><span data-stu-id="3d653-123">createdBy</span></span>|[<span data-ttu-id="3d653-124">identitySet</span><span class="sxs-lookup"><span data-stu-id="3d653-124">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="3d653-125">Пользователь, создавший операцию.</span><span class="sxs-lookup"><span data-stu-id="3d653-125">The user who created the operation.</span></span> <span data-ttu-id="3d653-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d653-126">Read-only.</span></span> <span data-ttu-id="3d653-127">Унаследованный от [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="3d653-127">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="3d653-128">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3d653-128">createdDateTime</span></span>|<span data-ttu-id="3d653-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d653-129">DateTimeOffset</span></span>|<span data-ttu-id="3d653-130">Дата и время начала операции.</span><span class="sxs-lookup"><span data-stu-id="3d653-130">The date and time the operation was started.</span></span> <span data-ttu-id="3d653-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d653-131">Read-only.</span></span> <span data-ttu-id="3d653-132">Унаследованный от [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="3d653-132">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="3d653-133">id</span><span class="sxs-lookup"><span data-stu-id="3d653-133">id</span></span>|<span data-ttu-id="3d653-134">String</span><span class="sxs-lookup"><span data-stu-id="3d653-134">String</span></span>| <span data-ttu-id="3d653-135">ID для операции.</span><span class="sxs-lookup"><span data-stu-id="3d653-135">The ID for the operation.</span></span> <span data-ttu-id="3d653-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d653-136">Read-only.</span></span> <span data-ttu-id="3d653-137">Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="3d653-137">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="3d653-138">percentProgress</span><span class="sxs-lookup"><span data-stu-id="3d653-138">percentProgress</span></span>|<span data-ttu-id="3d653-139">Int32</span><span class="sxs-lookup"><span data-stu-id="3d653-139">Int32</span></span>|<span data-ttu-id="3d653-140">Ход операции.</span><span class="sxs-lookup"><span data-stu-id="3d653-140">The progress of the operation.</span></span> <span data-ttu-id="3d653-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d653-141">Read-only.</span></span> <span data-ttu-id="3d653-142">Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="3d653-142">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="3d653-143">resultInfo</span><span class="sxs-lookup"><span data-stu-id="3d653-143">resultInfo</span></span>|[<span data-ttu-id="3d653-144">resultInfo</span><span class="sxs-lookup"><span data-stu-id="3d653-144">resultInfo</span></span>](../resources/resultinfo.md)|<span data-ttu-id="3d653-145">Содержит сведения о результатах, характерных для успешного и неудачного сбоя.</span><span class="sxs-lookup"><span data-stu-id="3d653-145">Contains success and failure-specific result information.</span></span> <span data-ttu-id="3d653-146">Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="3d653-146">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="3d653-147">status</span><span class="sxs-lookup"><span data-stu-id="3d653-147">status</span></span>|[<span data-ttu-id="3d653-148">microsoft.graph.ediscovery.caseOperationStatus</span><span class="sxs-lookup"><span data-stu-id="3d653-148">microsoft.graph.ediscovery.caseOperationStatus</span></span>](../resources/ediscovery-caseoperation.md#caseoperationstatus-values)|<span data-ttu-id="3d653-149">Состояние операции дела.</span><span class="sxs-lookup"><span data-stu-id="3d653-149">The status of the case operation.</span></span> <span data-ttu-id="3d653-150">Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="3d653-150">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span> <span data-ttu-id="3d653-151">Возможные значения: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="3d653-151">Possible values are: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.</span></span>|

### <a name="datacollectionscope-values"></a><span data-ttu-id="3d653-152">значения dataCollectionScope</span><span class="sxs-lookup"><span data-stu-id="3d653-152">dataCollectionScope values</span></span>

|<span data-ttu-id="3d653-153">Member</span><span class="sxs-lookup"><span data-stu-id="3d653-153">Member</span></span>|<span data-ttu-id="3d653-154">Описание</span><span class="sxs-lookup"><span data-stu-id="3d653-154">Description</span></span>|
|:----|-----------|
|<span data-ttu-id="3d653-155">allVersions</span><span class="sxs-lookup"><span data-stu-id="3d653-155">allVersions</span></span>|<span data-ttu-id="3d653-156">Включай все версии файлов с сайтов.</span><span class="sxs-lookup"><span data-stu-id="3d653-156">Include all versions of files from sites.</span></span>|
|<span data-ttu-id="3d653-157">linkedFiles</span><span class="sxs-lookup"><span data-stu-id="3d653-157">linkedFiles</span></span>|<span data-ttu-id="3d653-158">**Включайте облачное** вложение с электронными письмами в коллекцию.</span><span class="sxs-lookup"><span data-stu-id="3d653-158">Include **cloud attachment** with emails in the collection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d653-159">Связи</span><span class="sxs-lookup"><span data-stu-id="3d653-159">Relationships</span></span>

|<span data-ttu-id="3d653-160">Связь</span><span class="sxs-lookup"><span data-stu-id="3d653-160">Relationship</span></span>|<span data-ttu-id="3d653-161">Тип</span><span class="sxs-lookup"><span data-stu-id="3d653-161">Type</span></span>|<span data-ttu-id="3d653-162">Описание</span><span class="sxs-lookup"><span data-stu-id="3d653-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d653-163">reviewSet</span><span class="sxs-lookup"><span data-stu-id="3d653-163">reviewSet</span></span>|[<span data-ttu-id="3d653-164">microsoft.graph.ediscovery.reviewSet</span><span class="sxs-lookup"><span data-stu-id="3d653-164">microsoft.graph.ediscovery.reviewSet</span></span>](../resources/ediscovery-reviewset.md)| <span data-ttu-id="3d653-165">Набор отзывов, к которым добавляются элементы, совпадающие с запросом коллекции источника.</span><span class="sxs-lookup"><span data-stu-id="3d653-165">The review set to which items matching the source collection query are added to.</span></span> |
|<span data-ttu-id="3d653-166">sourceCollection</span><span class="sxs-lookup"><span data-stu-id="3d653-166">sourceCollection</span></span>|[<span data-ttu-id="3d653-167">microsoft.graph.ediscovery.sourceCollection</span><span class="sxs-lookup"><span data-stu-id="3d653-167">microsoft.graph.ediscovery.sourceCollection</span></span>](../resources/ediscovery-sourceCollection.md)| <span data-ttu-id="3d653-168">SourceCollection, из него добавляются элементы.</span><span class="sxs-lookup"><span data-stu-id="3d653-168">The sourceCollection that items are being added from.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3d653-169">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3d653-169">JSON representation</span></span>

<span data-ttu-id="3d653-170">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3d653-170">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.addToReviewSetOperation",
  "baseType": "microsoft.graph.ediscovery.caseOperation",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.addToReviewSetOperation",
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

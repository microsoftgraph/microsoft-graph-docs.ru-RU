---
title: тип ресурса estimateStatisticsOperation
description: Представляет операцию, которая обрабатывает оценку подсчета и размера коллекции исходных данных.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: e816ba01d4bb648a8e78b5b96369236f63fb163e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447487"
---
# <a name="estimatestatisticsoperation-resource-type"></a><span data-ttu-id="9d308-103">тип ресурса estimateStatisticsOperation</span><span class="sxs-lookup"><span data-stu-id="9d308-103">estimateStatisticsOperation resource type</span></span>

<span data-ttu-id="9d308-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="9d308-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d308-105">Представляет операцию, которая обрабатывает оценку подсчета и размера [sourceCollection.](../resources/ediscovery-sourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="9d308-105">Represents the operation that handles estimating the count and size of a [sourceCollection](../resources/ediscovery-sourcecollection.md).</span></span> <span data-ttu-id="9d308-106">Дополнительные сведения [см. в материале Сбор данных по делу в advanced eDiscovery.](/microsoft-365/compliance/collecting-data-for-ediscovery)</span><span class="sxs-lookup"><span data-stu-id="9d308-106">For details, see [Collect data for a case in Advanced eDiscovery](/microsoft-365/compliance/collecting-data-for-ediscovery).</span></span>

<span data-ttu-id="9d308-107">Наследует [от caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="9d308-107">Inherits from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>

## <a name="methods"></a><span data-ttu-id="9d308-108">Methods</span><span class="sxs-lookup"><span data-stu-id="9d308-108">Methods</span></span>

<span data-ttu-id="9d308-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="9d308-109">None.</span></span>

## <a name="properties"></a><span data-ttu-id="9d308-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="9d308-110">Properties</span></span>

|<span data-ttu-id="9d308-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d308-111">Property</span></span>|<span data-ttu-id="9d308-112">Тип</span><span class="sxs-lookup"><span data-stu-id="9d308-112">Type</span></span>|<span data-ttu-id="9d308-113">Описание</span><span class="sxs-lookup"><span data-stu-id="9d308-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d308-114">action</span><span class="sxs-lookup"><span data-stu-id="9d308-114">action</span></span>|<span data-ttu-id="9d308-115">microsoft.graph.ediscovery.caseAction</span><span class="sxs-lookup"><span data-stu-id="9d308-115">microsoft.graph.ediscovery.caseAction</span></span>| <span data-ttu-id="9d308-116">Тип операции.</span><span class="sxs-lookup"><span data-stu-id="9d308-116">The type of operation.</span></span> <span data-ttu-id="9d308-117">Действие случая для этой сущности всегда будет `estimateStatistics` .</span><span class="sxs-lookup"><span data-stu-id="9d308-117">The case action for this entity will always be `estimateStatistics`.</span></span> <span data-ttu-id="9d308-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9d308-118">Read-only.</span></span> <span data-ttu-id="9d308-119">Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="9d308-119">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="9d308-120">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="9d308-120">completedDateTime</span></span>|<span data-ttu-id="9d308-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d308-121">DateTimeOffset</span></span>|<span data-ttu-id="9d308-122">Дата и время завершения операции.</span><span class="sxs-lookup"><span data-stu-id="9d308-122">The date and time the operation was completed.</span></span> <span data-ttu-id="9d308-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9d308-123">Read-only.</span></span> <span data-ttu-id="9d308-124">Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="9d308-124">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="9d308-125">createdBy</span><span class="sxs-lookup"><span data-stu-id="9d308-125">createdBy</span></span>|[<span data-ttu-id="9d308-126">identitySet</span><span class="sxs-lookup"><span data-stu-id="9d308-126">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="9d308-127">Пользователь, создавший операцию.</span><span class="sxs-lookup"><span data-stu-id="9d308-127">The user who created the operation.</span></span> <span data-ttu-id="9d308-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9d308-128">Read-only.</span></span> <span data-ttu-id="9d308-129">Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="9d308-129">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="9d308-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9d308-130">createdDateTime</span></span>|<span data-ttu-id="9d308-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d308-131">DateTimeOffset</span></span>|<span data-ttu-id="9d308-132">Дата и время начала операции.</span><span class="sxs-lookup"><span data-stu-id="9d308-132">The date and time the operation was started.</span></span> <span data-ttu-id="9d308-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9d308-133">Read-only.</span></span> <span data-ttu-id="9d308-134">Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="9d308-134">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="9d308-135">id</span><span class="sxs-lookup"><span data-stu-id="9d308-135">id</span></span>|<span data-ttu-id="9d308-136">String</span><span class="sxs-lookup"><span data-stu-id="9d308-136">String</span></span>| <span data-ttu-id="9d308-137">ID для операции.</span><span class="sxs-lookup"><span data-stu-id="9d308-137">The ID for the operation.</span></span> <span data-ttu-id="9d308-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9d308-138">Read-only.</span></span> <span data-ttu-id="9d308-139">Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="9d308-139">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="9d308-140">indexedItemCount</span><span class="sxs-lookup"><span data-stu-id="9d308-140">indexedItemCount</span></span>|<span data-ttu-id="9d308-141">Int64</span><span class="sxs-lookup"><span data-stu-id="9d308-141">Int64</span></span>|<span data-ttu-id="9d308-142">Предполагаемое количество элементов **для sourceCollection,** которые соответствуют запросу контента.</span><span class="sxs-lookup"><span data-stu-id="9d308-142">The estimated count of items for the **sourceCollection** that matched the content query.</span></span>|
|<span data-ttu-id="9d308-143">indexedItemsSize</span><span class="sxs-lookup"><span data-stu-id="9d308-143">indexedItemsSize</span></span>|<span data-ttu-id="9d308-144">Int64</span><span class="sxs-lookup"><span data-stu-id="9d308-144">Int64</span></span>|<span data-ttu-id="9d308-145">Предполагаемый размер элементов **для sourceCollection,** совпадающий с запросом контента.</span><span class="sxs-lookup"><span data-stu-id="9d308-145">The estimated size of items for the **sourceCollection** that matched the content query.</span></span>|
|<span data-ttu-id="9d308-146">mailboxCount</span><span class="sxs-lookup"><span data-stu-id="9d308-146">mailboxCount</span></span>|<span data-ttu-id="9d308-147">Int32</span><span class="sxs-lookup"><span data-stu-id="9d308-147">Int32</span></span>|<span data-ttu-id="9d308-148">Количество почтовых ящиков с хитами поиска.</span><span class="sxs-lookup"><span data-stu-id="9d308-148">The number of mailboxes that had search hits.</span></span>|
|<span data-ttu-id="9d308-149">percentProgress</span><span class="sxs-lookup"><span data-stu-id="9d308-149">percentProgress</span></span>|<span data-ttu-id="9d308-150">Int32</span><span class="sxs-lookup"><span data-stu-id="9d308-150">Int32</span></span>|<span data-ttu-id="9d308-151">Ход операции.</span><span class="sxs-lookup"><span data-stu-id="9d308-151">The progress of the operation.</span></span> <span data-ttu-id="9d308-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9d308-152">Read-only.</span></span> <span data-ttu-id="9d308-153">Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="9d308-153">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="9d308-154">resultInfo</span><span class="sxs-lookup"><span data-stu-id="9d308-154">resultInfo</span></span>|[<span data-ttu-id="9d308-155">resultInfo</span><span class="sxs-lookup"><span data-stu-id="9d308-155">resultInfo</span></span>](../resources/resultinfo.md)|<span data-ttu-id="9d308-156">Содержит сведения о результатах, характерных для успешного и неудачного сбоя.</span><span class="sxs-lookup"><span data-stu-id="9d308-156">Contains success and failure-specific result information.</span></span> <span data-ttu-id="9d308-157">Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="9d308-157">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="9d308-158">siteCount</span><span class="sxs-lookup"><span data-stu-id="9d308-158">siteCount</span></span>|<span data-ttu-id="9d308-159">Int32</span><span class="sxs-lookup"><span data-stu-id="9d308-159">Int32</span></span>|<span data-ttu-id="9d308-160">Количество почтовых ящиков с хитами поиска.</span><span class="sxs-lookup"><span data-stu-id="9d308-160">The number of mailboxes that had search hits.</span></span>|
|<span data-ttu-id="9d308-161">status</span><span class="sxs-lookup"><span data-stu-id="9d308-161">status</span></span>|[<span data-ttu-id="9d308-162">microsoft.graph.ediscovery.caseOperationStatus</span><span class="sxs-lookup"><span data-stu-id="9d308-162">microsoft.graph.ediscovery.caseOperationStatus</span></span>](../resources/ediscovery-caseoperation.md#caseoperationstatus-values)|<span data-ttu-id="9d308-163">Состояние операции дела.</span><span class="sxs-lookup"><span data-stu-id="9d308-163">The status of the case operation.</span></span> <span data-ttu-id="9d308-164">Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="9d308-164">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span> <span data-ttu-id="9d308-165">Возможные значения: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="9d308-165">Possible values are: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.</span></span>|
|<span data-ttu-id="9d308-166">unindexedItemCount</span><span class="sxs-lookup"><span data-stu-id="9d308-166">unindexedItemCount</span></span>|<span data-ttu-id="9d308-167">Int64</span><span class="sxs-lookup"><span data-stu-id="9d308-167">Int64</span></span>|<span data-ttu-id="9d308-168">Предполагаемое количество неиндексуальных элементов для коллекции.</span><span class="sxs-lookup"><span data-stu-id="9d308-168">The estimated count of unindexed items for the collection.</span></span>|
|<span data-ttu-id="9d308-169">unindexedItemsSize</span><span class="sxs-lookup"><span data-stu-id="9d308-169">unindexedItemsSize</span></span>|<span data-ttu-id="9d308-170">Int64</span><span class="sxs-lookup"><span data-stu-id="9d308-170">Int64</span></span>|<span data-ttu-id="9d308-171">Предполагаемый размер неиндексуальных элементов для коллекции.</span><span class="sxs-lookup"><span data-stu-id="9d308-171">The estimated size of unindexed items for the collection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d308-172">Связи</span><span class="sxs-lookup"><span data-stu-id="9d308-172">Relationships</span></span>

|<span data-ttu-id="9d308-173">Связь</span><span class="sxs-lookup"><span data-stu-id="9d308-173">Relationship</span></span>|<span data-ttu-id="9d308-174">Тип</span><span class="sxs-lookup"><span data-stu-id="9d308-174">Type</span></span>|<span data-ttu-id="9d308-175">Описание</span><span class="sxs-lookup"><span data-stu-id="9d308-175">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d308-176">sourceCollection</span><span class="sxs-lookup"><span data-stu-id="9d308-176">sourceCollection</span></span>|[<span data-ttu-id="9d308-177">microsoft.graph.ediscovery.sourceCollection</span><span class="sxs-lookup"><span data-stu-id="9d308-177">microsoft.graph.ediscovery.sourceCollection</span></span>](../resources/ediscovery-sourcecollection.md)|<span data-ttu-id="9d308-178">коллекция электронных данных, обычно известная как поиск.</span><span class="sxs-lookup"><span data-stu-id="9d308-178">eDiscovery collection, commonly known as a search.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9d308-179">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9d308-179">JSON representation</span></span>

<span data-ttu-id="9d308-180">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d308-180">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.estimateStatisticsOperation",
  "baseType": "microsoft.graph.ediscovery.caseOperation",
  "openType": false
}
-->

``` json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/operations/$entity",
    "@odata.type": "#microsoft.graph.ediscovery.estimateStatisticsOperation",
    "createdDateTime": "2021-01-12T18:47:23.3974907Z",
    "completedDateTime": "2021-01-12T18:47:51.1461805Z",
    "percentProgress": 100,
    "status": "succeeded",
    "action": "estimateStatistics",
    "id": "82edd40e182a464fa02c24a36fa94873",
    "indexedItemCount": 2,
    "indexedItemsSize": 39276,
    "unindexedItemCount": 0,
    "unindexedItemsSize": 0,
    "mailboxCount": 1,
    "siteCount": 0,
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": null,
            "userPrincipalName": "admin@contoso.com"
        }
    }
}
```

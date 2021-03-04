---
title: тип ресурса caseOperation
description: Абстрактная сущность, которая представляет собой длительный процесс электронных разыскных открытий.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: b94aeba03a49f2c49cbf991f0046422a18b20b50
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447559"
---
# <a name="caseoperation-resource-type"></a><span data-ttu-id="ad60d-103">тип ресурса caseOperation</span><span class="sxs-lookup"><span data-stu-id="ad60d-103">caseOperation resource type</span></span>

<span data-ttu-id="ad60d-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="ad60d-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad60d-105">Абстрактная сущность, которая представляет собой длительный процесс электронных разыскных открытий.</span><span class="sxs-lookup"><span data-stu-id="ad60d-105">An abstract entity that represents a long-running eDiscovery process.</span></span> <span data-ttu-id="ad60d-106">Он содержит общий набор свойств, которые разделяются между наследующих сущностями.</span><span class="sxs-lookup"><span data-stu-id="ad60d-106">It contains a common set of properties that are shared among inheriting entities.</span></span>  <span data-ttu-id="ad60d-107">Сущности, которые вытекают из **caseOperation,** включают:</span><span class="sxs-lookup"><span data-stu-id="ad60d-107">Entities that derive from **caseOperation** include:</span></span>

- [<span data-ttu-id="ad60d-108">caseExportOperation</span><span class="sxs-lookup"><span data-stu-id="ad60d-108">caseExportOperation</span></span>](../resources/ediscovery-caseexportoperation.md)
- [<span data-ttu-id="ad60d-109">tagOperation</span><span class="sxs-lookup"><span data-stu-id="ad60d-109">tagOperation</span></span>](../resources/ediscovery-tagoperation.md)
- [<span data-ttu-id="ad60d-110">estimateStatisticsOperation</span><span class="sxs-lookup"><span data-stu-id="ad60d-110">estimateStatisticsOperation</span></span>](../resources/ediscovery-estimatestatisticsoperation.md)

<span data-ttu-id="ad60d-111">Наследует от [объекта](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="ad60d-111">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ad60d-112">Methods</span><span class="sxs-lookup"><span data-stu-id="ad60d-112">Methods</span></span>

<span data-ttu-id="ad60d-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="ad60d-113">None.</span></span>

## <a name="properties"></a><span data-ttu-id="ad60d-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="ad60d-114">Properties</span></span>

|<span data-ttu-id="ad60d-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad60d-115">Property</span></span>|<span data-ttu-id="ad60d-116">Тип</span><span class="sxs-lookup"><span data-stu-id="ad60d-116">Type</span></span>|<span data-ttu-id="ad60d-117">Описание</span><span class="sxs-lookup"><span data-stu-id="ad60d-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad60d-118">action</span><span class="sxs-lookup"><span data-stu-id="ad60d-118">action</span></span>|[<span data-ttu-id="ad60d-119">microsoft.graph.ediscovery.caseAction</span><span class="sxs-lookup"><span data-stu-id="ad60d-119">microsoft.graph.ediscovery.caseAction</span></span>](../resources/ediscovery-caseoperation.md#caseaction-values)| <span data-ttu-id="ad60d-120">Тип действия, который представляет операция.</span><span class="sxs-lookup"><span data-stu-id="ad60d-120">The type of action the operation represents.</span></span> <span data-ttu-id="ad60d-121">Возможные значения: `addToReviewSet` `applyTags` , , `contentExport` `convertToPdf` ,`estimateStatistics`</span><span class="sxs-lookup"><span data-stu-id="ad60d-121">Possible values are: `addToReviewSet`,`applyTags`,`contentExport`,`convertToPdf`,`estimateStatistics`</span></span>|
|<span data-ttu-id="ad60d-122">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="ad60d-122">completedDateTime</span></span>|<span data-ttu-id="ad60d-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad60d-123">DateTimeOffset</span></span>| <span data-ttu-id="ad60d-124">Дата и время завершения операции.</span><span class="sxs-lookup"><span data-stu-id="ad60d-124">The date and time the operation was completed.</span></span> |
|<span data-ttu-id="ad60d-125">createdBy</span><span class="sxs-lookup"><span data-stu-id="ad60d-125">createdBy</span></span>|[<span data-ttu-id="ad60d-126">identitySet</span><span class="sxs-lookup"><span data-stu-id="ad60d-126">identitySet</span></span>](../resources/identityset.md)| <span data-ttu-id="ad60d-127">Пользователь, создав операцию.</span><span class="sxs-lookup"><span data-stu-id="ad60d-127">The user that created the operation.</span></span> |
|<span data-ttu-id="ad60d-128">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ad60d-128">createdDateTime</span></span>|<span data-ttu-id="ad60d-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad60d-129">DateTimeOffset</span></span>| <span data-ttu-id="ad60d-130">Дата и время создания операции.</span><span class="sxs-lookup"><span data-stu-id="ad60d-130">The date and time the operation was created.</span></span> |
|<span data-ttu-id="ad60d-131">id</span><span class="sxs-lookup"><span data-stu-id="ad60d-131">id</span></span>|<span data-ttu-id="ad60d-132">String</span><span class="sxs-lookup"><span data-stu-id="ad60d-132">String</span></span>| <span data-ttu-id="ad60d-133">ID для операции.</span><span class="sxs-lookup"><span data-stu-id="ad60d-133">The ID for the operation.</span></span> <span data-ttu-id="ad60d-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ad60d-134">Read-only.</span></span> |
|<span data-ttu-id="ad60d-135">percentProgress</span><span class="sxs-lookup"><span data-stu-id="ad60d-135">percentProgress</span></span>|<span data-ttu-id="ad60d-136">Int32</span><span class="sxs-lookup"><span data-stu-id="ad60d-136">Int32</span></span>| <span data-ttu-id="ad60d-137">Ход операции.</span><span class="sxs-lookup"><span data-stu-id="ad60d-137">The progress of the operation.</span></span> |
|<span data-ttu-id="ad60d-138">resultInfo</span><span class="sxs-lookup"><span data-stu-id="ad60d-138">resultInfo</span></span>|[<span data-ttu-id="ad60d-139">resultInfo</span><span class="sxs-lookup"><span data-stu-id="ad60d-139">resultInfo</span></span>](../resources/resultinfo.md)| <span data-ttu-id="ad60d-140">Содержит сведения о результатах, характерных для успешного и неудачного сбоя.</span><span class="sxs-lookup"><span data-stu-id="ad60d-140">Contains success and failure-specific result information.</span></span> |
|<span data-ttu-id="ad60d-141">status</span><span class="sxs-lookup"><span data-stu-id="ad60d-141">status</span></span>|[<span data-ttu-id="ad60d-142">microsoft.graph.ediscovery.caseOperationStatus</span><span class="sxs-lookup"><span data-stu-id="ad60d-142">microsoft.graph.ediscovery.caseOperationStatus</span></span>](../resources/ediscovery-caseoperation.md#caseoperationstatus-values)| <span data-ttu-id="ad60d-143">Состояние операции дела.</span><span class="sxs-lookup"><span data-stu-id="ad60d-143">The status of the case operation.</span></span> <span data-ttu-id="ad60d-144">Возможные значения: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="ad60d-144">Possible values are: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.</span></span>|

### <a name="caseaction-values"></a><span data-ttu-id="ad60d-145">значения caseAction</span><span class="sxs-lookup"><span data-stu-id="ad60d-145">caseAction values</span></span>

|<span data-ttu-id="ad60d-146">Member</span><span class="sxs-lookup"><span data-stu-id="ad60d-146">Member</span></span>|<span data-ttu-id="ad60d-147">Описание</span><span class="sxs-lookup"><span data-stu-id="ad60d-147">Description</span></span>|
|:----|-----------|
| <span data-ttu-id="ad60d-148">addToReviewSet</span><span class="sxs-lookup"><span data-stu-id="ad60d-148">addToReviewSet</span></span> | <span data-ttu-id="ad60d-149">Операция представляет добавление данных в набор отзывов из коллекции eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="ad60d-149">The operation represents adding data to a review set from an eDiscovery collection.</span></span> |
| <span data-ttu-id="ad60d-150">applyTags</span><span class="sxs-lookup"><span data-stu-id="ad60d-150">applyTags</span></span> | <span data-ttu-id="ad60d-151">Операция представляет документы с массовыми тегами в наборе отзывов для указанного запроса набора обзоров.</span><span class="sxs-lookup"><span data-stu-id="ad60d-151">The operation represents bulk tagging documents in a review set for the specified review set query.</span></span> |
| <span data-ttu-id="ad60d-152">contentExport</span><span class="sxs-lookup"><span data-stu-id="ad60d-152">contentExport</span></span> | <span data-ttu-id="ad60d-153">Операция представляет экспорт контента из набора отзывов.</span><span class="sxs-lookup"><span data-stu-id="ad60d-153">The operation represents a content export from a review set.</span></span> |
| <span data-ttu-id="ad60d-154">convertToPdf</span><span class="sxs-lookup"><span data-stu-id="ad60d-154">convertToPdf</span></span> | <span data-ttu-id="ad60d-155">Операция представляет преобразование документов в PDF с помощью отредакций.</span><span class="sxs-lookup"><span data-stu-id="ad60d-155">The operation represents converting documents to PDFs with redactions.</span></span> |
| <span data-ttu-id="ad60d-156">estimateStatistics</span><span class="sxs-lookup"><span data-stu-id="ad60d-156">estimateStatistics</span></span>  | <span data-ttu-id="ad60d-157">Операция представляет поиск по таким службам Microsoft 365, как Exchange, SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="ad60d-157">The operation represents searching against Microsoft 365 services such as Exchange, SharePoint, and OneDrive for business.</span></span> |

### <a name="caseoperationstatus-values"></a><span data-ttu-id="ad60d-158">значения caseOperationStatus</span><span class="sxs-lookup"><span data-stu-id="ad60d-158">caseOperationStatus values</span></span>

|<span data-ttu-id="ad60d-159">Member</span><span class="sxs-lookup"><span data-stu-id="ad60d-159">Member</span></span>|<span data-ttu-id="ad60d-160">Описание</span><span class="sxs-lookup"><span data-stu-id="ad60d-160">Description</span></span>|
|:----|-----------|
| <span data-ttu-id="ad60d-161">notStarted</span><span class="sxs-lookup"><span data-stu-id="ad60d-161">notStarted</span></span> | <span data-ttu-id="ad60d-162">Операция еще не началась.</span><span class="sxs-lookup"><span data-stu-id="ad60d-162">The operation has not yet started.</span></span> |
| <span data-ttu-id="ad60d-163">submissionFailed</span><span class="sxs-lookup"><span data-stu-id="ad60d-163">submissionFailed</span></span> | <span data-ttu-id="ad60d-164">Отправка операции не удалась.</span><span class="sxs-lookup"><span data-stu-id="ad60d-164">Submission of the operation failed.</span></span> |
| <span data-ttu-id="ad60d-165">запуск</span><span class="sxs-lookup"><span data-stu-id="ad60d-165">running</span></span> | <span data-ttu-id="ad60d-166">Операция в настоящее время запущена.</span><span class="sxs-lookup"><span data-stu-id="ad60d-166">The operation is currently running.</span></span> |
| <span data-ttu-id="ad60d-167">успешно</span><span class="sxs-lookup"><span data-stu-id="ad60d-167">succeeded</span></span> | <span data-ttu-id="ad60d-168">Операция была успешно выполнена без ошибок.</span><span class="sxs-lookup"><span data-stu-id="ad60d-168">The operation was successfully completed without any errors.</span></span> |
| <span data-ttu-id="ad60d-169">partiallySucceeded</span><span class="sxs-lookup"><span data-stu-id="ad60d-169">partiallySucceeded</span></span> | <span data-ttu-id="ad60d-170">Операция завершена, но произошли ошибки . Сведения об ошибках см. [в материале resultInfo.](../resources/resultinfo.md)</span><span class="sxs-lookup"><span data-stu-id="ad60d-170">The operation completed, but there were errors - See [resultInfo](../resources/resultinfo.md) for error details.</span></span> |
| <span data-ttu-id="ad60d-171">не удалось</span><span class="sxs-lookup"><span data-stu-id="ad60d-171">failed</span></span> | <span data-ttu-id="ad60d-172">Операция не удалась . Сведения об ошибках см. в результатах.</span><span class="sxs-lookup"><span data-stu-id="ad60d-172">The operation failed - See result info for error details.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ad60d-173">Связи</span><span class="sxs-lookup"><span data-stu-id="ad60d-173">Relationships</span></span>

<span data-ttu-id="ad60d-174">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ad60d-174">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ad60d-175">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ad60d-175">JSON representation</span></span>

<span data-ttu-id="ad60d-176">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad60d-176">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.caseOperation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.caseOperation",
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

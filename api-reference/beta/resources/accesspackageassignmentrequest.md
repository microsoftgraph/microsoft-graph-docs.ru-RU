---
title: Тип ресурса Акцесспаккажеассигнментрекуест
description: Запрос на назначение пакета Access создается пользователем, желающим получить назначение пакета Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b546071984f938f7e07c927681aa1b9e50d4cfd0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064404"
---
# <a name="accesspackageassignmentrequest-resource-type"></a><span data-ttu-id="d8510-103">Тип ресурса Акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="d8510-103">accessPackageAssignmentRequest resource type</span></span>

<span data-ttu-id="d8510-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8510-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8510-105">В [управлении обслуживанием в Azure AD](entitlementmanagement-root.md)запрос на назначение пакета Access создается или от имени пользователя, которому требуется получить назначение пакета Access.</span><span class="sxs-lookup"><span data-stu-id="d8510-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by or on behalf of a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="d8510-106">Если запрос выполнен успешно, при наличии необходимых утверждений пользователь получает назначение пакета Access и является темой этого назначенного пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="d8510-106">If the request is successful, with any necessary approvals, the user receives an access package assignment, and is the subject of that resulting access package assignment.</span></span>  <span data-ttu-id="d8510-107">Кроме того, Azure AD автоматически создает запросы на отправку для отслеживания удаления.</span><span class="sxs-lookup"><span data-stu-id="d8510-107">Azure AD also creates access package assignment requests automatically for tracking access removal.</span></span>

## <a name="methods"></a><span data-ttu-id="d8510-108">Методы</span><span class="sxs-lookup"><span data-stu-id="d8510-108">Methods</span></span>

| <span data-ttu-id="d8510-109">Метод</span><span class="sxs-lookup"><span data-stu-id="d8510-109">Method</span></span>       | <span data-ttu-id="d8510-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d8510-110">Return Type</span></span> | <span data-ttu-id="d8510-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d8510-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d8510-112">Список Акцесспаккажеассигнментрекуестс</span><span class="sxs-lookup"><span data-stu-id="d8510-112">List accessPackageAssignmentRequests</span></span>](../api/accesspackageassignmentrequest-list.md) | <span data-ttu-id="d8510-113">Коллекция [акцесспаккажеассигнментрекуест](accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="d8510-113">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md) collection</span></span> | <span data-ttu-id="d8510-114">Получение списка объектов акцесспаккажеассигнментрекуест.</span><span class="sxs-lookup"><span data-stu-id="d8510-114">Retrieve a list of accesspackageassignmentrequest objects.</span></span> |
| [<span data-ttu-id="d8510-115">Создание Акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="d8510-115">Create accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-post.md) | [<span data-ttu-id="d8510-116">акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="d8510-116">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="d8510-117">Создание нового Акцесспаккажеассигнментрекуест.</span><span class="sxs-lookup"><span data-stu-id="d8510-117">Create a new accessPackageAssignmentRequest.</span></span> |
| [<span data-ttu-id="d8510-118">Получение Акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="d8510-118">Get accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-get.md) | [<span data-ttu-id="d8510-119">акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="d8510-119">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="d8510-120">Чтение свойств и связей объекта Акцесспаккажеассигнментрекуест.</span><span class="sxs-lookup"><span data-stu-id="d8510-120">Read properties and relationships of an accessPackageAssignmentRequest object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d8510-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="d8510-121">Properties</span></span>

| <span data-ttu-id="d8510-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8510-122">Property</span></span>     | <span data-ttu-id="d8510-123">Тип</span><span class="sxs-lookup"><span data-stu-id="d8510-123">Type</span></span>        | <span data-ttu-id="d8510-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d8510-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d8510-125">комплетеддате</span><span class="sxs-lookup"><span data-stu-id="d8510-125">completedDate</span></span>|<span data-ttu-id="d8510-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8510-126">DateTimeOffset</span></span>|<span data-ttu-id="d8510-127">Дата завершения обработки (успешное или неудачное) запроса.</span><span class="sxs-lookup"><span data-stu-id="d8510-127">The date of the end of processing, either successful or failure, of a request.</span></span> <span data-ttu-id="d8510-128">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="d8510-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d8510-129">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d8510-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="d8510-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d8510-130">Read-only.</span></span>|
|<span data-ttu-id="d8510-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d8510-131">createdDateTime</span></span>|<span data-ttu-id="d8510-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8510-132">DateTimeOffset</span></span>|<span data-ttu-id="d8510-133">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="d8510-133">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d8510-134">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d8510-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="d8510-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d8510-135">Read-only.</span></span>|
|<span data-ttu-id="d8510-136">id</span><span class="sxs-lookup"><span data-stu-id="d8510-136">id</span></span>|<span data-ttu-id="d8510-137">String</span><span class="sxs-lookup"><span data-stu-id="d8510-137">String</span></span>| <span data-ttu-id="d8510-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d8510-138">Read-only.</span></span>|
|<span data-ttu-id="d8510-139">исвалидатиононли</span><span class="sxs-lookup"><span data-stu-id="d8510-139">isValidationOnly</span></span>|<span data-ttu-id="d8510-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8510-140">Boolean</span></span>|<span data-ttu-id="d8510-141">Имеет значение true, если запрос не обрабатывается для назначения.</span><span class="sxs-lookup"><span data-stu-id="d8510-141">True if the request is not to be processed for assignment.</span></span>|
|<span data-ttu-id="d8510-142">текста</span><span class="sxs-lookup"><span data-stu-id="d8510-142">justification</span></span>|<span data-ttu-id="d8510-143">String</span><span class="sxs-lookup"><span data-stu-id="d8510-143">String</span></span>|<span data-ttu-id="d8510-144">Выставляемое по запросу обоснование.</span><span class="sxs-lookup"><span data-stu-id="d8510-144">The requestor's supplied justification.</span></span>|
|<span data-ttu-id="d8510-145">рекуестстате</span><span class="sxs-lookup"><span data-stu-id="d8510-145">requestState</span></span>|<span data-ttu-id="d8510-146">String</span><span class="sxs-lookup"><span data-stu-id="d8510-146">String</span></span>|<span data-ttu-id="d8510-147">Один из `PendingApproval` ,,,,, `Canceled`  `Denied` `Delivering` `Delivered` `PartiallyDelivered` , `Submitted` или `Scheduled` .</span><span class="sxs-lookup"><span data-stu-id="d8510-147">One of `PendingApproval`, `Canceled`,  `Denied`, `Delivering`, `Delivered`, `PartiallyDelivered`, `Submitted` or `Scheduled`.</span></span> <span data-ttu-id="d8510-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d8510-148">Read-only.</span></span>|
|<span data-ttu-id="d8510-149">рекуестстатус</span><span class="sxs-lookup"><span data-stu-id="d8510-149">requestStatus</span></span>|<span data-ttu-id="d8510-150">String</span><span class="sxs-lookup"><span data-stu-id="d8510-150">String</span></span>|<span data-ttu-id="d8510-151">Дополнительные сведения о состоянии обработки запроса.</span><span class="sxs-lookup"><span data-stu-id="d8510-151">More information on the request processing status.</span></span> <span data-ttu-id="d8510-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d8510-152">Read-only.</span></span>|
|<span data-ttu-id="d8510-153">requestType</span><span class="sxs-lookup"><span data-stu-id="d8510-153">requestType</span></span>|<span data-ttu-id="d8510-154">String</span><span class="sxs-lookup"><span data-stu-id="d8510-154">String</span></span>|<span data-ttu-id="d8510-155">Один из `UserAdd` , `UserRemove` , `AdminAdd` `AdminRemove` или `SystemRemove` .</span><span class="sxs-lookup"><span data-stu-id="d8510-155">One of `UserAdd`, `UserRemove`, `AdminAdd`, `AdminRemove` or `SystemRemove`.</span></span> <span data-ttu-id="d8510-156">У самого пользователя запрос будет иметь значение requestType `UserAdd` или `UserRemove` .</span><span class="sxs-lookup"><span data-stu-id="d8510-156">A request from the user themselves would have requestType of `UserAdd` or `UserRemove`.</span></span> <span data-ttu-id="d8510-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d8510-157">Read-only.</span></span>|
|<span data-ttu-id="d8510-158">schedule</span><span class="sxs-lookup"><span data-stu-id="d8510-158">schedule</span></span>|[<span data-ttu-id="d8510-159">рекуестсчедуле</span><span class="sxs-lookup"><span data-stu-id="d8510-159">requestSchedule</span></span>](requestschedule.md)| <span data-ttu-id="d8510-160">Диапазон дат, к которым требуется назначить доступ для запрашивающего.</span><span class="sxs-lookup"><span data-stu-id="d8510-160">The range of dates that access is to be assigned to the requestor.</span></span> <span data-ttu-id="d8510-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d8510-161">Read-only.</span></span>|
|<span data-ttu-id="d8510-162">акцесспаккажеассигнмент</span><span class="sxs-lookup"><span data-stu-id="d8510-162">accessPackageAssignment</span></span>|[<span data-ttu-id="d8510-163">акцесспаккажеассигнмент</span><span class="sxs-lookup"><span data-stu-id="d8510-163">accessPackageAssignment</span></span>](accesspackageassignment.md)| <span data-ttu-id="d8510-164">Для параметра requestType `UserAdd` или необходимо `AdminAdd` создать назначение пакета Access.</span><span class="sxs-lookup"><span data-stu-id="d8510-164">For a requestType of `UserAdd` or `AdminAdd`, this is an access package assignment requested to be created.</span></span>  <span data-ttu-id="d8510-165">Для объекта requestType `UserRemove` , `AdminRemove` или `SystemRemove` , это свойство содержит `id` свойство существующего назначения, которое необходимо удалить.</span><span class="sxs-lookup"><span data-stu-id="d8510-165">For a requestType of `UserRemove`, `AdminRemove` or `SystemRemove`, this has the `id` property of an existing assignment to be removed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8510-166">Связи</span><span class="sxs-lookup"><span data-stu-id="d8510-166">Relationships</span></span>

| <span data-ttu-id="d8510-167">Связь</span><span class="sxs-lookup"><span data-stu-id="d8510-167">Relationship</span></span> | <span data-ttu-id="d8510-168">Тип</span><span class="sxs-lookup"><span data-stu-id="d8510-168">Type</span></span>        | <span data-ttu-id="d8510-169">Описание</span><span class="sxs-lookup"><span data-stu-id="d8510-169">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d8510-170">опросчика</span><span class="sxs-lookup"><span data-stu-id="d8510-170">requestor</span></span>|[<span data-ttu-id="d8510-171">акцесспаккажесубжект</span><span class="sxs-lookup"><span data-stu-id="d8510-171">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="d8510-172">Тема, которая запросила или, если назначено прямое назначение, было назначено.</span><span class="sxs-lookup"><span data-stu-id="d8510-172">The subject who requested or, if a direct assignment, was assigned.</span></span> <span data-ttu-id="d8510-173">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d8510-173">Read-only.</span></span> <span data-ttu-id="d8510-174">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="d8510-174">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d8510-175">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d8510-175">JSON representation</span></span>

<span data-ttu-id="d8510-176">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8510-176">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "createdDateTime": "2020-02-12T22:06:58.303Z",
  "completedDate": "2020-02-12T22:14:28.19Z",
  "id": "1244d439-5baa-4b9a-be5f-e8fdef5a998b",
  "requestType": "UserAdd",
  "requestState": "Delivered",
  "requestStatus": "FulfilledNotificationTriggered",
  "isValidationOnly": false,
  "justification": ""
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageAssignmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



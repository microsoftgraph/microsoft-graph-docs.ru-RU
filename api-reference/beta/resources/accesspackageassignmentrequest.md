---
title: Тип ресурса Акцесспаккажеассигнментрекуест
description: Запрос на назначение пакета Access создается пользователем, желающим получить назначение пакета Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 11b3095bf54f6d5ffe1af4ca4926fe4409429b48
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319535"
---
# <a name="accesspackageassignmentrequest-resource-type"></a><span data-ttu-id="0511c-103">Тип ресурса Акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="0511c-103">accessPackageAssignmentRequest resource type</span></span>

<span data-ttu-id="0511c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0511c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0511c-105">В [управлении обслуживанием в Azure AD](entitlementmanagement-root.md)запрос на назначение пакета Access создается или от имени пользователя, которому требуется получить назначение пакета Access.</span><span class="sxs-lookup"><span data-stu-id="0511c-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by or on behalf of a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="0511c-106">Если запрос выполнен успешно, при наличии необходимых утверждений пользователь получает назначение пакета Access и является темой этого назначенного пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="0511c-106">If the request is successful, with any necessary approvals, the user receives an access package assignment, and is the subject of that resulting access package assignment.</span></span>  <span data-ttu-id="0511c-107">Кроме того, Azure AD автоматически создает запросы на отправку для отслеживания удаления.</span><span class="sxs-lookup"><span data-stu-id="0511c-107">Azure AD also creates access package assignment requests automatically for tracking access removal.</span></span>

## <a name="methods"></a><span data-ttu-id="0511c-108">Методы</span><span class="sxs-lookup"><span data-stu-id="0511c-108">Methods</span></span>

| <span data-ttu-id="0511c-109">Метод</span><span class="sxs-lookup"><span data-stu-id="0511c-109">Method</span></span>       | <span data-ttu-id="0511c-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0511c-110">Return Type</span></span> | <span data-ttu-id="0511c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0511c-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="0511c-112">Список Акцесспаккажеассигнментрекуестс</span><span class="sxs-lookup"><span data-stu-id="0511c-112">List accessPackageAssignmentRequests</span></span>](../api/accesspackageassignmentrequest-list.md) | <span data-ttu-id="0511c-113">Коллекция [акцесспаккажеассигнментрекуест](accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="0511c-113">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md) collection</span></span> | <span data-ttu-id="0511c-114">Получение списка объектов акцесспаккажеассигнментрекуест.</span><span class="sxs-lookup"><span data-stu-id="0511c-114">Retrieve a list of accesspackageassignmentrequest objects.</span></span> |
| [<span data-ttu-id="0511c-115">Создание Акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="0511c-115">Create accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-post.md) | [<span data-ttu-id="0511c-116">акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="0511c-116">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="0511c-117">Создание нового Акцесспаккажеассигнментрекуест.</span><span class="sxs-lookup"><span data-stu-id="0511c-117">Create a new accessPackageAssignmentRequest.</span></span> |
| [<span data-ttu-id="0511c-118">Получение Акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="0511c-118">Get accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-get.md) | [<span data-ttu-id="0511c-119">акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="0511c-119">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="0511c-120">Чтение свойств и связей объекта Акцесспаккажеассигнментрекуест.</span><span class="sxs-lookup"><span data-stu-id="0511c-120">Read properties and relationships of an accessPackageAssignmentRequest object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0511c-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="0511c-121">Properties</span></span>

| <span data-ttu-id="0511c-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="0511c-122">Property</span></span>     | <span data-ttu-id="0511c-123">Тип</span><span class="sxs-lookup"><span data-stu-id="0511c-123">Type</span></span>        | <span data-ttu-id="0511c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="0511c-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0511c-125">комплетеддате</span><span class="sxs-lookup"><span data-stu-id="0511c-125">completedDate</span></span>|<span data-ttu-id="0511c-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0511c-126">DateTimeOffset</span></span>|<span data-ttu-id="0511c-127">Дата завершения обработки (успешное или неудачное) запроса.</span><span class="sxs-lookup"><span data-stu-id="0511c-127">The date of the end of processing, either successful or failure, of a request.</span></span> <span data-ttu-id="0511c-128">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="0511c-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0511c-129">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="0511c-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="0511c-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0511c-130">Read-only.</span></span>|
|<span data-ttu-id="0511c-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0511c-131">createdDateTime</span></span>|<span data-ttu-id="0511c-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0511c-132">DateTimeOffset</span></span>|<span data-ttu-id="0511c-133">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="0511c-133">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0511c-134">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="0511c-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="0511c-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0511c-135">Read-only.</span></span>|
|<span data-ttu-id="0511c-136">id</span><span class="sxs-lookup"><span data-stu-id="0511c-136">id</span></span>|<span data-ttu-id="0511c-137">String</span><span class="sxs-lookup"><span data-stu-id="0511c-137">String</span></span>| <span data-ttu-id="0511c-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0511c-138">Read-only.</span></span>|
|<span data-ttu-id="0511c-139">исвалидатиононли</span><span class="sxs-lookup"><span data-stu-id="0511c-139">isValidationOnly</span></span>|<span data-ttu-id="0511c-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="0511c-140">Boolean</span></span>|<span data-ttu-id="0511c-141">Имеет значение true, если запрос не обрабатывается для назначения.</span><span class="sxs-lookup"><span data-stu-id="0511c-141">True if the request is not to be processed for assignment.</span></span>|
|<span data-ttu-id="0511c-142">текста</span><span class="sxs-lookup"><span data-stu-id="0511c-142">justification</span></span>|<span data-ttu-id="0511c-143">String</span><span class="sxs-lookup"><span data-stu-id="0511c-143">String</span></span>|<span data-ttu-id="0511c-144">Выставляемое по запросу обоснование.</span><span class="sxs-lookup"><span data-stu-id="0511c-144">The requestor's supplied justification.</span></span>|
|<span data-ttu-id="0511c-145">рекуестстате</span><span class="sxs-lookup"><span data-stu-id="0511c-145">requestState</span></span>|<span data-ttu-id="0511c-146">String</span><span class="sxs-lookup"><span data-stu-id="0511c-146">String</span></span>|<span data-ttu-id="0511c-147">Один из `PendingApproval` ,,,,, `Canceled`  `Denied` `Delivering` `Delivered` `PartiallyDelivered` , `Submitted` или `Scheduled` .</span><span class="sxs-lookup"><span data-stu-id="0511c-147">One of `PendingApproval`, `Canceled`,  `Denied`, `Delivering`, `Delivered`, `PartiallyDelivered`, `Submitted` or `Scheduled`.</span></span> <span data-ttu-id="0511c-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0511c-148">Read-only.</span></span>|
|<span data-ttu-id="0511c-149">рекуестстатус</span><span class="sxs-lookup"><span data-stu-id="0511c-149">requestStatus</span></span>|<span data-ttu-id="0511c-150">String</span><span class="sxs-lookup"><span data-stu-id="0511c-150">String</span></span>|<span data-ttu-id="0511c-151">Дополнительные сведения о состоянии обработки запроса.</span><span class="sxs-lookup"><span data-stu-id="0511c-151">More information on the request processing status.</span></span> <span data-ttu-id="0511c-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0511c-152">Read-only.</span></span>|
|<span data-ttu-id="0511c-153">requestType</span><span class="sxs-lookup"><span data-stu-id="0511c-153">requestType</span></span>|<span data-ttu-id="0511c-154">String</span><span class="sxs-lookup"><span data-stu-id="0511c-154">String</span></span>|<span data-ttu-id="0511c-155">Один из `UserAdd` , `UserRemove` , `AdminAdd` `AdminRemove` или `SystemRemove` .</span><span class="sxs-lookup"><span data-stu-id="0511c-155">One of `UserAdd`, `UserRemove`, `AdminAdd`, `AdminRemove` or `SystemRemove`.</span></span> <span data-ttu-id="0511c-156">У самого пользователя запрос будет иметь значение requestType `UserAdd` или `UserRemove` .</span><span class="sxs-lookup"><span data-stu-id="0511c-156">A request from the user themselves would have requestType of `UserAdd` or `UserRemove`.</span></span> <span data-ttu-id="0511c-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0511c-157">Read-only.</span></span>|
|<span data-ttu-id="0511c-158">акцесспаккажеассигнмент</span><span class="sxs-lookup"><span data-stu-id="0511c-158">accessPackageAssignment</span></span>|[<span data-ttu-id="0511c-159">акцесспаккажеассигнмент</span><span class="sxs-lookup"><span data-stu-id="0511c-159">accessPackageAssignment</span></span>](accesspackageassignment.md)| <span data-ttu-id="0511c-160">Для параметра requestType `UserAdd` или необходимо `AdminAdd` создать назначение пакета Access.</span><span class="sxs-lookup"><span data-stu-id="0511c-160">For a requestType of `UserAdd` or `AdminAdd`, this is an access package assignment requested to be created.</span></span>  <span data-ttu-id="0511c-161">Для объекта requestType `UserRemove` , `AdminRemove` или `SystemRemove` , это свойство содержит `id` свойство существующего назначения, которое необходимо удалить.</span><span class="sxs-lookup"><span data-stu-id="0511c-161">For a requestType of `UserRemove`, `AdminRemove` or `SystemRemove`, this has the `id` property of an existing assignment to be removed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0511c-162">Отношения</span><span class="sxs-lookup"><span data-stu-id="0511c-162">Relationships</span></span>

| <span data-ttu-id="0511c-163">Связь</span><span class="sxs-lookup"><span data-stu-id="0511c-163">Relationship</span></span> | <span data-ttu-id="0511c-164">Тип</span><span class="sxs-lookup"><span data-stu-id="0511c-164">Type</span></span>        | <span data-ttu-id="0511c-165">Описание</span><span class="sxs-lookup"><span data-stu-id="0511c-165">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0511c-166">опросчика</span><span class="sxs-lookup"><span data-stu-id="0511c-166">requestor</span></span>|[<span data-ttu-id="0511c-167">акцесспаккажесубжект</span><span class="sxs-lookup"><span data-stu-id="0511c-167">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="0511c-168">Тема, которая запросила или, если назначено прямое назначение, было назначено.</span><span class="sxs-lookup"><span data-stu-id="0511c-168">The subject who requested or, if a direct assignment, was assigned.</span></span> <span data-ttu-id="0511c-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0511c-169">Read-only.</span></span> <span data-ttu-id="0511c-170">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="0511c-170">Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="0511c-171">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0511c-171">JSON representation</span></span>

<span data-ttu-id="0511c-172">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0511c-172">The following is a JSON representation of the resource.</span></span>

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

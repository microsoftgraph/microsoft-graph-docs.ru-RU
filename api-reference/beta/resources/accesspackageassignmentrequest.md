---
title: Тип ресурса Акцесспаккажеассигнментрекуест
description: Запрос на назначение пакета Access создается пользователем, желающим получить назначение пакета Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0fd9f5ea9cd15abac7eea693b2af5c595b145ac7
ms.sourcegitcommit: f51ba08d604d93f5f6af9ee8979cbf76baa285ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/19/2020
ms.locfileid: "42108443"
---
# <a name="accesspackageassignmentrequest-resource-type"></a><span data-ttu-id="64fb1-103">Тип ресурса Акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="64fb1-103">accessPackageAssignmentRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64fb1-104">В [управлении обслуживанием в Azure AD](entitlementmanagement-root.md)запрос на назначение пакета Access создается пользователем, желающим получить назначение пакета Access.</span><span class="sxs-lookup"><span data-stu-id="64fb1-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="64fb1-105">Если запрос выполнен успешно, при наличии необходимых утверждений пользователь получает назначение пакета Access и является темой этого назначенного пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="64fb1-105">If the request is successful, with any necessary approvals, the user receives an access package assignment, and is the subject of that resulting access package assignment.</span></span>


## <a name="methods"></a><span data-ttu-id="64fb1-106">Методы</span><span class="sxs-lookup"><span data-stu-id="64fb1-106">Methods</span></span>

| <span data-ttu-id="64fb1-107">Метод</span><span class="sxs-lookup"><span data-stu-id="64fb1-107">Method</span></span>       | <span data-ttu-id="64fb1-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="64fb1-108">Return Type</span></span> | <span data-ttu-id="64fb1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="64fb1-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="64fb1-110">Список Акцесспаккажеассигнментрекуестс</span><span class="sxs-lookup"><span data-stu-id="64fb1-110">List accessPackageAssignmentRequests</span></span>](../api/accesspackageassignmentrequest-list.md) | <span data-ttu-id="64fb1-111">Коллекция [акцесспаккажеассигнментрекуест](accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="64fb1-111">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md) collection</span></span> | <span data-ttu-id="64fb1-112">Получение списка объектов акцесспаккажеассигнментрекуест.</span><span class="sxs-lookup"><span data-stu-id="64fb1-112">Retrieve a list of accesspackageassignmentrequest objects.</span></span> |
| [<span data-ttu-id="64fb1-113">Создание Акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="64fb1-113">Create accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-post.md) | [<span data-ttu-id="64fb1-114">акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="64fb1-114">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="64fb1-115">Создание нового Акцесспаккажеассигнментрекуест.</span><span class="sxs-lookup"><span data-stu-id="64fb1-115">Create a new accessPackageAssignmentRequest.</span></span> |
| [<span data-ttu-id="64fb1-116">Получение Акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="64fb1-116">Get accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-get.md) | [<span data-ttu-id="64fb1-117">акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="64fb1-117">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="64fb1-118">Чтение свойств и связей объекта Акцесспаккажеассигнментрекуест.</span><span class="sxs-lookup"><span data-stu-id="64fb1-118">Read properties and relationships of an accessPackageAssignmentRequest object.</span></span> |

## <a name="properties"></a><span data-ttu-id="64fb1-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="64fb1-119">Properties</span></span>

| <span data-ttu-id="64fb1-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="64fb1-120">Property</span></span>     | <span data-ttu-id="64fb1-121">Тип</span><span class="sxs-lookup"><span data-stu-id="64fb1-121">Type</span></span>        | <span data-ttu-id="64fb1-122">Описание</span><span class="sxs-lookup"><span data-stu-id="64fb1-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="64fb1-123">комплетеддате</span><span class="sxs-lookup"><span data-stu-id="64fb1-123">completedDate</span></span>|<span data-ttu-id="64fb1-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64fb1-124">DateTimeOffset</span></span>|<span data-ttu-id="64fb1-125">Дата завершения обработки (успешное или неудачное) запроса.</span><span class="sxs-lookup"><span data-stu-id="64fb1-125">The date of the end of processing, either successful or failure, of a request.</span></span> <span data-ttu-id="64fb1-126">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="64fb1-126">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="64fb1-127">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="64fb1-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="64fb1-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64fb1-128">Read-only.</span></span>|
|<span data-ttu-id="64fb1-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="64fb1-129">createdDateTime</span></span>|<span data-ttu-id="64fb1-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64fb1-130">DateTimeOffset</span></span>|<span data-ttu-id="64fb1-131">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="64fb1-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="64fb1-132">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="64fb1-132">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="64fb1-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64fb1-133">Read-only.</span></span>|
|<span data-ttu-id="64fb1-134">id</span><span class="sxs-lookup"><span data-stu-id="64fb1-134">id</span></span>|<span data-ttu-id="64fb1-135">String</span><span class="sxs-lookup"><span data-stu-id="64fb1-135">String</span></span>| <span data-ttu-id="64fb1-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64fb1-136">Read-only.</span></span>|
|<span data-ttu-id="64fb1-137">исвалидатиононли</span><span class="sxs-lookup"><span data-stu-id="64fb1-137">isValidationOnly</span></span>|<span data-ttu-id="64fb1-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="64fb1-138">Boolean</span></span>|<span data-ttu-id="64fb1-139">Имеет значение true, если запрос не обрабатывается для назначения.</span><span class="sxs-lookup"><span data-stu-id="64fb1-139">True if the request is not to be processed for assignment.</span></span>|
|<span data-ttu-id="64fb1-140">текста</span><span class="sxs-lookup"><span data-stu-id="64fb1-140">justification</span></span>|<span data-ttu-id="64fb1-141">String</span><span class="sxs-lookup"><span data-stu-id="64fb1-141">String</span></span>|<span data-ttu-id="64fb1-142">Выставляемое по запросу обоснование.</span><span class="sxs-lookup"><span data-stu-id="64fb1-142">The requestor's supplied justification.</span></span>|
|<span data-ttu-id="64fb1-143">рекуестстате</span><span class="sxs-lookup"><span data-stu-id="64fb1-143">requestState</span></span>|<span data-ttu-id="64fb1-144">String</span><span class="sxs-lookup"><span data-stu-id="64fb1-144">String</span></span>|<span data-ttu-id="64fb1-145">Один из `Denied`, `Delivered` `PartiallyDelivered` или `Submitted`.</span><span class="sxs-lookup"><span data-stu-id="64fb1-145">One of `Denied`, `Delivered`, `PartiallyDelivered` or `Submitted`.</span></span> <span data-ttu-id="64fb1-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64fb1-146">Read-only.</span></span>|
|<span data-ttu-id="64fb1-147">рекуестстатус</span><span class="sxs-lookup"><span data-stu-id="64fb1-147">requestStatus</span></span>|<span data-ttu-id="64fb1-148">String</span><span class="sxs-lookup"><span data-stu-id="64fb1-148">String</span></span>|<span data-ttu-id="64fb1-149">Дополнительные сведения о состоянии обработки запроса.</span><span class="sxs-lookup"><span data-stu-id="64fb1-149">More information on the request processing status.</span></span> <span data-ttu-id="64fb1-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64fb1-150">Read-only.</span></span>|
|<span data-ttu-id="64fb1-151">requestType</span><span class="sxs-lookup"><span data-stu-id="64fb1-151">requestType</span></span>|<span data-ttu-id="64fb1-152">String</span><span class="sxs-lookup"><span data-stu-id="64fb1-152">String</span></span>|<span data-ttu-id="64fb1-153">Один из `UserAdd`, `UserRemove` `AdminAdd` или `AdminRemove`.</span><span class="sxs-lookup"><span data-stu-id="64fb1-153">One of `UserAdd`, `UserRemove`, `AdminAdd` or `AdminRemove`.</span></span> <span data-ttu-id="64fb1-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64fb1-154">Read-only.</span></span>|
|<span data-ttu-id="64fb1-155">акцесспаккажеассигнмент</span><span class="sxs-lookup"><span data-stu-id="64fb1-155">accessPackageAssignment</span></span>|[<span data-ttu-id="64fb1-156">акцесспаккажеассигнмент</span><span class="sxs-lookup"><span data-stu-id="64fb1-156">accessPackageAssignment</span></span>](accesspackageassignment.md)| <span data-ttu-id="64fb1-157">Требуется создать назначение пакета Access.</span><span class="sxs-lookup"><span data-stu-id="64fb1-157">An access package assignment requested to be created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="64fb1-158">Отношения</span><span class="sxs-lookup"><span data-stu-id="64fb1-158">Relationships</span></span>

| <span data-ttu-id="64fb1-159">Связь</span><span class="sxs-lookup"><span data-stu-id="64fb1-159">Relationship</span></span> | <span data-ttu-id="64fb1-160">Тип</span><span class="sxs-lookup"><span data-stu-id="64fb1-160">Type</span></span>        | <span data-ttu-id="64fb1-161">Описание</span><span class="sxs-lookup"><span data-stu-id="64fb1-161">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="64fb1-162">опросчика</span><span class="sxs-lookup"><span data-stu-id="64fb1-162">requestor</span></span>|[<span data-ttu-id="64fb1-163">акцесспаккажесубжект</span><span class="sxs-lookup"><span data-stu-id="64fb1-163">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="64fb1-164">Тема, которая запросила или, если назначено прямое назначение, было назначено.</span><span class="sxs-lookup"><span data-stu-id="64fb1-164">The subject who requested or, if a direct assignment, was assigned.</span></span> <span data-ttu-id="64fb1-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64fb1-165">Read-only.</span></span> <span data-ttu-id="64fb1-166">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="64fb1-166">Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="64fb1-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="64fb1-167">JSON representation</span></span>

<span data-ttu-id="64fb1-168">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64fb1-168">The following is a JSON representation of the resource.</span></span>

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

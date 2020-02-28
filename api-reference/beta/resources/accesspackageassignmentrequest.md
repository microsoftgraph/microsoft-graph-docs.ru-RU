---
title: Тип ресурса Акцесспаккажеассигнментрекуест
description: Запрос на назначение пакета Access создается пользователем, желающим получить назначение пакета Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c2440dfc7e798ea5b0a197f60b62acce4199b4ca
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331271"
---
# <a name="accesspackageassignmentrequest-resource-type"></a><span data-ttu-id="909d3-103">Тип ресурса Акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="909d3-103">accessPackageAssignmentRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="909d3-104">В [управлении обслуживанием в Azure AD](entitlementmanagement-root.md)запрос на назначение пакета Access создается пользователем, желающим получить назначение пакета Access.</span><span class="sxs-lookup"><span data-stu-id="909d3-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="909d3-105">Если запрос выполнен успешно, при наличии необходимых утверждений пользователь получает назначение пакета Access и является темой этого назначенного пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="909d3-105">If the request is successful, with any necessary approvals, the user receives an access package assignment, and is the subject of that resulting access package assignment.</span></span>  <span data-ttu-id="909d3-106">Кроме того, Azure AD автоматически создает запросы на отправку для отслеживания удаления.</span><span class="sxs-lookup"><span data-stu-id="909d3-106">Azure AD also creates access package assignment requests automatically for tracking access removal.</span></span>


## <a name="methods"></a><span data-ttu-id="909d3-107">Методы</span><span class="sxs-lookup"><span data-stu-id="909d3-107">Methods</span></span>

| <span data-ttu-id="909d3-108">Метод</span><span class="sxs-lookup"><span data-stu-id="909d3-108">Method</span></span>       | <span data-ttu-id="909d3-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="909d3-109">Return Type</span></span> | <span data-ttu-id="909d3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="909d3-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="909d3-111">Список Акцесспаккажеассигнментрекуестс</span><span class="sxs-lookup"><span data-stu-id="909d3-111">List accessPackageAssignmentRequests</span></span>](../api/accesspackageassignmentrequest-list.md) | <span data-ttu-id="909d3-112">Коллекция [акцесспаккажеассигнментрекуест](accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="909d3-112">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md) collection</span></span> | <span data-ttu-id="909d3-113">Получение списка объектов акцесспаккажеассигнментрекуест.</span><span class="sxs-lookup"><span data-stu-id="909d3-113">Retrieve a list of accesspackageassignmentrequest objects.</span></span> |
| [<span data-ttu-id="909d3-114">Создание Акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="909d3-114">Create accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-post.md) | [<span data-ttu-id="909d3-115">акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="909d3-115">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="909d3-116">Создание нового Акцесспаккажеассигнментрекуест.</span><span class="sxs-lookup"><span data-stu-id="909d3-116">Create a new accessPackageAssignmentRequest.</span></span> |
| [<span data-ttu-id="909d3-117">Получение Акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="909d3-117">Get accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-get.md) | [<span data-ttu-id="909d3-118">акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="909d3-118">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="909d3-119">Чтение свойств и связей объекта Акцесспаккажеассигнментрекуест.</span><span class="sxs-lookup"><span data-stu-id="909d3-119">Read properties and relationships of an accessPackageAssignmentRequest object.</span></span> |

## <a name="properties"></a><span data-ttu-id="909d3-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="909d3-120">Properties</span></span>

| <span data-ttu-id="909d3-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="909d3-121">Property</span></span>     | <span data-ttu-id="909d3-122">Тип</span><span class="sxs-lookup"><span data-stu-id="909d3-122">Type</span></span>        | <span data-ttu-id="909d3-123">Описание</span><span class="sxs-lookup"><span data-stu-id="909d3-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="909d3-124">комплетеддате</span><span class="sxs-lookup"><span data-stu-id="909d3-124">completedDate</span></span>|<span data-ttu-id="909d3-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="909d3-125">DateTimeOffset</span></span>|<span data-ttu-id="909d3-126">Дата завершения обработки (успешное или неудачное) запроса.</span><span class="sxs-lookup"><span data-stu-id="909d3-126">The date of the end of processing, either successful or failure, of a request.</span></span> <span data-ttu-id="909d3-127">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="909d3-127">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="909d3-128">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="909d3-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="909d3-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="909d3-129">Read-only.</span></span>|
|<span data-ttu-id="909d3-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="909d3-130">createdDateTime</span></span>|<span data-ttu-id="909d3-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="909d3-131">DateTimeOffset</span></span>|<span data-ttu-id="909d3-132">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="909d3-132">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="909d3-133">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="909d3-133">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="909d3-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="909d3-134">Read-only.</span></span>|
|<span data-ttu-id="909d3-135">id</span><span class="sxs-lookup"><span data-stu-id="909d3-135">id</span></span>|<span data-ttu-id="909d3-136">String</span><span class="sxs-lookup"><span data-stu-id="909d3-136">String</span></span>| <span data-ttu-id="909d3-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="909d3-137">Read-only.</span></span>|
|<span data-ttu-id="909d3-138">исвалидатиононли</span><span class="sxs-lookup"><span data-stu-id="909d3-138">isValidationOnly</span></span>|<span data-ttu-id="909d3-139">Логический</span><span class="sxs-lookup"><span data-stu-id="909d3-139">Boolean</span></span>|<span data-ttu-id="909d3-140">Имеет значение true, если запрос не обрабатывается для назначения.</span><span class="sxs-lookup"><span data-stu-id="909d3-140">True if the request is not to be processed for assignment.</span></span>|
|<span data-ttu-id="909d3-141">текста</span><span class="sxs-lookup"><span data-stu-id="909d3-141">justification</span></span>|<span data-ttu-id="909d3-142">String</span><span class="sxs-lookup"><span data-stu-id="909d3-142">String</span></span>|<span data-ttu-id="909d3-143">Выставляемое по запросу обоснование.</span><span class="sxs-lookup"><span data-stu-id="909d3-143">The requestor's supplied justification.</span></span>|
|<span data-ttu-id="909d3-144">рекуестстате</span><span class="sxs-lookup"><span data-stu-id="909d3-144">requestState</span></span>|<span data-ttu-id="909d3-145">String</span><span class="sxs-lookup"><span data-stu-id="909d3-145">String</span></span>|<span data-ttu-id="909d3-146">Один из `Denied`, `Delivered` `PartiallyDelivered`, `Submitted` или `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="909d3-146">One of `Denied`, `Delivered`, `PartiallyDelivered`, `Submitted` or `Scheduled`.</span></span> <span data-ttu-id="909d3-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="909d3-147">Read-only.</span></span>|
|<span data-ttu-id="909d3-148">рекуестстатус</span><span class="sxs-lookup"><span data-stu-id="909d3-148">requestStatus</span></span>|<span data-ttu-id="909d3-149">String</span><span class="sxs-lookup"><span data-stu-id="909d3-149">String</span></span>|<span data-ttu-id="909d3-150">Дополнительные сведения о состоянии обработки запроса.</span><span class="sxs-lookup"><span data-stu-id="909d3-150">More information on the request processing status.</span></span> <span data-ttu-id="909d3-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="909d3-151">Read-only.</span></span>|
|<span data-ttu-id="909d3-152">requestType</span><span class="sxs-lookup"><span data-stu-id="909d3-152">requestType</span></span>|<span data-ttu-id="909d3-153">String</span><span class="sxs-lookup"><span data-stu-id="909d3-153">String</span></span>|<span data-ttu-id="909d3-154">Один из `UserAdd`, `UserRemove` `AdminAdd`, `AdminRemove` или `SystemRemove`.</span><span class="sxs-lookup"><span data-stu-id="909d3-154">One of `UserAdd`, `UserRemove`, `AdminAdd`, `AdminRemove` or `SystemRemove`.</span></span> <span data-ttu-id="909d3-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="909d3-155">Read-only.</span></span>|
|<span data-ttu-id="909d3-156">акцесспаккажеассигнмент</span><span class="sxs-lookup"><span data-stu-id="909d3-156">accessPackageAssignment</span></span>|[<span data-ttu-id="909d3-157">акцесспаккажеассигнмент</span><span class="sxs-lookup"><span data-stu-id="909d3-157">accessPackageAssignment</span></span>](accesspackageassignment.md)| <span data-ttu-id="909d3-158">Требуется создать назначение пакета Access.</span><span class="sxs-lookup"><span data-stu-id="909d3-158">An access package assignment requested to be created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="909d3-159">Связи</span><span class="sxs-lookup"><span data-stu-id="909d3-159">Relationships</span></span>

| <span data-ttu-id="909d3-160">Связь</span><span class="sxs-lookup"><span data-stu-id="909d3-160">Relationship</span></span> | <span data-ttu-id="909d3-161">Тип</span><span class="sxs-lookup"><span data-stu-id="909d3-161">Type</span></span>        | <span data-ttu-id="909d3-162">Описание</span><span class="sxs-lookup"><span data-stu-id="909d3-162">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="909d3-163">опросчика</span><span class="sxs-lookup"><span data-stu-id="909d3-163">requestor</span></span>|[<span data-ttu-id="909d3-164">акцесспаккажесубжект</span><span class="sxs-lookup"><span data-stu-id="909d3-164">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="909d3-165">Тема, которая запросила или, если назначено прямое назначение, было назначено.</span><span class="sxs-lookup"><span data-stu-id="909d3-165">The subject who requested or, if a direct assignment, was assigned.</span></span> <span data-ttu-id="909d3-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="909d3-166">Read-only.</span></span> <span data-ttu-id="909d3-167">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="909d3-167">Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="909d3-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="909d3-168">JSON representation</span></span>

<span data-ttu-id="909d3-169">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="909d3-169">The following is a JSON representation of the resource.</span></span>

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

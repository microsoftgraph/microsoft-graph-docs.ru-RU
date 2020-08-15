---
title: Тип ресурса Акцесспаккажеассигнментрекуест
description: Запрос на назначение пакета Access создается пользователем, желающим получить назначение пакета Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 908d1e4b2fd27895416058a1c8528126dad7ca6b
ms.sourcegitcommit: da4f3d03e98ee5fa13f8c7a263d931e68a20a12c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2020
ms.locfileid: "46757190"
---
# <a name="accesspackageassignmentrequest-resource-type"></a><span data-ttu-id="ebc15-103">Тип ресурса Акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="ebc15-103">accessPackageAssignmentRequest resource type</span></span>

<span data-ttu-id="ebc15-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebc15-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebc15-105">В [управлении обслуживанием в Azure AD](entitlementmanagement-root.md)запрос на назначение пакета Access создается пользователем, желающим получить назначение пакета Access.</span><span class="sxs-lookup"><span data-stu-id="ebc15-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="ebc15-106">Если запрос выполнен успешно, при наличии необходимых утверждений пользователь получает назначение пакета Access и является темой этого назначенного пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="ebc15-106">If the request is successful, with any necessary approvals, the user receives an access package assignment, and is the subject of that resulting access package assignment.</span></span>  <span data-ttu-id="ebc15-107">Кроме того, Azure AD автоматически создает запросы на отправку для отслеживания удаления.</span><span class="sxs-lookup"><span data-stu-id="ebc15-107">Azure AD also creates access package assignment requests automatically for tracking access removal.</span></span>


## <a name="methods"></a><span data-ttu-id="ebc15-108">Методы</span><span class="sxs-lookup"><span data-stu-id="ebc15-108">Methods</span></span>

| <span data-ttu-id="ebc15-109">Метод</span><span class="sxs-lookup"><span data-stu-id="ebc15-109">Method</span></span>       | <span data-ttu-id="ebc15-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ebc15-110">Return Type</span></span> | <span data-ttu-id="ebc15-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ebc15-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ebc15-112">Список Акцесспаккажеассигнментрекуестс</span><span class="sxs-lookup"><span data-stu-id="ebc15-112">List accessPackageAssignmentRequests</span></span>](../api/accesspackageassignmentrequest-list.md) | <span data-ttu-id="ebc15-113">Коллекция [акцесспаккажеассигнментрекуест](accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="ebc15-113">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md) collection</span></span> | <span data-ttu-id="ebc15-114">Получение списка объектов акцесспаккажеассигнментрекуест.</span><span class="sxs-lookup"><span data-stu-id="ebc15-114">Retrieve a list of accesspackageassignmentrequest objects.</span></span> |
| [<span data-ttu-id="ebc15-115">Создание Акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="ebc15-115">Create accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-post.md) | [<span data-ttu-id="ebc15-116">акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="ebc15-116">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="ebc15-117">Создание нового Акцесспаккажеассигнментрекуест.</span><span class="sxs-lookup"><span data-stu-id="ebc15-117">Create a new accessPackageAssignmentRequest.</span></span> |
| [<span data-ttu-id="ebc15-118">Получение Акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="ebc15-118">Get accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-get.md) | [<span data-ttu-id="ebc15-119">акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="ebc15-119">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="ebc15-120">Чтение свойств и связей объекта Акцесспаккажеассигнментрекуест.</span><span class="sxs-lookup"><span data-stu-id="ebc15-120">Read properties and relationships of an accessPackageAssignmentRequest object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ebc15-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="ebc15-121">Properties</span></span>

| <span data-ttu-id="ebc15-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="ebc15-122">Property</span></span>     | <span data-ttu-id="ebc15-123">Тип</span><span class="sxs-lookup"><span data-stu-id="ebc15-123">Type</span></span>        | <span data-ttu-id="ebc15-124">Описание</span><span class="sxs-lookup"><span data-stu-id="ebc15-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ebc15-125">комплетеддате</span><span class="sxs-lookup"><span data-stu-id="ebc15-125">completedDate</span></span>|<span data-ttu-id="ebc15-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebc15-126">DateTimeOffset</span></span>|<span data-ttu-id="ebc15-127">Дата завершения обработки (успешное или неудачное) запроса.</span><span class="sxs-lookup"><span data-stu-id="ebc15-127">The date of the end of processing, either successful or failure, of a request.</span></span> <span data-ttu-id="ebc15-128">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="ebc15-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ebc15-129">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="ebc15-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="ebc15-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ebc15-130">Read-only.</span></span>|
|<span data-ttu-id="ebc15-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ebc15-131">createdDateTime</span></span>|<span data-ttu-id="ebc15-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebc15-132">DateTimeOffset</span></span>|<span data-ttu-id="ebc15-133">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="ebc15-133">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ebc15-134">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="ebc15-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="ebc15-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ebc15-135">Read-only.</span></span>|
|<span data-ttu-id="ebc15-136">id</span><span class="sxs-lookup"><span data-stu-id="ebc15-136">id</span></span>|<span data-ttu-id="ebc15-137">String</span><span class="sxs-lookup"><span data-stu-id="ebc15-137">String</span></span>| <span data-ttu-id="ebc15-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ebc15-138">Read-only.</span></span>|
|<span data-ttu-id="ebc15-139">исвалидатиононли</span><span class="sxs-lookup"><span data-stu-id="ebc15-139">isValidationOnly</span></span>|<span data-ttu-id="ebc15-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="ebc15-140">Boolean</span></span>|<span data-ttu-id="ebc15-141">Имеет значение true, если запрос не обрабатывается для назначения.</span><span class="sxs-lookup"><span data-stu-id="ebc15-141">True if the request is not to be processed for assignment.</span></span>|
|<span data-ttu-id="ebc15-142">текста</span><span class="sxs-lookup"><span data-stu-id="ebc15-142">justification</span></span>|<span data-ttu-id="ebc15-143">Строка</span><span class="sxs-lookup"><span data-stu-id="ebc15-143">String</span></span>|<span data-ttu-id="ebc15-144">Выставляемое по запросу обоснование.</span><span class="sxs-lookup"><span data-stu-id="ebc15-144">The requestor's supplied justification.</span></span>|
|<span data-ttu-id="ebc15-145">рекуестстате</span><span class="sxs-lookup"><span data-stu-id="ebc15-145">requestState</span></span>|<span data-ttu-id="ebc15-146">Строка</span><span class="sxs-lookup"><span data-stu-id="ebc15-146">String</span></span>|<span data-ttu-id="ebc15-147">Один из `PendingApproval` ,,,,, `Canceled`  `Denied` `Delivering` `Delivered` `PartiallyDelivered` , `Submitted` или `Scheduled` .</span><span class="sxs-lookup"><span data-stu-id="ebc15-147">One of `PendingApproval`, `Canceled`,  `Denied`, `Delivering`, `Delivered`, `PartiallyDelivered`, `Submitted` or `Scheduled`.</span></span> <span data-ttu-id="ebc15-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ebc15-148">Read-only.</span></span>|
|<span data-ttu-id="ebc15-149">рекуестстатус</span><span class="sxs-lookup"><span data-stu-id="ebc15-149">requestStatus</span></span>|<span data-ttu-id="ebc15-150">Строка</span><span class="sxs-lookup"><span data-stu-id="ebc15-150">String</span></span>|<span data-ttu-id="ebc15-151">Дополнительные сведения о состоянии обработки запроса.</span><span class="sxs-lookup"><span data-stu-id="ebc15-151">More information on the request processing status.</span></span> <span data-ttu-id="ebc15-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ebc15-152">Read-only.</span></span>|
|<span data-ttu-id="ebc15-153">requestType</span><span class="sxs-lookup"><span data-stu-id="ebc15-153">requestType</span></span>|<span data-ttu-id="ebc15-154">Строка</span><span class="sxs-lookup"><span data-stu-id="ebc15-154">String</span></span>|<span data-ttu-id="ebc15-155">Один из `UserAdd` , `UserRemove` , `AdminAdd` `AdminRemove` или `SystemRemove` .</span><span class="sxs-lookup"><span data-stu-id="ebc15-155">One of `UserAdd`, `UserRemove`, `AdminAdd`, `AdminRemove` or `SystemRemove`.</span></span> <span data-ttu-id="ebc15-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ebc15-156">Read-only.</span></span>|
|<span data-ttu-id="ebc15-157">акцесспаккажеассигнмент</span><span class="sxs-lookup"><span data-stu-id="ebc15-157">accessPackageAssignment</span></span>|[<span data-ttu-id="ebc15-158">акцесспаккажеассигнмент</span><span class="sxs-lookup"><span data-stu-id="ebc15-158">accessPackageAssignment</span></span>](accesspackageassignment.md)| <span data-ttu-id="ebc15-159">Требуется создать назначение пакета Access.</span><span class="sxs-lookup"><span data-stu-id="ebc15-159">An access package assignment requested to be created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebc15-160">Связи</span><span class="sxs-lookup"><span data-stu-id="ebc15-160">Relationships</span></span>

| <span data-ttu-id="ebc15-161">Связь</span><span class="sxs-lookup"><span data-stu-id="ebc15-161">Relationship</span></span> | <span data-ttu-id="ebc15-162">Тип</span><span class="sxs-lookup"><span data-stu-id="ebc15-162">Type</span></span>        | <span data-ttu-id="ebc15-163">Описание</span><span class="sxs-lookup"><span data-stu-id="ebc15-163">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ebc15-164">опросчика</span><span class="sxs-lookup"><span data-stu-id="ebc15-164">requestor</span></span>|[<span data-ttu-id="ebc15-165">акцесспаккажесубжект</span><span class="sxs-lookup"><span data-stu-id="ebc15-165">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="ebc15-166">Тема, которая запросила или, если назначено прямое назначение, было назначено.</span><span class="sxs-lookup"><span data-stu-id="ebc15-166">The subject who requested or, if a direct assignment, was assigned.</span></span> <span data-ttu-id="ebc15-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ebc15-167">Read-only.</span></span> <span data-ttu-id="ebc15-168">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="ebc15-168">Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="ebc15-169">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ebc15-169">JSON representation</span></span>

<span data-ttu-id="ebc15-170">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ebc15-170">The following is a JSON representation of the resource.</span></span>

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

---
title: Тип ресурса accessPackageAssignmentRequest
description: Запрос на назначение пакета доступа создается пользователем, который хочет получить назначение пакета доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7ce7d47ccb4e911689e9398c2514cb8311b3ae0a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155613"
---
# <a name="accesspackageassignmentrequest-resource-type"></a><span data-ttu-id="9fc6c-103">Тип ресурса accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="9fc6c-103">accessPackageAssignmentRequest resource type</span></span>

<span data-ttu-id="9fc6c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fc6c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fc6c-105">В [управлении правами Azure AD](entitlementmanagement-root.md)запрос на назначение пакета доступа создается пользователем, который хочет получить назначение пакета доступа, или от его имени.</span><span class="sxs-lookup"><span data-stu-id="9fc6c-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by or on behalf of a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="9fc6c-106">В случае успешного выполнения запроса с необходимыми утверждениями пользователь получает назначение пакета доступа и является субъектом этого назначения пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="9fc6c-106">If the request is successful, with any necessary approvals, the user receives an access package assignment, and is the subject of that resulting access package assignment.</span></span>  <span data-ttu-id="9fc6c-107">Azure AD также автоматически создает запросы на назначение пакета доступа для отслеживания удаления доступа.</span><span class="sxs-lookup"><span data-stu-id="9fc6c-107">Azure AD also creates access package assignment requests automatically for tracking access removal.</span></span>

## <a name="methods"></a><span data-ttu-id="9fc6c-108">Методы</span><span class="sxs-lookup"><span data-stu-id="9fc6c-108">Methods</span></span>

| <span data-ttu-id="9fc6c-109">Метод</span><span class="sxs-lookup"><span data-stu-id="9fc6c-109">Method</span></span>       | <span data-ttu-id="9fc6c-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9fc6c-110">Return Type</span></span> | <span data-ttu-id="9fc6c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9fc6c-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9fc6c-112">Список accessPackageAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="9fc6c-112">List accessPackageAssignmentRequests</span></span>](../api/accesspackageassignmentrequest-list.md) | <span data-ttu-id="9fc6c-113">[Коллекция accessPackageAssignmentRequest](accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="9fc6c-113">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md) collection</span></span> | <span data-ttu-id="9fc6c-114">Получить список объектов accesspackageassignmentrequest.</span><span class="sxs-lookup"><span data-stu-id="9fc6c-114">Retrieve a list of accesspackageassignmentrequest objects.</span></span> |
| [<span data-ttu-id="9fc6c-115">Создание accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="9fc6c-115">Create accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-post.md) | [<span data-ttu-id="9fc6c-116">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="9fc6c-116">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="9fc6c-117">Создайте новый accessPackageAssignmentRequest.</span><span class="sxs-lookup"><span data-stu-id="9fc6c-117">Create a new accessPackageAssignmentRequest.</span></span> |
| [<span data-ttu-id="9fc6c-118">Get accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="9fc6c-118">Get accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-get.md) | [<span data-ttu-id="9fc6c-119">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="9fc6c-119">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="9fc6c-120">Чтение свойств и связей объекта accessPackageAssignmentRequest.</span><span class="sxs-lookup"><span data-stu-id="9fc6c-120">Read properties and relationships of an accessPackageAssignmentRequest object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9fc6c-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="9fc6c-121">Properties</span></span>

| <span data-ttu-id="9fc6c-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="9fc6c-122">Property</span></span>     | <span data-ttu-id="9fc6c-123">Тип</span><span class="sxs-lookup"><span data-stu-id="9fc6c-123">Type</span></span>        | <span data-ttu-id="9fc6c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="9fc6c-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9fc6c-125">completedDate</span><span class="sxs-lookup"><span data-stu-id="9fc6c-125">completedDate</span></span>|<span data-ttu-id="9fc6c-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fc6c-126">DateTimeOffset</span></span>|<span data-ttu-id="9fc6c-127">Дата окончания обработки (успешного или неудачного) запроса.</span><span class="sxs-lookup"><span data-stu-id="9fc6c-127">The date of the end of processing, either successful or failure, of a request.</span></span> <span data-ttu-id="9fc6c-128">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="9fc6c-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9fc6c-129">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9fc6c-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="9fc6c-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9fc6c-130">Read-only.</span></span>|
|<span data-ttu-id="9fc6c-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9fc6c-131">createdDateTime</span></span>|<span data-ttu-id="9fc6c-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fc6c-132">DateTimeOffset</span></span>|<span data-ttu-id="9fc6c-133">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="9fc6c-133">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9fc6c-134">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9fc6c-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="9fc6c-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9fc6c-135">Read-only.</span></span>|
|<span data-ttu-id="9fc6c-136">id</span><span class="sxs-lookup"><span data-stu-id="9fc6c-136">id</span></span>|<span data-ttu-id="9fc6c-137">String</span><span class="sxs-lookup"><span data-stu-id="9fc6c-137">String</span></span>| <span data-ttu-id="9fc6c-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9fc6c-138">Read-only.</span></span>|
|<span data-ttu-id="9fc6c-139">isValidationOnly</span><span class="sxs-lookup"><span data-stu-id="9fc6c-139">isValidationOnly</span></span>|<span data-ttu-id="9fc6c-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="9fc6c-140">Boolean</span></span>|<span data-ttu-id="9fc6c-141">Имеет true, если запрос не обрабатывается для назначения.</span><span class="sxs-lookup"><span data-stu-id="9fc6c-141">True if the request is not to be processed for assignment.</span></span>|
|<span data-ttu-id="9fc6c-142">обоснование</span><span class="sxs-lookup"><span data-stu-id="9fc6c-142">justification</span></span>|<span data-ttu-id="9fc6c-143">String</span><span class="sxs-lookup"><span data-stu-id="9fc6c-143">String</span></span>|<span data-ttu-id="9fc6c-144">Предоставленная запросителем обоснование.</span><span class="sxs-lookup"><span data-stu-id="9fc6c-144">The requestor's supplied justification.</span></span>|
|<span data-ttu-id="9fc6c-145">requestState</span><span class="sxs-lookup"><span data-stu-id="9fc6c-145">requestState</span></span>|<span data-ttu-id="9fc6c-146">String</span><span class="sxs-lookup"><span data-stu-id="9fc6c-146">String</span></span>|<span data-ttu-id="9fc6c-147">Один из `PendingApproval` , , , , , , или `Canceled`  `Denied` `Delivering` `Delivered` `PartiallyDelivered` `Submitted` `Scheduled` .</span><span class="sxs-lookup"><span data-stu-id="9fc6c-147">One of `PendingApproval`, `Canceled`,  `Denied`, `Delivering`, `Delivered`, `PartiallyDelivered`, `Submitted` or `Scheduled`.</span></span> <span data-ttu-id="9fc6c-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9fc6c-148">Read-only.</span></span>|
|<span data-ttu-id="9fc6c-149">requestStatus</span><span class="sxs-lookup"><span data-stu-id="9fc6c-149">requestStatus</span></span>|<span data-ttu-id="9fc6c-150">String</span><span class="sxs-lookup"><span data-stu-id="9fc6c-150">String</span></span>|<span data-ttu-id="9fc6c-151">Дополнительные сведения о состоянии обработки запроса.</span><span class="sxs-lookup"><span data-stu-id="9fc6c-151">More information on the request processing status.</span></span> <span data-ttu-id="9fc6c-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9fc6c-152">Read-only.</span></span>|
|<span data-ttu-id="9fc6c-153">requestType</span><span class="sxs-lookup"><span data-stu-id="9fc6c-153">requestType</span></span>|<span data-ttu-id="9fc6c-154">String</span><span class="sxs-lookup"><span data-stu-id="9fc6c-154">String</span></span>|<span data-ttu-id="9fc6c-155">Один из `UserAdd` , , , или `UserRemove` `AdminAdd` `AdminRemove` `SystemRemove` .</span><span class="sxs-lookup"><span data-stu-id="9fc6c-155">One of `UserAdd`, `UserRemove`, `AdminAdd`, `AdminRemove` or `SystemRemove`.</span></span> <span data-ttu-id="9fc6c-156">Запрос от самого пользователя будет иметь requestType или `UserAdd` `UserRemove` .</span><span class="sxs-lookup"><span data-stu-id="9fc6c-156">A request from the user themselves would have requestType of `UserAdd` or `UserRemove`.</span></span> <span data-ttu-id="9fc6c-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9fc6c-157">Read-only.</span></span>|
|<span data-ttu-id="9fc6c-158">schedule</span><span class="sxs-lookup"><span data-stu-id="9fc6c-158">schedule</span></span>|[<span data-ttu-id="9fc6c-159">requestSchedule</span><span class="sxs-lookup"><span data-stu-id="9fc6c-159">requestSchedule</span></span>](requestschedule.md)| <span data-ttu-id="9fc6c-160">Диапазон дат, в которые должен быть назначен доступ запрашиваемой информации.</span><span class="sxs-lookup"><span data-stu-id="9fc6c-160">The range of dates that access is to be assigned to the requestor.</span></span> <span data-ttu-id="9fc6c-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9fc6c-161">Read-only.</span></span>|
|<span data-ttu-id="9fc6c-162">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="9fc6c-162">accessPackageAssignment</span></span>|[<span data-ttu-id="9fc6c-163">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="9fc6c-163">accessPackageAssignment</span></span>](accesspackageassignment.md)| <span data-ttu-id="9fc6c-164">Для requestType или , это назначение пакета доступа `UserAdd` `AdminAdd` запрашивается для создания.</span><span class="sxs-lookup"><span data-stu-id="9fc6c-164">For a requestType of `UserAdd` or `AdminAdd`, this is an access package assignment requested to be created.</span></span>  <span data-ttu-id="9fc6c-165">Для объекта requestType или , это свойство существующего `UserRemove` `AdminRemove` `SystemRemove` `id` назначения, который необходимо удалить.</span><span class="sxs-lookup"><span data-stu-id="9fc6c-165">For a requestType of `UserRemove`, `AdminRemove` or `SystemRemove`, this has the `id` property of an existing assignment to be removed.</span></span>|
|<span data-ttu-id="9fc6c-166">answers</span><span class="sxs-lookup"><span data-stu-id="9fc6c-166">answers</span></span>|<span data-ttu-id="9fc6c-167">[Коллекция accessPackageAnswer](accesspackageanswer.md)</span><span class="sxs-lookup"><span data-stu-id="9fc6c-167">[accessPackageAnswer](accesspackageanswer.md) collection</span></span>|<span data-ttu-id="9fc6c-168">Ответы, предоставленные запрашивателем [для accessPackageQuestions,](accesspackagequestion.md) которые запрашивали их во время запроса.</span><span class="sxs-lookup"><span data-stu-id="9fc6c-168">Answers provided by the requestor to [accessPackageQuestions](accesspackagequestion.md) asked of them at the time of request.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9fc6c-169">Связи</span><span class="sxs-lookup"><span data-stu-id="9fc6c-169">Relationships</span></span>

| <span data-ttu-id="9fc6c-170">Связь</span><span class="sxs-lookup"><span data-stu-id="9fc6c-170">Relationship</span></span> | <span data-ttu-id="9fc6c-171">Тип</span><span class="sxs-lookup"><span data-stu-id="9fc6c-171">Type</span></span>        | <span data-ttu-id="9fc6c-172">Описание</span><span class="sxs-lookup"><span data-stu-id="9fc6c-172">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9fc6c-173">requestor</span><span class="sxs-lookup"><span data-stu-id="9fc6c-173">requestor</span></span>|[<span data-ttu-id="9fc6c-174">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="9fc6c-174">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="9fc6c-175">Субъект, запросивший или, если прямое назначение, был назначен.</span><span class="sxs-lookup"><span data-stu-id="9fc6c-175">The subject who requested or, if a direct assignment, was assigned.</span></span> <span data-ttu-id="9fc6c-176">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9fc6c-176">Read-only.</span></span> <span data-ttu-id="9fc6c-177">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9fc6c-177">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9fc6c-178">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9fc6c-178">JSON representation</span></span>

<span data-ttu-id="9fc6c-179">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9fc6c-179">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest",
  "keyProperty": "id"
}-->

```json
{
    "createdDateTime": "string",
    "completedDate": "string",
    "id": "string",
    "requestType": "string",
    "requestState": "string",
    "requestStatus": "string",
    "isValidationOnly": false,
    "justification": "string",
    "answers": [{
        "@odata.type": "#microsoft.graph.accessPackageAnswerString",
        "value": "string",
        "answeredQuestion": {
            "id": "string",
            "text": {
                "defaultText": "string",
                "localizedTexts": [{
                    "text": "string",
                    "languageCode": "string"
                }]
            },
            "isRequired": true,
            "@odata.type": "#microsoft.graph.accessPackageTextInputQuestion",
            "isSingleLineQuestion": true
        }
    }]
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


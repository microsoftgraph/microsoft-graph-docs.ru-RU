---
title: Тип ресурса accessPackageAssignmentRequest
description: Запрос на назначение пакета доступа создается пользователем, который хочет получить назначение пакета доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9ecaa9b77a92dc6393b3c7231976937e36502c8d
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49719757"
---
# <a name="accesspackageassignmentrequest-resource-type"></a><span data-ttu-id="f05d3-103">Тип ресурса accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="f05d3-103">accessPackageAssignmentRequest resource type</span></span>

<span data-ttu-id="f05d3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f05d3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f05d3-105">В [управлении правами Azure AD](entitlementmanagement-root.md)запрос на назначение пакета доступа создается пользователем, который хочет получить назначение пакета доступа, или от его имени.</span><span class="sxs-lookup"><span data-stu-id="f05d3-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by or on behalf of a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="f05d3-106">В случае успешного выполнения запроса с любыми необходимыми утверждениями пользователь получает назначение пакета доступа и является субъектом этого назначения пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="f05d3-106">If the request is successful, with any necessary approvals, the user receives an access package assignment, and is the subject of that resulting access package assignment.</span></span>  <span data-ttu-id="f05d3-107">Azure AD также автоматически создает запросы на назначение пакета доступа для отслеживания удаления доступа.</span><span class="sxs-lookup"><span data-stu-id="f05d3-107">Azure AD also creates access package assignment requests automatically for tracking access removal.</span></span>

## <a name="methods"></a><span data-ttu-id="f05d3-108">Методы</span><span class="sxs-lookup"><span data-stu-id="f05d3-108">Methods</span></span>

| <span data-ttu-id="f05d3-109">Метод</span><span class="sxs-lookup"><span data-stu-id="f05d3-109">Method</span></span>       | <span data-ttu-id="f05d3-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f05d3-110">Return Type</span></span> | <span data-ttu-id="f05d3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f05d3-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f05d3-112">Список accessPackageAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="f05d3-112">List accessPackageAssignmentRequests</span></span>](../api/accesspackageassignmentrequest-list.md) | <span data-ttu-id="f05d3-113">[Коллекция accessPackageAssignmentRequest](accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="f05d3-113">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md) collection</span></span> | <span data-ttu-id="f05d3-114">Получить список объектов accesspackageassignmentrequest.</span><span class="sxs-lookup"><span data-stu-id="f05d3-114">Retrieve a list of accesspackageassignmentrequest objects.</span></span> |
| [<span data-ttu-id="f05d3-115">Создание accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="f05d3-115">Create accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-post.md) | [<span data-ttu-id="f05d3-116">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="f05d3-116">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="f05d3-117">Создайте новый accessPackageAssignmentRequest.</span><span class="sxs-lookup"><span data-stu-id="f05d3-117">Create a new accessPackageAssignmentRequest.</span></span> |
| [<span data-ttu-id="f05d3-118">Get accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="f05d3-118">Get accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-get.md) | [<span data-ttu-id="f05d3-119">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="f05d3-119">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="f05d3-120">Чтение свойств и связей объекта accessPackageAssignmentRequest.</span><span class="sxs-lookup"><span data-stu-id="f05d3-120">Read properties and relationships of an accessPackageAssignmentRequest object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f05d3-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="f05d3-121">Properties</span></span>

| <span data-ttu-id="f05d3-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="f05d3-122">Property</span></span>     | <span data-ttu-id="f05d3-123">Тип</span><span class="sxs-lookup"><span data-stu-id="f05d3-123">Type</span></span>        | <span data-ttu-id="f05d3-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f05d3-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f05d3-125">completedDate</span><span class="sxs-lookup"><span data-stu-id="f05d3-125">completedDate</span></span>|<span data-ttu-id="f05d3-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f05d3-126">DateTimeOffset</span></span>|<span data-ttu-id="f05d3-127">Дата окончания обработки (успешного или неудачного) запроса.</span><span class="sxs-lookup"><span data-stu-id="f05d3-127">The date of the end of processing, either successful or failure, of a request.</span></span> <span data-ttu-id="f05d3-128">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="f05d3-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f05d3-129">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f05d3-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="f05d3-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f05d3-130">Read-only.</span></span>|
|<span data-ttu-id="f05d3-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f05d3-131">createdDateTime</span></span>|<span data-ttu-id="f05d3-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f05d3-132">DateTimeOffset</span></span>|<span data-ttu-id="f05d3-133">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="f05d3-133">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f05d3-134">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f05d3-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="f05d3-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f05d3-135">Read-only.</span></span>|
|<span data-ttu-id="f05d3-136">id</span><span class="sxs-lookup"><span data-stu-id="f05d3-136">id</span></span>|<span data-ttu-id="f05d3-137">String</span><span class="sxs-lookup"><span data-stu-id="f05d3-137">String</span></span>| <span data-ttu-id="f05d3-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f05d3-138">Read-only.</span></span>|
|<span data-ttu-id="f05d3-139">isValidationOnly</span><span class="sxs-lookup"><span data-stu-id="f05d3-139">isValidationOnly</span></span>|<span data-ttu-id="f05d3-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="f05d3-140">Boolean</span></span>|<span data-ttu-id="f05d3-141">Имеет true, если запрос не обрабатывается для назначения.</span><span class="sxs-lookup"><span data-stu-id="f05d3-141">True if the request is not to be processed for assignment.</span></span>|
|<span data-ttu-id="f05d3-142">обоснование</span><span class="sxs-lookup"><span data-stu-id="f05d3-142">justification</span></span>|<span data-ttu-id="f05d3-143">String</span><span class="sxs-lookup"><span data-stu-id="f05d3-143">String</span></span>|<span data-ttu-id="f05d3-144">Предоставленная запросителем обоснование.</span><span class="sxs-lookup"><span data-stu-id="f05d3-144">The requestor's supplied justification.</span></span>|
|<span data-ttu-id="f05d3-145">requestState</span><span class="sxs-lookup"><span data-stu-id="f05d3-145">requestState</span></span>|<span data-ttu-id="f05d3-146">String</span><span class="sxs-lookup"><span data-stu-id="f05d3-146">String</span></span>|<span data-ttu-id="f05d3-147">Один из `PendingApproval` , , , или `Canceled`  `Denied` `Delivering` `Delivered` `PartiallyDelivered` `Submitted` `Scheduled` .</span><span class="sxs-lookup"><span data-stu-id="f05d3-147">One of `PendingApproval`, `Canceled`,  `Denied`, `Delivering`, `Delivered`, `PartiallyDelivered`, `Submitted` or `Scheduled`.</span></span> <span data-ttu-id="f05d3-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f05d3-148">Read-only.</span></span>|
|<span data-ttu-id="f05d3-149">requestStatus</span><span class="sxs-lookup"><span data-stu-id="f05d3-149">requestStatus</span></span>|<span data-ttu-id="f05d3-150">String</span><span class="sxs-lookup"><span data-stu-id="f05d3-150">String</span></span>|<span data-ttu-id="f05d3-151">Дополнительные сведения о состоянии обработки запроса.</span><span class="sxs-lookup"><span data-stu-id="f05d3-151">More information on the request processing status.</span></span> <span data-ttu-id="f05d3-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f05d3-152">Read-only.</span></span>|
|<span data-ttu-id="f05d3-153">requestType</span><span class="sxs-lookup"><span data-stu-id="f05d3-153">requestType</span></span>|<span data-ttu-id="f05d3-154">String</span><span class="sxs-lookup"><span data-stu-id="f05d3-154">String</span></span>|<span data-ttu-id="f05d3-155">Один из `UserAdd` , , , или `UserRemove` `AdminAdd` `AdminRemove` `SystemRemove` .</span><span class="sxs-lookup"><span data-stu-id="f05d3-155">One of `UserAdd`, `UserRemove`, `AdminAdd`, `AdminRemove` or `SystemRemove`.</span></span> <span data-ttu-id="f05d3-156">Запрос от самого пользователя будет иметь requestType или `UserAdd` `UserRemove` .</span><span class="sxs-lookup"><span data-stu-id="f05d3-156">A request from the user themselves would have requestType of `UserAdd` or `UserRemove`.</span></span> <span data-ttu-id="f05d3-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f05d3-157">Read-only.</span></span>|
|<span data-ttu-id="f05d3-158">schedule</span><span class="sxs-lookup"><span data-stu-id="f05d3-158">schedule</span></span>|[<span data-ttu-id="f05d3-159">requestSchedule</span><span class="sxs-lookup"><span data-stu-id="f05d3-159">requestSchedule</span></span>](requestschedule.md)| <span data-ttu-id="f05d3-160">Диапазон дат, в которые должен быть назначен доступ запрашиваемой информации.</span><span class="sxs-lookup"><span data-stu-id="f05d3-160">The range of dates that access is to be assigned to the requestor.</span></span> <span data-ttu-id="f05d3-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f05d3-161">Read-only.</span></span>|
|<span data-ttu-id="f05d3-162">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="f05d3-162">accessPackageAssignment</span></span>|[<span data-ttu-id="f05d3-163">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="f05d3-163">accessPackageAssignment</span></span>](accesspackageassignment.md)| <span data-ttu-id="f05d3-164">Для requestType или , это назначение пакета доступа `UserAdd` `AdminAdd` запрашивается для создания.</span><span class="sxs-lookup"><span data-stu-id="f05d3-164">For a requestType of `UserAdd` or `AdminAdd`, this is an access package assignment requested to be created.</span></span>  <span data-ttu-id="f05d3-165">Для объекта requestType или , это свойство существующего `UserRemove` `AdminRemove` `SystemRemove` `id` назначения, который необходимо удалить.</span><span class="sxs-lookup"><span data-stu-id="f05d3-165">For a requestType of `UserRemove`, `AdminRemove` or `SystemRemove`, this has the `id` property of an existing assignment to be removed.</span></span>|
|<span data-ttu-id="f05d3-166">answers</span><span class="sxs-lookup"><span data-stu-id="f05d3-166">answers</span></span>|<span data-ttu-id="f05d3-167">[Коллекция accessPackageAnswer](accesspackageanswer.md)</span><span class="sxs-lookup"><span data-stu-id="f05d3-167">[accessPackageAnswer](accesspackageanswer.md) collection</span></span>|<span data-ttu-id="f05d3-168">Ответы, предоставленные запрашивателем [для accessPackageQuestions,](accesspackagequestion.md) которые запрашивали их во время запроса.</span><span class="sxs-lookup"><span data-stu-id="f05d3-168">Answers provided by the requestor to [accessPackageQuestions](accesspackagequestion.md) asked of them at the time of request.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f05d3-169">Отношения</span><span class="sxs-lookup"><span data-stu-id="f05d3-169">Relationships</span></span>

| <span data-ttu-id="f05d3-170">Связь</span><span class="sxs-lookup"><span data-stu-id="f05d3-170">Relationship</span></span> | <span data-ttu-id="f05d3-171">Тип</span><span class="sxs-lookup"><span data-stu-id="f05d3-171">Type</span></span>        | <span data-ttu-id="f05d3-172">Описание</span><span class="sxs-lookup"><span data-stu-id="f05d3-172">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f05d3-173">requestor</span><span class="sxs-lookup"><span data-stu-id="f05d3-173">requestor</span></span>|[<span data-ttu-id="f05d3-174">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="f05d3-174">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="f05d3-175">Субъект, запросивший или, если прямое назначение, был назначен.</span><span class="sxs-lookup"><span data-stu-id="f05d3-175">The subject who requested or, if a direct assignment, was assigned.</span></span> <span data-ttu-id="f05d3-176">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f05d3-176">Read-only.</span></span> <span data-ttu-id="f05d3-177">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f05d3-177">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f05d3-178">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f05d3-178">JSON representation</span></span>

<span data-ttu-id="f05d3-179">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f05d3-179">The following is a JSON representation of the resource.</span></span>

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


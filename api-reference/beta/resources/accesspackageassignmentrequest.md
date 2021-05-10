---
title: тип ресурса accessPackageAssignmentRequest
description: Запрос на назначение пакета доступа создается пользователем, который хочет получить назначение пакета доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7825b19e80274c8bcd54a5d8d03aa1dd40cf49c9
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52298500"
---
# <a name="accesspackageassignmentrequest-resource-type"></a><span data-ttu-id="88d6f-103">тип ресурса accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="88d6f-103">accessPackageAssignmentRequest resource type</span></span>

<span data-ttu-id="88d6f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88d6f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88d6f-105">В [Azure AD Entitlement Management](entitlementmanagement-root.md)запрос на назначение пакета доступа создается пользователем или от имени пользователя, который хочет получить назначение пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="88d6f-105">In [Azure AD Entitlement Management](entitlementmanagement-root.md), an access package assignment request is created by or on behalf of a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="88d6f-106">Если запрос является успешным, с любыми необходимыми утверждениями, пользователь получает назначение пакета доступа и является субъектом этого назначения пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="88d6f-106">If the request is successful, with any necessary approvals, the user receives an access package assignment, and is the subject of that resulting access package assignment.</span></span>  <span data-ttu-id="88d6f-107">Azure AD также создает запросы на назначение пакетов доступа автоматически для отслеживания удаления доступа.</span><span class="sxs-lookup"><span data-stu-id="88d6f-107">Azure AD also creates access package assignment requests automatically for tracking access removal.</span></span>

## <a name="methods"></a><span data-ttu-id="88d6f-108">Методы</span><span class="sxs-lookup"><span data-stu-id="88d6f-108">Methods</span></span>

| <span data-ttu-id="88d6f-109">Метод</span><span class="sxs-lookup"><span data-stu-id="88d6f-109">Method</span></span>       | <span data-ttu-id="88d6f-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="88d6f-110">Return Type</span></span> | <span data-ttu-id="88d6f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="88d6f-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="88d6f-112">Список accessPackageAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="88d6f-112">List accessPackageAssignmentRequests</span></span>](../api/accesspackageassignmentrequest-list.md) | <span data-ttu-id="88d6f-113">[accessPackageAssignmentRequest collection](accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="88d6f-113">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md) collection</span></span> | <span data-ttu-id="88d6f-114">Извлечение списка **объектов accesspackageassignmentrequest.**</span><span class="sxs-lookup"><span data-stu-id="88d6f-114">Retrieve a list of **accesspackageassignmentrequest** objects.</span></span> |
| [<span data-ttu-id="88d6f-115">Создание accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="88d6f-115">Create accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-post.md) | [<span data-ttu-id="88d6f-116">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="88d6f-116">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="88d6f-117">Создание нового **accessPackageAssignmentRequest**.</span><span class="sxs-lookup"><span data-stu-id="88d6f-117">Create a new **accessPackageAssignmentRequest**.</span></span> |
| [<span data-ttu-id="88d6f-118">Получить accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="88d6f-118">Get accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-get.md) | [<span data-ttu-id="88d6f-119">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="88d6f-119">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="88d6f-120">Чтение свойств и связей объекта **accessPackageAssignmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="88d6f-120">Read properties and relationships of an **accessPackageAssignmentRequest** object.</span></span> |
|[<span data-ttu-id="88d6f-121">filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="88d6f-121">filterByCurrentUser</span></span>](../api/accesspackageassignmentrequest-filterbycurrentuser.md)|<span data-ttu-id="88d6f-122">[accessPackageAssignmentRequest collection](../resources/accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="88d6f-122">[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) collection</span></span>|<span data-ttu-id="88d6f-123">Извлечение списка **объектов accessPackageAssignmentRequest,** фильтруемых на входе пользователя.</span><span class="sxs-lookup"><span data-stu-id="88d6f-123">Retrieve the list of **accessPackageAssignmentRequest** objects filtered on the signed-in user.</span></span>|
|[<span data-ttu-id="88d6f-124">cancel</span><span class="sxs-lookup"><span data-stu-id="88d6f-124">cancel</span></span>](../api/accesspackageassignmentrequest-cancel.md)|<span data-ttu-id="88d6f-125">[accessPackageAssignmentRequest collection](../resources/accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="88d6f-125">[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) collection</span></span>|<span data-ttu-id="88d6f-126">Отмена **объекта accessPackageAssignmentRequest,** который находится в отменяемом состоянии.</span><span class="sxs-lookup"><span data-stu-id="88d6f-126">Cancel an **accessPackageAssignmentRequest** object that is in a cancellable state.</span></span>|

## <a name="properties"></a><span data-ttu-id="88d6f-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="88d6f-127">Properties</span></span>

| <span data-ttu-id="88d6f-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="88d6f-128">Property</span></span>     | <span data-ttu-id="88d6f-129">Тип</span><span class="sxs-lookup"><span data-stu-id="88d6f-129">Type</span></span>        | <span data-ttu-id="88d6f-130">Описание</span><span class="sxs-lookup"><span data-stu-id="88d6f-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="88d6f-131">completedDate</span><span class="sxs-lookup"><span data-stu-id="88d6f-131">completedDate</span></span>|<span data-ttu-id="88d6f-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88d6f-132">DateTimeOffset</span></span>|<span data-ttu-id="88d6f-133">Дата окончания обработки , успешной или неудачной, запроса.</span><span class="sxs-lookup"><span data-stu-id="88d6f-133">The date of the end of processing, either successful or failure, of a request.</span></span> <span data-ttu-id="88d6f-134">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="88d6f-134">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="88d6f-135">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="88d6f-135">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="88d6f-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="88d6f-136">Read-only.</span></span>|
|<span data-ttu-id="88d6f-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="88d6f-137">createdDateTime</span></span>|<span data-ttu-id="88d6f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88d6f-138">DateTimeOffset</span></span>|<span data-ttu-id="88d6f-139">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="88d6f-139">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="88d6f-140">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="88d6f-140">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="88d6f-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="88d6f-141">Read-only.</span></span>|
|<span data-ttu-id="88d6f-142">id</span><span class="sxs-lookup"><span data-stu-id="88d6f-142">id</span></span>|<span data-ttu-id="88d6f-143">String</span><span class="sxs-lookup"><span data-stu-id="88d6f-143">String</span></span>| <span data-ttu-id="88d6f-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="88d6f-144">Read-only.</span></span>|
|<span data-ttu-id="88d6f-145">isValidationOnly</span><span class="sxs-lookup"><span data-stu-id="88d6f-145">isValidationOnly</span></span>|<span data-ttu-id="88d6f-146">Логический</span><span class="sxs-lookup"><span data-stu-id="88d6f-146">Boolean</span></span>|<span data-ttu-id="88d6f-147">True, если запрос не обрабатывается для назначения.</span><span class="sxs-lookup"><span data-stu-id="88d6f-147">True if the request is not to be processed for assignment.</span></span>|
|<span data-ttu-id="88d6f-148">обоснование</span><span class="sxs-lookup"><span data-stu-id="88d6f-148">justification</span></span>|<span data-ttu-id="88d6f-149">Строка</span><span class="sxs-lookup"><span data-stu-id="88d6f-149">String</span></span>|<span data-ttu-id="88d6f-150">Предоставлено обоснование запроса.</span><span class="sxs-lookup"><span data-stu-id="88d6f-150">The requestor's supplied justification.</span></span>|
|<span data-ttu-id="88d6f-151">requestState</span><span class="sxs-lookup"><span data-stu-id="88d6f-151">requestState</span></span>|<span data-ttu-id="88d6f-152">Строка</span><span class="sxs-lookup"><span data-stu-id="88d6f-152">String</span></span>|<span data-ttu-id="88d6f-153">Один `PendingApproval` из `Canceled` , , , , , или  `Denied` `Delivering` `Delivered` `PartiallyDelivered` `Submitted` `Scheduled` .</span><span class="sxs-lookup"><span data-stu-id="88d6f-153">One of `PendingApproval`, `Canceled`,  `Denied`, `Delivering`, `Delivered`, `PartiallyDelivered`, `Submitted` or `Scheduled`.</span></span> <span data-ttu-id="88d6f-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="88d6f-154">Read-only.</span></span>|
|<span data-ttu-id="88d6f-155">requestStatus</span><span class="sxs-lookup"><span data-stu-id="88d6f-155">requestStatus</span></span>|<span data-ttu-id="88d6f-156">Строка</span><span class="sxs-lookup"><span data-stu-id="88d6f-156">String</span></span>|<span data-ttu-id="88d6f-157">Дополнительные сведения о состоянии обработки запросов.</span><span class="sxs-lookup"><span data-stu-id="88d6f-157">More information on the request processing status.</span></span> <span data-ttu-id="88d6f-158">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="88d6f-158">Read-only.</span></span>|
|<span data-ttu-id="88d6f-159">requestType</span><span class="sxs-lookup"><span data-stu-id="88d6f-159">requestType</span></span>|<span data-ttu-id="88d6f-160">Строка</span><span class="sxs-lookup"><span data-stu-id="88d6f-160">String</span></span>|<span data-ttu-id="88d6f-161">Один `UserAdd` из `UserRemove` , , или `AdminAdd` `AdminRemove` `SystemRemove` .</span><span class="sxs-lookup"><span data-stu-id="88d6f-161">One of `UserAdd`, `UserRemove`, `AdminAdd`, `AdminRemove` or `SystemRemove`.</span></span> <span data-ttu-id="88d6f-162">Запрос от самого пользователя будет иметь requestType или `UserAdd` `UserRemove` .</span><span class="sxs-lookup"><span data-stu-id="88d6f-162">A request from the user themselves would have requestType of `UserAdd` or `UserRemove`.</span></span> <span data-ttu-id="88d6f-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="88d6f-163">Read-only.</span></span>|
|<span data-ttu-id="88d6f-164">schedule</span><span class="sxs-lookup"><span data-stu-id="88d6f-164">schedule</span></span>|[<span data-ttu-id="88d6f-165">requestSchedule</span><span class="sxs-lookup"><span data-stu-id="88d6f-165">requestSchedule</span></span>](requestschedule.md)| <span data-ttu-id="88d6f-166">Диапазон дат, которые должен быть назначен запросчику.</span><span class="sxs-lookup"><span data-stu-id="88d6f-166">The range of dates that access is to be assigned to the requestor.</span></span> <span data-ttu-id="88d6f-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="88d6f-167">Read-only.</span></span>|
|<span data-ttu-id="88d6f-168">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="88d6f-168">accessPackageAssignment</span></span>|[<span data-ttu-id="88d6f-169">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="88d6f-169">accessPackageAssignment</span></span>](accesspackageassignment.md)| <span data-ttu-id="88d6f-170">Для requestType или , это назначение пакета `UserAdd` `AdminAdd` доступа, запрашиваемого для создания.</span><span class="sxs-lookup"><span data-stu-id="88d6f-170">For a requestType of `UserAdd` or `AdminAdd`, this is an access package assignment requested to be created.</span></span>  <span data-ttu-id="88d6f-171">Для requestType или , это свойство существующего `UserRemove` `AdminRemove` `SystemRemove` `id` назначения, которые будут удалены.</span><span class="sxs-lookup"><span data-stu-id="88d6f-171">For a requestType of `UserRemove`, `AdminRemove` or `SystemRemove`, this has the `id` property of an existing assignment to be removed.</span></span>|
|<span data-ttu-id="88d6f-172">ответы</span><span class="sxs-lookup"><span data-stu-id="88d6f-172">answers</span></span>|<span data-ttu-id="88d6f-173">[коллекция accessPackageAnswer](accesspackageanswer.md)</span><span class="sxs-lookup"><span data-stu-id="88d6f-173">[accessPackageAnswer](accesspackageanswer.md) collection</span></span>|<span data-ttu-id="88d6f-174">Ответы, предоставленные запрашивателем для [доступа кPackageQuestions,](accesspackagequestion.md) заданные им во время запроса.</span><span class="sxs-lookup"><span data-stu-id="88d6f-174">Answers provided by the requestor to [accessPackageQuestions](accesspackagequestion.md) asked of them at the time of request.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88d6f-175">Связи</span><span class="sxs-lookup"><span data-stu-id="88d6f-175">Relationships</span></span>

| <span data-ttu-id="88d6f-176">Связь</span><span class="sxs-lookup"><span data-stu-id="88d6f-176">Relationship</span></span> | <span data-ttu-id="88d6f-177">Тип</span><span class="sxs-lookup"><span data-stu-id="88d6f-177">Type</span></span>        | <span data-ttu-id="88d6f-178">Описание</span><span class="sxs-lookup"><span data-stu-id="88d6f-178">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="88d6f-179">accessPackage</span><span class="sxs-lookup"><span data-stu-id="88d6f-179">accessPackage</span></span>|[<span data-ttu-id="88d6f-180">accessPackage</span><span class="sxs-lookup"><span data-stu-id="88d6f-180">accessPackage</span></span>](../resources/accesspackage.md)|<span data-ttu-id="88d6f-181">Пакет доступа, связанный с accessPackageAssignmentRequest.</span><span class="sxs-lookup"><span data-stu-id="88d6f-181">The access package associated with the accessPackageAssignmentRequest.</span></span> <span data-ttu-id="88d6f-182">Пакет доступа определяет коллекции ролей ресурсов и политики получения доступа к этим ресурсам для одного или более пользователей.</span><span class="sxs-lookup"><span data-stu-id="88d6f-182">An access package defines the collections of resource roles and the policies for how one or more users can get access to those resources.</span></span> <span data-ttu-id="88d6f-183">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="88d6f-183">Read-only.</span></span> <span data-ttu-id="88d6f-184">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="88d6f-184">Nullable.</span></span>|
|<span data-ttu-id="88d6f-185">запросчик</span><span class="sxs-lookup"><span data-stu-id="88d6f-185">requestor</span></span>|[<span data-ttu-id="88d6f-186">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="88d6f-186">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="88d6f-187">Субъекту, который запрашивал или, если прямое назначение, было назначено.</span><span class="sxs-lookup"><span data-stu-id="88d6f-187">The subject who requested or, if a direct assignment, was assigned.</span></span> <span data-ttu-id="88d6f-188">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="88d6f-188">Read-only.</span></span> <span data-ttu-id="88d6f-189">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="88d6f-189">Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="88d6f-190">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="88d6f-190">JSON representation</span></span>

<span data-ttu-id="88d6f-191">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="88d6f-191">The following is a JSON representation of the resource.</span></span>

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

